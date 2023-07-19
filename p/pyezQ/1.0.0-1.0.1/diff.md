# Comparing `tmp/pyezQ-1.0.0-py3-none-any.whl.zip` & `tmp/pyezQ-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17542 bytes, number of entries: 13
--rw-r--r--  2.0 unx    36315 b- defN 23-May-23 16:48 pyezQ.py
+Zip file size: 18253 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    39509 b- defN 23-Jul-19 03:44 pyezQ.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 07:55 qasm_to_qcis/__init__.py
 -rw-r--r--  2.0 unx     3973 b- defN 23-May-09 07:55 qasm_to_qcis/const.py
 -rw-r--r--  2.0 unx     7262 b- defN 23-May-09 07:55 qasm_to_qcis/qasm.py
 -rw-r--r--  2.0 unx     9361 b- defN 23-May-09 07:55 qasm_to_qcis/qasm_to_qcis.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 07:55 qcis_to_qasm/__init__.py
 -rw-r--r--  2.0 unx      409 b- defN 23-May-09 07:55 qcis_to_qasm/const.py
 -rw-r--r--  2.0 unx     2624 b- defN 23-May-09 07:55 qcis_to_qasm/qcis.py
 -rw-r--r--  2.0 unx     1638 b- defN 23-May-09 07:55 qcis_to_qasm/qcis_to_qasm.py
--rw-r--r--  2.0 unx     2472 b- defN 23-May-23 16:54 pyezQ-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 16:54 pyezQ-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       32 b- defN 23-May-23 16:54 pyezQ-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      991 b- defN 23-May-23 16:54 pyezQ-1.0.0.dist-info/RECORD
-13 files, 65169 bytes uncompressed, 15904 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     2472 b- defN 23-Jul-19 03:46 pyezQ-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 03:46 pyezQ-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       32 b- defN 23-Jul-19 03:46 pyezQ-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      991 b- defN 23-Jul-19 03:46 pyezQ-1.0.1.dist-info/RECORD
+13 files, 68363 bytes uncompressed, 16615 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: qcis_to_qasm/qcis.py
 Comment: 
 
 Filename: qcis_to_qasm/qcis_to_qasm.py
 Comment: 
 
-Filename: pyezQ-1.0.0.dist-info/METADATA
+Filename: pyezQ-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pyezQ-1.0.0.dist-info/WHEEL
+Filename: pyezQ-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyezQ-1.0.0.dist-info/top_level.txt
+Filename: pyezQ-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyezQ-1.0.0.dist-info/RECORD
+Filename: pyezQ-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyezQ.py

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 import json
 import requests
 import re
