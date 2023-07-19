# Comparing `tmp/smartwatts-2.1.1.tar.gz` & `tmp/smartwatts-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartwatts-2.1.1.tar", last modified: Wed Jun 14 13:41:28 2023, max compression
+gzip compressed data, was "smartwatts-2.1.2.tar", last modified: Wed Jul 19 14:18:09 2023, max compression
```

## Comparing `smartwatts-2.1.1.tar` & `smartwatts-2.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.426062 smartwatts-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-14 13:41:16.000000 smartwatts-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-14 13:41:28.426062 smartwatts-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-14 13:41:16.000000 smartwatts-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-14 13:41:16.000000 smartwatts-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:41:28.426062 smartwatts-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.422062 smartwatts-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.422062 smartwatts-2.1.1/src/smartwatts/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.422062 smartwatts-2.1.1/src/smartwatts/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/actor/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/actor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.422062 smartwatts-2.1.1/src/smartwatts/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/cli/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.422062 smartwatts-2.1.1/src/smartwatts/handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/handler/hwpc_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.426062 smartwatts-2.1.1/src/smartwatts/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/model/cpu_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/model/power_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 13:41:16.000000 smartwatts-2.1.1/src/smartwatts/model/report_history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:28.422062 smartwatts-2.1.1/src/smartwatts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-14 13:41:28.000000 smartwatts-2.1.1/src/smartwatts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 13:41:28.000000 smartwatts-2.1.1/src/smartwatts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:41:28.000000 smartwatts-2.1.1/src/smartwatts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 13:41:28.000000 smartwatts-2.1.1/src/smartwatts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 13:41:28.000000 smartwatts-2.1.1/src/smartwatts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.906573 smartwatts-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-19 14:17:54.000000 smartwatts-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-19 14:18:09.906573 smartwatts-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-19 14:17:54.000000 smartwatts-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-19 14:17:54.000000 smartwatts-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:18:09.906573 smartwatts-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/smartwatts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/smartwatts/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/actor/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/actor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/smartwatts/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/cli/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/smartwatts/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/handler/hwpc_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/smartwatts/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/model/cpu_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/model/power_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-19 14:17:54.000000 smartwatts-2.1.2/src/smartwatts/model/report_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:18:09.902573 smartwatts-2.1.2/src/smartwatts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-19 14:18:09.000000 smartwatts-2.1.2/src/smartwatts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-19 14:18:09.000000 smartwatts-2.1.2/src/smartwatts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:18:09.000000 smartwatts-2.1.2/src/smartwatts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 14:18:09.000000 smartwatts-2.1.2/src/smartwatts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 14:18:09.000000 smartwatts-2.1.2/src/smartwatts.egg-info/top_level.txt
```

### Comparing `smartwatts-2.1.1/LICENSE` & `smartwatts-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/PKG-INFO` & `smartwatts-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartwatts
-Version: 2.1.1
+Version: 2.1.2
 Summary: SmartWatts is a formula for a self-adaptive software-defined power meter based on the PowerAPI framework.
 Author-email: Guillaume Fieni <guillaume.fieni@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/smartwatts-formula
 Keywords: powerapi,energy,power-meter,power-model,green-computing,containers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartwatts Version: 2.1.1 Summary: SmartWatts is a
+Metadata-Version: 2.1 Name: smartwatts Version: 2.1.2 Summary: SmartWatts is a
 formula for a self-adaptive software-defined power meter based on the PowerAPI
 framework. Author-email: Guillaume Fieni
 fieni@inria.fr> License: BSD-3-Clause Project-URL: homepage, https://
 powerapi.org Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/smartwatts-formula
 Keywords: powerapi,energy,power-meter,power-model,green-computing,containers
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `smartwatts-2.1.1/README.md` & `smartwatts-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/pyproject.toml` & `smartwatts-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 
 authors = [
     {name = "Guillaume Fieni", email = "guillaume.fieni@inria.fr"},
 ]
 
 dependencies = [
-    "powerapi[everything] == 2.0.4",
+    "powerapi[everything] == 2.1.0",
     "scikit-learn >= 0.20.2",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest >= 3.9.2",
     "pytest-cov >= 4.0.0",
```