+import os
+import shutil
 from time import time, sleep
 import random
 import numpy as np
 import traceback
 import datetime
 from isqmap import transpile
 from qcis_to_qasm.qcis_to_qasm import QcisToQasm
 from qasm_to_qcis.qasm_to_qcis import QasmToQcis
 from sabreMapper.sabre_mapper import SabreMapper
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Union
 
 
 class Account():
 
     def __init__(
             self,
             login_key: Optional[str]=None,
@@ -102,25 +104,28 @@
         lab_id = result.get('data').get('lab_id')
         return lab_id
 
     def save_experiment(
             self,
             lab_id: str,
             exp_data: str,
-            version: str
+            version: str,
+            is_verify: Optional[bool]=True
         ):
         """save the experiment and return the experiment ID.
 
         Args:
             lab_id: 
                 the result returned by the create_experiment interface, experimental set id
             exp_data: 
                 experimental content, qics
             version: 
                 version description
+            is_verify:
+                Is the circuit verified.True verify, False do not verify. Defaults to True.
         
         Examples:
             the input parameter can be the following value:
 
                 lab_id: XXX
                 exp_data:
                     X Q1
@@ -153,15 +158,16 @@
         if self.computer_selection_mark:
             url = f'{self.base_url}/sdk/api/multiple/experiment/detail/save'
         else:
             url = f'{self.base_url}/sdk/api/experiment/detail/save'
         data = {
             "circuit": exp_data, "lab_id": lab_id,
             "language": "qcis", "version": version,
-            "machineName": self.machine_name
+            "machineName": self.machine_name,
+            "is_verify": is_verify
         }
         headers = {"sdk_token": self.token}
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
         if status_code != 200:
             return 0
         result = json.loads(res.text)
@@ -210,15 +216,15 @@
             print(f'运行实验失败：{msg}')
             return 0
         run_result = result.get('data').get('query_id')
         return run_result
 
     def query_experiment(
             self,
-            query_id: str,
+            query_id: Union[str, List[str]],
             max_wait_time: Optional[int]=60,
             result_type=2
         ):
         """query experimental results
 
         Args:
             query_id: 
@@ -226,34 +232,37 @@
             max_wait_time: 
                 maximum waiting time for querying experiments. Defaults to 60.
             result_type: 
                 election of return value type of other quantum computer except oneD12,
                 only probability is returned by oneD12,
                 result_type value of 0 represents the raw data, 
                 and a value of 1 represents the probability valueDefaults to 2.
+            
+            The maximum number of experimental result queries supported by the server is 50.
+            If there are more than 50, an error message will be displayed.
 
         Raises:
             Exception: query experiment result type error
 
         Returns:
             Union[int, str]: 0 failed, not 0 successful, success returns the experimental result
         """
+        if isinstance(query_id, str):
+            query_id = [query_id]
         t0 = time()
         while time()-t0 < max_wait_time:
             try:
                 if self.computer_selection_mark:
                     url = f'{self.base_url}/sdk/api/multiple/experiment/find/results'
                     if result_type not in [0, 1, 2]:
                         raise Exception('查询实验结果类型错误')
                 else:
                     url = f'{self.base_url}/sdk/api/experiment/find/results'
                     result_type = 1                
-                data = {"circuit": "", "exp_id": "", "lab_id": "",
-                        "quantumComputer": "", "query_id": query_id,
-                        "shots": 0, "version": "string", "type": result_type}
+                data = {"query_id": query_id, "type": result_type}
                 headers = {"sdk_token": self.token}
                 res = requests.post(url, json=data, headers=headers)
                 status_code = res.status_code
                 if status_code != 200:
                     return 0
                 result = json.loads(res.text)
                 code = result.get('code', -1)
@@ -273,22 +282,23 @@
             print(f'查询实验结果请等待: {{:.2f}}秒'.format(sleep_time))
             sleep(sleep_time)
         print(f'查询实验结果失败')
         return 0
 
     def submit_job(
             self,
-            circuit: Optional[str]=None,
+            circuit: Optional[Union[List, str]]=None,
             exp_name: Optional[str]="exp0",
-            parameters: Optional[List]=None,
-            values: Optional[List]=None,
+            parameters: Optional[List[List]]=None, 
+            values: Optional[List[List]]=None,
             num_shots: Optional[int]=12000,
             lab_id: Optional[str]=None,
             exp_id: Optional[str]=None,
-            version: Optional[str]="version01"
+            version: Optional[str]="version01",
+            is_verify: Optional[bool]=True
         ):
         """submit experimental tasks
 
         Args:
             circuit: 
                 experimental content, qics. Defaults to None.
             exp_name:
@@ -301,32 +311,52 @@
                 number of repetitions per experiment. Defaults to 12000.
             lab_id: 
                 the result returned by the create_experiment interface, experimental set id. Defaults to None.
             exp_id: 
                 the result returned by the save_experiment interface, experimental id. Defaults to None.
             version: 
                 version description. Defaults to 'version01'.
+            is_verify:
+                Is the circuit verified.True verify, False do not verify. Defaults to True.
+            
+            There are some parameter range limitations when using batch submission circiuts.
+                1. circuits length less than 50
+                   numshots maximum 100000
+                   the number of measurement qubits is less than 15
+                2. circuits length greater than 50 but less than 100
+                   numshots maximum 50000
+                   the number of measurement qubits is less than 30
+                3. circuits length greater than 100 but less than 600
+                   numshots maximum 10000
+                   the number of measurement bits is less than the number of all available qubits
 
         Returns:
             Union[int, str]: 0 failed, not 0 successful, success returns the query id.
         """
-        if circuit:
-            circuit = self.assign_parameters(
-                circuit.upper(), parameters, values)
-            if not circuit:
+        if isinstance(circuit, str):
+            circuit = [circuit]
+        if len(circuit) > 1:
+            version = None
+        if circuit and parameters and values and len(parameters) == len(circuit) == len(values):
+            new_circuit = self.assign_parameters(circuit, parameters, values)
+            if not new_circuit:
                 print('无法为线路赋值，请检查线路，参数和参数值之后重试')
                 return 0
+        else:
+            new_circuit = circuit
         if self.computer_selection_mark:
             url = f'{self.base_url}/sdk/api/multiple/experiment/temporary/save'
         else:
             url = f'{self.base_url}/sdk/api/experiment/temporary/save'
         data = {"circuit": circuit, "exp_id": exp_id,
                 "lab_id": lab_id, "name": exp_name,
                 "shots": num_shots, "version": version,
-                "machineName": self.machine_name, "source": 'SDK'}
+                "machineName": self.machine_name, "source": 'SDK',
+                "is_verify": is_verify
+            }
         headers = {"sdk_token": self.token}
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
         if status_code != 200:
             return 0
         result = json.loads(res.text)
         code = result.get('code', -1)
@@ -334,18 +364,18 @@
         if code != 0:
             print(f'运行实验失败：{msg}')
             return 0
         run_result = result.get('data').get('query_id')
         return run_result
 
     def assign_parameters(
-            self, 
-            circuit: str, 
-            parameters: List, 
-            values: List
+            self,
+            circuits: List[str], 
+            parameters: List[List], 
+            values: List[List]
         ):
         """Check if the number of parameters, values match the circuit definition
 
         Args:
             circuit: 
                 string, QCIS circuit definition with or without parameter place holder
             parameters: 
@@ -353,63 +383,65 @@
             values: 
                 list or ndarray of floats, values to be assigned
 
         Returns:
             circuit: circuit with parameters replaced by values or empty string
             empty string occurs when errors prevents parameters to be assigned
         """
-        circuit = circuit.upper()
-        p = re.compile(r'\{(\w+)\}')
-        circuit_parameters = p.findall(circuit)
-        if circuit_parameters:
-
-            # 如果values为整数或浮点数，改为列表格式##########################################################
-            if isinstance(values, (float, int)):
-                values = [values]
-            # 如果parameters为字符格式，改为列表格式#########################################################
-            if isinstance(parameters, str):
-                parameters = [parameters]
-            # 将所有parameter变为大写， 否则set(parameters) != set(circuit_parameters) 不通过 ###############
-            parameters = [p.upper() for p in parameters]
-
-            if not values:
-                error_message = f'线路含有参数{circuit_parameters}, 请提供相应的参数值'
-                print(error_message)
-                return ''
+        new_circuit = []
+        for circuit, parameter, value in zip(circuits, parameters, values):
+            circuit = circuit.upper()
+            p = re.compile(r'\{(\w+)\}')
+            circuit_parameters = p.findall(circuit)
+            if circuit_parameters:
+                # # 如果values为整数或浮点数，改为列表格式##########################################################
+                # if isinstance(values, (float, int)):
+                #     values = [values]
+                # # 如果parameters为字符格式，改为列表格式#########################################################
+                # if isinstance(parameters, str):
+                #     parameters = [parameters]
+                
+                # 将所有parameter变为大写， 否则set(parameters) != set(circuit_parameters) 不通过 ###############
+                parameters = [p.upper() for p in parameter]
 
-            else:
-                if len(circuit_parameters) != len(values):
-                    error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(values)}个参数值'
-                    print(error_message)
-                    return ''
-
-                elif parameters and len(circuit_parameters) != len(parameters):
-                    error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(parameters)}个参数'
+                if not value:
+                    error_message = f'线路含有参数{circuit_parameters}, 请提供相应的参数值'
                     print(error_message)
                     return ''
 
-                elif set(parameters) != set(circuit_parameters):
-                    error_message = '线路中的参数与您输入的参数名称不符'
-                    print(error_message)
                 else:
-                    param_dic = {}
-                    ############################# 这个转化可以删了 #########################################
-                    # parameters_upper = [p.upper() for p in parameters]
-                    for p, v in zip(parameters, values):
-                        param_dic[p] = v
-                    expData = circuit.format(**param_dic)
-                    return expData
-
-        elif parameters or values:
-            error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
-            print(error_message)
-            return ''
-        else:
-            expData = circuit
-            return expData
+                    if len(circuit_parameters) != len(value):
+                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(value)}个参数值'
+                        print(error_message)
+                        return ''
+
+                    elif parameter and len(circuit_parameters) != len(parameter):
+                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(parameter)}个参数'
+                        print(error_message)
+                        return ''
+                    
+                    elif set(parameter) != set(circuit_parameters):
+                        error_message = '线路中的参数与您输入的参数名称不符'
+                        print(error_message)
+                    else:
+                        param_dic = {}
+                        ############################# 这个转化可以删了 #########################################
+                        #parameters_upper = [p.upper() for p in parameters]
+                        for p, v in zip(parameter, value):
+                            param_dic[p] = v
+                        expData = circuit.format(**param_dic)
+                        new_circuit.append(expData)
+            elif parameter or value:
+                error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
+                print(error_message)
+                return ''
+            else:
+                expData = circuit
+                new_circuit.append(expData)
+        return new_circuit
 
     def get_experiment_data(
             self, 
             circuit: str):
         """Parse circuit description and generate 
            experiment script and extract number of measured qubits.
 
@@ -783,14 +815,40 @@
                 inv_CM = np.kron(inv_CM, inv_cm)
             CM_CACHE[f] = inv_CM
         else:
             inv_CM = CM_CACHE[f]
         Pi = np.dot(inv_CM, (np.array(Pm, ndmin=2).T))
         Pi = {bin(idx)[2:].zfill(n): k[0] for idx, k in enumerate(Pi)}
         return Pi
+    
+    # 对矫正后的概率进行修正
+    def probability_correction(self, probabilities):
+        """correction of the measured probability of 01 quantum state.
+           If there is a probability greater than 1, change this item to 1; 
+           If there is anything less than 0, change the item to 0.
+
+        Args:
+            probabilities:
+               corrected probability.
+            
+        Returns:
+            Dict: corrected probability.
+        """
+        abnormal_fidelity_list = list(filter(lambda x: x < 0 or x > 1, probabilities.values()))
+        if not abnormal_fidelity_list:
+            return probabilities
+        for k, v in probabilities.items():
+            if v > 1:
+                probabilities[k] = 1
+            elif v < 0:
+                probabilities[k] = 0
+        fidelity_sum = sum(probabilities.values())
+        for k, v in probabilities.items():
+            probabilities[k] = v / fidelity_sum
+        return probabilities
 
     def qcis_mapping_isq(
             self,
             qcis_circuit: str,
             initial_layout: Optional[Dict]=None,
             objective: Optional[str]='size',
             seed: Optional[int]=None,
@@ -835,19 +893,21 @@
             qasm_transpiled, _, _, _ = transpile(qasm_circuit,
                                                  qpu_file,
                                                  initial_layout=initial_layout,
                                                  objective=objective,
                                                  seed=seed,
                                                  use_post_opt=use_post_opt)
             simplity_qcis = self.convert_qasm_to_qcis(qasm_transpiled)
+            os.remove(qpu_file)
             return simplity_qcis
         except Exception as e:
             print(e)
             print(traceback.format_exc())
             print('circuit mapping error, will submit using the original route')
+            os.remove(qpu_file)
             return qcis_circuit
 
     def qcis_mapping_sabre(
             self, 
             qcis_circuit: str):
         """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
            and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
@@ -861,15 +921,18 @@
         """
         if not self.computer_selection_mark:
             raise Exception(f'current quantum computer does not support qcis_mapping_quingo')
         config_json = self.download_config(down_file=False)
         try:
             # qcis转换成qasm并写入qasm_file中
             qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis_circuit)
-            qasm_file = 'temp/qasm.qasm'
+            folder_path = 'temp'
+            if not os.path.exists(folder_path): 
+                os.makedirs(folder_path)
+            qasm_file = f'{folder_path}/qasm.qasm'
             with open(qasm_file, 'w') as f:
                 f.write(qasm_circuit)
             sabre = SabreMapper()
             # 组装chip_info_fn映射信息
             chip_info_fn = {}
             couplings = []
             coupler_maps = config_json.get('overview').get('coupler_map')
@@ -890,33 +953,36 @@
             qubit_fidelity = {}
             for qubit, error in zip(qubit_used, qubit_gate_error):
                 qubit_fidelity[qubit] = 1 - error
             chip_info_fn['fidelity'] = qubit_fidelity
             chip_info_fn['has multiple chips'] = False
             chip_info_fn['qubits'] = qubit_used
 
-            chip_info_fn_file = "temp/chip_info_fn.json"
-            mapped_qasm_fn_file = "temp/mapped_qasm_fn.qasm"
-            qubit_mapping_fn_file = "temp/qubit_mapping_fn.json"
+            chip_info_fn_file = f'{folder_path}/chip_info_fn.json'
+            mapped_qasm_fn_file = f'{folder_path}/mapped_qasm_fn.qasm'
+            qubit_mapping_fn_file = f'{folder_path}/qubit_mapping_fn.json'
             with open(chip_info_fn_file, 'w') as f:
                 json.dump(chip_info_fn, f)
             # 调用quMapper做mapping操作
             success = sabre.map_schedule(
                 qasm_file, chip_info_fn_file, mapped_qasm_fn_file, qubit_mapping_fn_file)
             if success:
                 with open(qubit_mapping_fn_file, 'r') as f:
                     qubit_mapping_fn = json.load(f)
                 qubit_map = qubit_mapping_fn.get('physical qubits idx')
                 # mapping成功，将转换后的qasm转为qcis，其中编号根据physical qubits idx做映射
                 simplity_qcis = self.convert_qasm_to_qcis_from_file(
                     mapped_qasm_fn_file, qubit_map)
+                shutil.rmtree(folder_path)
                 return simplity_qcis
         except Exception as e:
             print(e)
+            print(traceback.format_exc())            
             print('circuit mapping error, will submit using the original route')
+            shutil.rmtree(folder_path)
             return qcis_circuit
     
     def get_experiment_circuit(
             self,
             exp_id: str):
         """according to the exp_id obtained experimental circuit
```

## Comparing `pyezQ-1.0.0.dist-info/METADATA` & `pyezQ-1.0.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyezQ
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK to use Quantum Computer @ quantumcomputer.ac.cn with QCIS.
 Home-page: https://quantumcomputer.ac.cn
 Author: Code42
 Author-email: support@quantumcomputer.ac.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 
 中科院量子创新院量子计算云平台, 2023年4月14日开放新机内测，官方网址：[https://quantumcomputer.ac.cn](https://quantumcomputer.ac.cn)
   
 如需申请新量子计算机使用权限，可以[参考这里](https://quantumcomputer.ac.cn/Forum/reply/21a180c9fcdd43098303cac6b98adff4/9b6aa8fddaf64925a05f1764fdec011c.html)
 
 本地快速安装SDK环境，请使用如下指令：
 ```python title='本地快速安装SDK环境，请使用如下指令：'
-pip install --upgrade ezQpy -i  https://pypi.tuna.tsinghua.edu.cn/simple
+pip install --upgrade pyezQ -i  https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 因近期内测调整较快，如遇到原有程序运行报错，或无法提交线路等问题，请及时联系官方人员或用以下指令更新SDK库。  
 同理，近期依赖关系有可能列的不全，用户可以根据报错提示来进行安装。  
 如遇国内源暂未同步，请强行指定国外原进行更新安装-i  https://pypi.org/simple  
   
 在云平台网站提供的jupyternotebook环境Tutorial目录下，可以得到可互动执行的例子程序，复制到个人目录后，可以快速运行。
```

## Comparing `pyezQ-1.0.0.dist-info/RECORD` & `pyezQ-1.0.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-pyezQ.py,sha256=M-YAGZmiQ5XnhV_eWLwPXwYiCnzgrm9JaAP64d1q0gI,36315
+pyezQ.py,sha256=Z8aGysdW0i0OeGeuaButTKcQKgMMotTlBp8sy-8GPDs,39509
 qasm_to_qcis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qasm_to_qcis/const.py,sha256=AZTrt8AjrREnIHsK_VQrd_fEcB3TNBJqR1TiatsIurY,3973
 qasm_to_qcis/qasm.py,sha256=_Pg4L8n40ygv0fE3IowEf6UxN_Y9K1tpmPUE_pUrPAk,7262
 qasm_to_qcis/qasm_to_qcis.py,sha256=xyz90kTp_J5YdbJs0BkQibDlJtN7ojThQfAwImcwZlg,9361
 qcis_to_qasm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qcis_to_qasm/const.py,sha256=jeuG0MbtqK3MxFlCC_eGwlsUO1nYp6B20KGztuJgmoc,409
 qcis_to_qasm/qcis.py,sha256=540IlWuMLhYgMCkGPFhFrJNHvmvGQLkm_ua61Bhw5sE,2624
 qcis_to_qasm/qcis_to_qasm.py,sha256=yPhCZvJIO9jnlleaeOwtmxuaO6bX8m-PoAVjjevHgT4,1638
-pyezQ-1.0.0.dist-info/METADATA,sha256=m7h9Y4XYVK_X5lXKTowC_KV09f3A3w4FTwFnd2Ev0co,2472
-pyezQ-1.0.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-pyezQ-1.0.0.dist-info/top_level.txt,sha256=_65c41HXDYn-w5gTDBgee8mYSgbEV4LjLYHe3gVv5dU,32
-pyezQ-1.0.0.dist-info/RECORD,,
+pyezQ-1.0.1.dist-info/METADATA,sha256=u3tHFr0LWTi1fouU5hPrPBhNm-Uh56bOJOb5CSYyJuw,2472
+pyezQ-1.0.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+pyezQ-1.0.1.dist-info/top_level.txt,sha256=_65c41HXDYn-w5gTDBgee8mYSgbEV4LjLYHe3gVv5dU,32
+pyezQ-1.0.1.dist-info/RECORD,,
```