### Comparing `smartwatts-2.1.1/src/smartwatts/__init__.py` & `smartwatts-2.1.2/src/smartwatts/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
```

### Comparing `smartwatts-2.1.1/src/smartwatts/__main__.py` & `smartwatts-2.1.2/src/smartwatts/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 from powerapi import __version__ as powerapi_version
 from powerapi.backend_supervisor import BackendSupervisor
 from powerapi.cli.common_cli_parsing_manager import CommonCLIParsingManager
 from powerapi.cli.config_parser import store_true
 from powerapi.cli.generator import PusherGenerator, PullerGenerator
 from powerapi.dispatch_rule import HWPCDispatchRule, HWPCDepthLevel
 from powerapi.dispatcher import DispatcherActor, RouteTable
-from powerapi.exception import PowerAPIException, MissingArgumentException, NotAllowedArgumentValueException, \
-    FileDoesNotExistException
+from powerapi.exception import PowerAPIException, MissingArgumentException, NotAllowedArgumentValueException, FileDoesNotExistException
 from powerapi.filter import Filter
 from powerapi.report import HWPCReport
 
 from smartwatts import __version__ as smartwatts_version
 from smartwatts.actor import SmartWattsFormulaActor, SmartWattsFormulaScope, SmartWattsFormulaConfig
 from smartwatts.cli import SmartWattsConfigValidator
 from smartwatts.exceptions import InvalidConfigurationParameterException
@@ -53,60 +52,41 @@
 
 
 def generate_smartwatts_parser() -> CommonCLIParsingManager:
     """
     Construct and returns the SmartWatts cli parameters parser.
     :return: SmartWatts cli parameters parser
     """
-    parser_manager = CommonCLIParsingManager()
+    pm = CommonCLIParsingManager()
 
     # Formula control parameters
-    parser_manager.add_argument_to_cli_parser('disable-cpu-formula', help_text='Disable CPU formula', is_flag=True,
-                                              argument_type=bool, default_value=False, action=store_true)
-    parser_manager.add_argument_to_cli_parser('disable-dram-formula', help_text='Disable DRAM formula', is_flag=True,
-                                              argument_type=bool, default_value=False, action=store_true)
+    pm.add_argument('disable-cpu-formula', help_text='Disable CPU formula', is_flag=True, argument_type=bool, default_value=False, action=store_true)
+    pm.add_argument('disable-dram-formula', help_text='Disable DRAM formula', is_flag=True, argument_type=bool, default_value=False, action=store_true)
 
     # Formula RAPL reference event
-    parser_manager.add_argument_to_cli_parser('cpu-rapl-ref-event',
-                                              help_text='RAPL event used as reference for the CPU power models',
-                                              default_value='RAPL_ENERGY_PKG')
-    parser_manager.add_argument_to_cli_parser('dram-rapl-ref-event',
-                                              help_text='RAPL event used as reference for the DRAM power models',
-                                              default_value='RAPL_ENERGY_DRAM')
+    pm.add_argument('cpu-rapl-ref-event', help_text='RAPL event used as reference for the CPU power models', default_value='RAPL_ENERGY_PKG')
+    pm.add_argument('dram-rapl-ref-event', help_text='RAPL event used as reference for the DRAM power models', default_value='RAPL_ENERGY_DRAM')
 
     # CPU topology information
-    parser_manager.add_argument_to_cli_parser('cpu-tdp', help_text='CPU TDP (in Watt)', argument_type=int,
-                                              default_value=400)
-    parser_manager.add_argument_to_cli_parser('cpu-base-clock', help_text='CPU base clock (in MHz)', argument_type=int,
-                                              default_value=100)
-    parser_manager.add_argument_to_cli_parser('cpu-base-freq', help_text='CPU base frequency (in MHz)',
-                                              argument_type=int, default_value=2100)
+    pm.add_argument('cpu-tdp', help_text='CPU TDP (in Watt)', argument_type=int, default_value=400)
+    pm.add_argument('cpu-base-clock', help_text='CPU base clock (in MHz)', argument_type=int, default_value=100)
+    pm.add_argument('cpu-base-freq', help_text='CPU base frequency (in MHz)', argument_type=int, default_value=2100)
 
     # Formula error threshold
-    parser_manager.add_argument_to_cli_parser('cpu-error-threshold',
-                                              help_text='Error threshold for the CPU power models (in Watt)',
-                                              argument_type=float, default_value=2.0)
-    parser_manager.add_argument_to_cli_parser('dram-error-threshold',
-                                              help_text='Error threshold for the DRAM power models (in Watt)',
-                                              argument_type=float, default_value=2.0)
+    pm.add_argument('cpu-error-threshold', help_text='Error threshold for the CPU power models (in Watt)', argument_type=float, default_value=2.0)
+    pm.add_argument('dram-error-threshold', help_text='Error threshold for the DRAM power models (in Watt)', argument_type=float, default_value=2.0)
 
     # Sensor information
-    parser_manager.add_argument_to_cli_parser('sensor-reports-frequency',
-                                              help_text='The frequency with which measurements are made (in milliseconds)',
-                                              argument_type=int, default_value=1000)
+    pm.add_argument('sensor-reports-frequency', help_text='The frequency with which measurements are made (in milliseconds)', argument_type=int, default_value=1000)
 
     # Learning parameters
-    parser_manager.add_argument_to_cli_parser('learn-min-samples-required',
-                                              help_text='Minimum amount of samples required before trying to learn a power model',
-                                              argument_type=int, default_value=10)
-    parser_manager.add_argument_to_cli_parser('learn-history-window-size',
-                                              help_text='Size of the history window used to keep samples to learn from',
-                                              argument_type=int, default_value=60)
+    pm.add_argument('learn-min-samples-required', help_text='Minimum amount of samples required before trying to learn a power model', argument_type=int, default_value=10)
+    pm.add_argument('learn-history-window-size', help_text='Size of the history window used to keep samples to learn from', argument_type=int, default_value=60)
 
-    return parser_manager
+    return pm
 
 
 def generate_formula_configuration(config: Dict, cpu_topology: CPUTopology, scope: SmartWattsFormulaScope) -> SmartWattsFormulaConfig:
     """
     Generate a SmartWatts actor configuration.
     """
     reports_freq = config['sensor-reports-frequency']
```

### Comparing `smartwatts-2.1.1/src/smartwatts/actor/__init__.py` & `smartwatts-2.1.2/src/smartwatts/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/actor/actor.py` & `smartwatts-2.1.2/src/smartwatts/actor/actor.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/actor/config.py` & `smartwatts-2.1.2/src/smartwatts/actor/config.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/cli/__init__.py` & `smartwatts-2.1.2/src/smartwatts/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/cli/config_validator.py` & `smartwatts-2.1.2/src/smartwatts/cli/config_validator.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/exceptions.py` & `smartwatts-2.1.2/src/smartwatts/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/handler/__init__.py` & `smartwatts-2.1.2/src/smartwatts/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/handler/hwpc_report.py` & `smartwatts-2.1.2/src/smartwatts/handler/hwpc_report.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/model/__init__.py` & `smartwatts-2.1.2/src/smartwatts/model/__init__.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/model/cpu_topology.py` & `smartwatts-2.1.2/src/smartwatts/model/cpu_topology.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/model/power_model.py` & `smartwatts-2.1.2/src/smartwatts/model/power_model.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts/model/report_history.py` & `smartwatts-2.1.2/src/smartwatts/model/report_history.py`

 * *Files identical despite different names*

### Comparing `smartwatts-2.1.1/src/smartwatts.egg-info/PKG-INFO` & `smartwatts-2.1.2/src/smartwatts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartwatts
-Version: 2.1.1
+Version: 2.1.2
 Summary: SmartWatts is a formula for a self-adaptive software-defined power meter based on the PowerAPI framework.
 Author-email: Guillaume Fieni <guillaume.fieni@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/smartwatts-formula
 Keywords: powerapi,energy,power-meter,power-model,green-computing,containers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartwatts Version: 2.1.1 Summary: SmartWatts is a
+Metadata-Version: 2.1 Name: smartwatts Version: 2.1.2 Summary: SmartWatts is a
 formula for a self-adaptive software-defined power meter based on the PowerAPI
 framework. Author-email: Guillaume Fieni
 fieni@inria.fr> License: BSD-3-Clause Project-URL: homepage, https://
 powerapi.org Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/smartwatts-formula
 Keywords: powerapi,energy,power-meter,power-model,green-computing,containers
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `smartwatts-2.1.1/src/smartwatts.egg-info/SOURCES.txt` & `smartwatts-2.1.2/src/smartwatts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

