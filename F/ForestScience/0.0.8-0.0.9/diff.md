# Comparing `tmp/ForestScience-0.0.8.tar.gz` & `tmp/ForestScience-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForestScience-0.0.8.tar", last modified: Thu Jul 13 22:11:31 2023, max compression
+gzip compressed data, was "ForestScience-0.0.9.tar", last modified: Wed Jul 19 14:38:38 2023, max compression
```

## Comparing `ForestScience-0.0.8.tar` & `ForestScience-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 22:11:31.453668 ForestScience-0.0.8/
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 22:11:31.274666 ForestScience-0.0.8/ForestScience/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    15160 2023-07-13 22:11:27.000000 ForestScience-0.0.8/ForestScience/InventarioFlorestal.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-13 22:11:27.000000 ForestScience-0.0.8/ForestScience/__init__.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2752 2023-07-13 22:11:27.000000 ForestScience-0.0.8/ForestScience/_modidx.py
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-13 22:11:31.426667 ForestScience-0.0.8/ForestScience.egg-info/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1415 2023-07-13 22:11:30.000000 ForestScience-0.0.8/ForestScience.egg-info/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      399 2023-07-13 22:11:31.000000 ForestScience-0.0.8/ForestScience.egg-info/SOURCES.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 22:11:30.000000 ForestScience-0.0.8/ForestScience.egg-info/dependency_links.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       48 2023-07-13 22:11:30.000000 ForestScience-0.0.8/ForestScience.egg-info/entry_points.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 22:01:51.000000 ForestScience-0.0.8/ForestScience.egg-info/not-zip-safe
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-13 22:11:30.000000 ForestScience-0.0.8/ForestScience.egg-info/requires.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       14 2023-07-13 22:11:30.000000 ForestScience-0.0.8/ForestScience.egg-info/top_level.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11357 2023-07-13 21:42:44.000000 ForestScience-0.0.8/LICENSE
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestScience-0.0.8/MANIFEST.in
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1415 2023-07-13 22:11:31.450666 ForestScience-0.0.8/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      620 2023-07-13 22:06:55.000000 ForestScience-0.0.8/README.md
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      888 2023-07-13 22:11:27.000000 ForestScience-0.0.8/settings.ini
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-13 22:11:31.454668 ForestScience-0.0.8/setup.cfg
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestScience-0.0.8/setup.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-19 14:38:38.666428 ForestScience-0.0.9/
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-19 14:38:38.481427 ForestScience-0.0.9/ForestScience/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    15478 2023-07-19 14:37:54.000000 ForestScience-0.0.9/ForestScience/InventarioFlorestal.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       23 2023-07-19 14:37:54.000000 ForestScience-0.0.9/ForestScience/__init__.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2773 2023-07-19 14:37:54.000000 ForestScience-0.0.9/ForestScience/_modidx.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-19 14:38:38.639425 ForestScience-0.0.9/ForestScience.egg-info/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1415 2023-07-19 14:38:38.000000 ForestScience-0.0.9/ForestScience.egg-info/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      399 2023-07-19 14:38:38.000000 ForestScience-0.0.9/ForestScience.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-19 14:38:38.000000 ForestScience-0.0.9/ForestScience.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       48 2023-07-19 14:38:38.000000 ForestScience-0.0.9/ForestScience.egg-info/entry_points.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-13 22:01:51.000000 ForestScience-0.0.9/ForestScience.egg-info/not-zip-safe
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-19 14:38:38.000000 ForestScience-0.0.9/ForestScience.egg-info/requires.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       14 2023-07-19 14:38:38.000000 ForestScience-0.0.9/ForestScience.egg-info/top_level.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11357 2023-07-13 21:42:44.000000 ForestScience-0.0.9/LICENSE
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestScience-0.0.9/MANIFEST.in
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1415 2023-07-19 14:38:38.663426 ForestScience-0.0.9/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      620 2023-07-13 22:06:55.000000 ForestScience-0.0.9/README.md
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      924 2023-07-19 14:37:54.000000 ForestScience-0.0.9/settings.ini
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-19 14:38:38.667426 ForestScience-0.0.9/setup.cfg
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestScience-0.0.9/setup.py
```

### Comparing `ForestScience-0.0.8/ForestScience/InventarioFlorestal.py` & `ForestScience-0.0.9/ForestScience/InventarioFlorestal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_InventarioFlorestal.ipynb.
-
-# %% auto 0
-__all__ = ['InventarioFlorestal']
-
-# %% ../nbs/00_InventarioFlorestal.ipynb 3
-class InventarioFlorestal:
-    
-    'Cálculo das estatitísticas de inventário amostragem casual simples e extratificada'
-    
-    def __tratativa_tabelas(dados, parcela, dap, ht, estrato = None,
-                     id_arvore = None, volume = None, equacao_volume = None):
-
-        dicionario = {'renomear_colunas':{estrato : 'estrato',parcela: 'parcela', id_arvore: 'n_arvores',
-                                             dap: 'dap', ht : 'ht'},
-                     'colunas_agrupar': {'ACS':'parcela','AE':['estrato','parcela']},
-                     'metodo_agregacao':{'com_arvore':{'volume': np.sum,'gi': np.sum,'n_arvores': lambda x: len(set(x))},
-                                         'sem_arvore':{'volume': np.sum,'gi': np.sum,'dap': lambda x: len(x)}}}
-        
-        # verificacoes iniciais
-        if (equacao_volume is not None) and (isinstance(equacao_volume, types.FunctionType) == False):
-            
-            raise TypeError("O parâmetro 'equacao_volume' deve ser uma função.")
-        
-        # salvando dataframe apenas com colunas que serão usadas
-        colunas = [estrato,parcela,id_arvore,dap,ht]
-
-        dados_tratado = dados[[x for x in colunas if x is not None]].copy()
-
-        # renomeando as colunas do dataframe
-        dados_tratado.rename(columns = dicionario['renomear_colunas'], inplace=True)
-
-        # criando coluna com área basal
-        dados_tratado['gi'] = (dados_tratado['dap']**2*np.pi)/40000
-
-        # verificando se há coluna de volume
-        if volume is None:
-
-            dados_tratado['volume'] = equacao_volume(dados_tratado)
-
-        else:
-            
-            dados_tratado['volume'] = dados[volume].copy()
-
-        # salvando colunas que serão agrupadas e dicionário com metódo de agregação
-        col_agrupar = dicionario['colunas_agrupar']['ACS'] if estrato is None else dicionario['colunas_agrupar']['AE']
-        metodo_agregacao = dicionario['metodo_agregacao']['sem_arvore'] if id_arvore is None else dicionario['metodo_agregacao']['com_arvore']
-
-        # criando tabela dinamica por parcela, soma de volume, soma de área basal e número de árvores
-        dados_pivotado = pd.DataFrame(dados_tratado.pivot_table(index=col_agrupar,aggfunc = metodo_agregacao))
-        dados_pivotado.reset_index(inplace = True)
-        dados_pivotado.rename(columns = {'dap': 'n_arvores'}, inplace = True)
-
-        return {'tabela_dados': dados_tratado, 'tabela_parcelas': dados_pivotado}
-
-    def __estatisticas(self):
-        
-        if 'estrato' in self.tabela_dados.columns:
-            
-            # Calculando número de estratos
-            n_estratos = len(self.tabela_parcelas['estrato'].unique())
-            
-            if n_estratos != len(self.__area_estratos):
-                
-                raise SyntaxError("O número de estratos no parâmetro area_estratos é diferente do número de estratos na tabela.")
-
-            area_total = sum([self.__area_estratos[k] for k in self.__area_estratos])
-
-            calc_estrato = {str(k): {} for k in self.__area_estratos}
-
-            for k, v in self.__area_estratos.items():
-                
-                calc_estrato[str(k)]['area'] = v
-                calc_estrato[str(k)]['Wh'] = v/area_total
-                calc_estrato[str(k)]['Nh'] = (v*10000)/self.__area_parcela
-                calc_estrato[str(k)]['nh'] = len(self.tabela_parcelas['estrato'][self.tabela_parcelas['estrato'].astype(str) == str(k)])
-                calc_estrato[str(k)]['Xh'] = np.mean(self.tabela_parcelas['volume'][self.tabela_parcelas['estrato'].astype(str) == str(k)])
-                calc_estrato[str(k)]['sh'] = np.std(self.tabela_parcelas['volume'][self.tabela_parcelas['estrato'].astype(str) == str(k)],ddof = 1)**2
-            
-            Wh = np.array([calc_estrato[x]['Wh'] for x in calc_estrato.keys()])
-            Nh = np.array([calc_estrato[x]['Nh'] for x in calc_estrato.keys()])
-            nh = np.array([calc_estrato[x]['nh'] for x in calc_estrato.keys()])
-            Xh = np.array([calc_estrato[x]['Xh'] for x in calc_estrato.keys()])
-            sh = np.array([calc_estrato[x]['sh'] for x in calc_estrato.keys()])
-                
-            # calculando intensidade amostral
-            ia = (self.__area_parcela*sum(nh))/(area_total*10000)*100
-
-            # calculando média estratificada
-            media_estratificada =  sum(np.array(Wh)*np.array(Xh))
-
-            # calculando média da variancia estratificada
-
-            # população finita
-            if ia >= 2:
-                sy_estratificada = sum(((Wh**2*sh)/nh)*(1-(nh/Nh)))
-    
-            # população infinita
-            else:
-                sy_estratificada = sum((Wh**2*sh)/nh)
-                        
-            # calculando valor T
-            t = scipy.stats.t.ppf(q=1-((1-self.__p)/2),df=(sum(nh)-1))
-
-            # calculando erro relativo e absoluto
-
-            ea = t * sy_estratificada**(1/2)
-            er = ea/media_estratificada*100
-
-            id_estratos = list(self.tabela_parcelas['estrato'].unique())
-
-            # calculando fator
-            f = 10000/self.__area_parcela
-            
-            resultado_estrato = {'Estrato': [], 'Área (ha)': [], 'Volume/parcela (m³)': [],
-                                 'Volume/ha (m³)': [], 'Volume total (m³)': []}
-            
-            for i in np.sort(list(calc_estrato.keys())):
-                
-                resultado_estrato['Estrato'].append(i)
-                resultado_estrato['Área (ha)'].append(calc_estrato[i]['area'])
-                resultado_estrato['Volume/parcela (m³)'].append(calc_estrato[i]['Xh'])
-                resultado_estrato['Volume/ha (m³)'].append(calc_estrato[i]['Xh']*f)
-                resultado_estrato['Volume total (m³)'].append(calc_estrato[i]['Xh']*f*calc_estrato[i]['area'])
-                            
-            resultado_geral = {'Parâmetros': ['Àrea total','Parcelas alocadas','Parcelas cabíveis',
-                                              'Intensidade amostral','Volume total de madeira', 'Desvio Padrão',
-                                              'Variância da média','Erro absoluto', 'Erro relativo', 'IC por parcela',
-                                              'IC por hectare','IC total', 'Valor de t tabelado'],
-                               'Unidade': ['hectare','-','-','%','m³','m³','(m³)²','m³','%','m³','m³','m³','-'],
-                               'Resultados': [area_total, sum(nh), sum(Nh), ia, media_estratificada*f*area_total,
-                                             sy_estratificada**(1/2), sy_estratificada, ea, er, 
-                                             f'{media_estratificada:.2f} ± {ea:.2f}',
-                                             f'{media_estratificada*f:.2f} ± {ea*f:.2f}',
-                                             f'{media_estratificada*f*area_total:.2f} ± {ea*f*area_total:.2f}',
-                                                t]}
-            
-            return resultado_estrato, resultado_geral
-        
-        else:
-            
-            # calculado número de parcelas
-            n_parcelas = len(self.tabela_parcelas['parcela'])
-
-            # calculando área amostral, desvio padrão, média e coeficiente de variação
-            area_amostral = (n_parcelas*self.__area_parcela)/10000
-            desvio = np.std(self.tabela_parcelas.eval(self.tabela_parcelas['volume']),ddof=1)
-            media = np.mean(self.tabela_parcelas.eval(self.tabela_parcelas['volume']))
-            CV = desvio/media*100
-                        
-            # calculando intensidade amostral
-            ia = area_amostral/self.__area_total*100
-
-            # fator
-            f = 10000/self.__area_parcela
-
-            # população finita
-            if ia >= 2:
-                sy = np.sqrt(((desvio**2)/n_parcelas)*(1-(ia/100)))
-            
-            # população infinita
-            else:
-                sy = np.sqrt((desvio**2)/n_parcelas)
-
-            # calculando o valor T
-            t = scipy.stats.t.ppf(q=1-((1-self.__p)/2),df=(n_parcelas-1))
-            
-            # calculando erro absoluto e erro relativo
-            ea = (sy*t)
-            er = ((sy*t)/media)*100
-
-            resultado_geral = {'Parâmetros': ['Àrea total','Parcelas alocadas','Parcelas cabíveis',
-                                  'Intensidade amostral','Volume total de madeira', 'Desvio Padrão',
-                                  'Variância da média','Erro absoluto', 'Erro relativo', 'IC por parcela',
-                                  'IC por hectare','IC total', 'Valor de t tabelado'],
-                   'Unidade': ['hectare','-','-','%','m³','m³','(m³)²','m³','%','m³','m³','m³','-'],
-                   'Resultados': [self.__area_total, n_parcelas, round(self.__area_total/(self.__area_parcela/10000),2),
-                                  round(ia,2), media*f*self.__area_total,
-                                  desvio, desvio**2, ea, er, 
-                                 f'{media:.2f} ± {ea:.2f}',
-                                 f'{media*f:.2f} ± {ea*f:.2f}',
-                                 f'{media*f*self.__area_total:.2f} ± {ea*f*self.__area_total:.2f}',
-                                    t]}
-
-            return resultado_geral
-        
-    # função para gerar o gráfico de distribuição diâmetrica
-    def __grafico(coluna_dap, titulo, DAP_min, DAP_max, amplitude_classe, save = False):
-               
-        n_fustes = len(coluna_dap)
-        plt.figure(figsize=(6, 4))
-        plt.hist(coluna_dap, histtype='bar', stacked=False, fill=False, bins = np.arange(DAP_min,DAP_max,amplitude_classe))
-        plt.title(titulo)
-        plt.xlabel("Classe diâmetrica")
-        plt.ylabel("Número de fustes")
-        plt.xticks(np.arange(DAP_min + amplitude_classe/2,DAP_max - amplitude_classe/2,
-                             amplitude_classe))
-        plt.text(0.62, 0.91,f"Número de fustes: {n_fustes}",transform=plt.gca().transAxes,
-                bbox=dict(facecolor='white', edgecolor='black',boxstyle='round'))
-
-        if save == True:
-
-            nome = 'distribuicao_diametrica'
-            nome_arquivo = nome if titulo == 'Distribuição diâmetrica' else f'{nome}_{titulo[33:]}'
-            plt.savefig(f'{nome_arquivo}.png', dpi = 300)
-            plt.close()
-
-        else:
-
-            plt.show()
-
-    def __init__(self, 
-                 dados, # tabela com as informações das árvores
-                 parcela:str, # nome da coluna com identificação das parcelas
-                 dap:str, # nome da coluna com o diamêtro a altura do peito em cm
-                 area_parcela:float, # área de cada parcela
-                 ht:str = None, # nome da coluna com o diamêtro a altura do peito em m
-                 estrato:str = None, # nome da coluna com identificação dos estratos
-                 area_total: float = None, # área total em ha
-                 area_estratos: dict = None, # dicionário com identificacao do extrato e área em ha
-                 id_arvore:str = None, # nome da coluna identificação as árvores
-                 p:float = 0.95, # significância [0, 1]
-                 volume: float = None, # nome da coluna com volume em m³
-                 equacao_volume = None # função que cálcula o volume de madeira em m³
-                ):
-        tabelas = InventarioFlorestal._InventarioFlorestal__tratativa_tabelas(dados = dados, parcela = parcela, dap = dap, ht = ht,
-                                                            estrato = estrato, id_arvore = id_arvore,
-                                                            volume = volume, equacao_volume = equacao_volume)
-
-        self.tabela_dados = tabelas['tabela_dados']
-        self.tabela_parcelas = tabelas['tabela_parcelas']
-        
-        # salvando informações
-        self.__area_total = area_total
-        self.__area_estratos = area_estratos
-        self.__area_parcela = area_parcela
-        self.__p = p
-        
-        resultados = InventarioFlorestal._InventarioFlorestal__estatisticas(self)
-        
-        if area_estratos is not None:
-            
-            self.resultados_estratos = pd.DataFrame(resultados[0]).round(2)
-            self.resultados = pd.DataFrame(resultados[1]).round(2)
-            
-        else:
-            
-            self.resultados = pd.DataFrame(resultados).round(2)
-            
-    def distribuicao_diametrica(self, save = False):
-
-        # calculando dap min e max
-        DAP_min = np.floor(np.min(self.tabela_dados['dap']))
-        DAP_max = np.ceil(np.max(self.tabela_dados['dap']))
-
-        # calculando a amplitude de classe ideal para os dados
-        possiveis_ampli_classe = []
-        for i in np.arange(2,20,0.5):
-            
-            comprimento = len(list(np.arange(DAP_min,DAP_max,i)))
-            
-            if comprimento <= 7 and comprimento >= 5:
-                possiveis_ampli_classe.append(i)
-        
-        amplitude_classe = np.min(possiveis_ampli_classe)
-                
-        # gerando gráfico para área totoal
-        InventarioFlorestal._InventarioFlorestal__grafico(self.tabela_dados['dap'], 'Distribuição diâmetrica',
-                                                          DAP_min, DAP_max, amplitude_classe, save)
-
-        # gerando gráfico por estratos caso seja amostragem estratificada
-        if 'estrato' in self.tabela_dados.columns:
-
-            for estrato in np.sort(list(self.tabela_parcelas['estrato'].unique())):
-
-                coluna_filtrada = self.tabela_dados['dap'][self.tabela_dados['estrato'] == estrato]
-                InventarioFlorestal._InventarioFlorestal__grafico(coluna_filtrada,
-                                                                 f'Distribuição diâmetrica estrato: {estrato}',
-                                                                  DAP_min, DAP_max, amplitude_classe, save)                      
-    def salvar_resultados(self):
-        
-        if self.__area_estratos is not None:
-            
-            pd.DataFrame(self.resultados_estratos).round(2).to_csv('estatisticas_inventario.csv',
-                                                             encoding='utf-8-sig', index= False, sep = ';')
-            pd.DataFrame(self.resultados).round(2).to_csv('estatisticas_estrato.csv',
-                                                               encoding='utf-8-sig', index= False, sep = ';')
-            
-        else:
-            
-            pd.DataFrame(self.resultados).round(2).to_csv('estatisticas_inventario.csv',
-                                                          encoding='utf-8-sig', index= False, sep = ';')
-            
-        InventarioFlorestal.distribuicao_diametrica(self, True)
-        
-        print('Arquivos salvos com sucesso.')
-
-# %% ../nbs/00_InventarioFlorestal.ipynb 4
-from .InventarioFlorestal import *
-import pandas as pd
-import numpy as np
-import scipy.stats
-import matplotlib.pyplot as plt
-import types
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_InventarioFlorestal.ipynb.
+
+# %% auto 0
+__all__ = ['InventarioFlorestal']
+
+# %% ../nbs/00_InventarioFlorestal.ipynb 3
+class InventarioFlorestal:
+    
+    'Cálculo das estatitísticas de inventário amostragem casual simples e extratificada'
+    
+    def __tratativa_tabelas(dados, parcela, dap, ht, estrato = None,
+                     id_arvore = None, volume = None, equacao_volume = None):
+
+        dicionario = {'renomear_colunas':{estrato : 'estrato',parcela: 'parcela', id_arvore: 'n_arvores',
+                                             dap: 'dap', ht : 'ht'},
+                     'colunas_agrupar': {'ACS':'parcela','AE':['estrato','parcela']},
+                     'metodo_agregacao':{'com_arvore':{'volume': np.sum,'gi': np.sum,'n_arvores': lambda x: len(set(x))},
+                                         'sem_arvore':{'volume': np.sum,'gi': np.sum,'dap': lambda x: len(x)}}}
+        
+        # verificacoes iniciais
+        if (equacao_volume is not None) and (isinstance(equacao_volume, types.FunctionType) == False):
+            
+            raise TypeError("O parâmetro 'equacao_volume' deve ser uma função.")
+        
+        # salvando dataframe apenas com colunas que serão usadas
+        colunas = [estrato,parcela,id_arvore,dap,ht]
+
+        dados_tratado = dados[[x for x in colunas if x is not None]].copy()
+
+        # renomeando as colunas do dataframe
+        dados_tratado.rename(columns = dicionario['renomear_colunas'], inplace=True)
+
+        # criando coluna com área basal
+        dados_tratado['gi'] = (dados_tratado['dap']**2*np.pi)/40000
+
+        # verificando se há coluna de volume
+        if volume is None:
+
+            dados_tratado['volume'] = equacao_volume(dados_tratado)
+
+        else:
+            
+            dados_tratado['volume'] = dados[volume].copy()
+
+        # salvando colunas que serão agrupadas e dicionário com metódo de agregação
+        col_agrupar = dicionario['colunas_agrupar']['ACS'] if estrato is None else dicionario['colunas_agrupar']['AE']
+        metodo_agregacao = dicionario['metodo_agregacao']['sem_arvore'] if id_arvore is None else dicionario['metodo_agregacao']['com_arvore']
+
+        # criando tabela dinamica por parcela, soma de volume, soma de área basal e número de árvores
+        dados_pivotado = pd.DataFrame(dados_tratado.pivot_table(index=col_agrupar,aggfunc = metodo_agregacao))
+        dados_pivotado.reset_index(inplace = True)
+        dados_pivotado.rename(columns = {'dap': 'n_arvores'}, inplace = True)
+
+        return {'tabela_dados': dados_tratado, 'tabela_parcelas': dados_pivotado}
+
+    def __estatisticas(self):
+        
+        if 'estrato' in self.tabela_dados.columns:
+            
+            # Calculando número de estratos
+            n_estratos = len(self.tabela_parcelas['estrato'].unique())
+            
+            if n_estratos != len(self.__area_estratos):
+                
+                raise SyntaxError("O número de estratos no parâmetro area_estratos é diferente do número de estratos na tabela.")
+
+            area_total = sum([self.__area_estratos[k] for k in self.__area_estratos])
+
+            calc_estrato = {str(k): {} for k in self.__area_estratos}
+
+            for k, v in self.__area_estratos.items():
+                
+                calc_estrato[str(k)]['area'] = v
+                calc_estrato[str(k)]['Wh'] = v/area_total
+                calc_estrato[str(k)]['Nh'] = (v*10000)/self.__area_parcela
+                calc_estrato[str(k)]['nh'] = len(self.tabela_parcelas['estrato'][self.tabela_parcelas['estrato'].astype(str) == str(k)])
+                calc_estrato[str(k)]['Xh'] = np.mean(self.tabela_parcelas['volume'][self.tabela_parcelas['estrato'].astype(str) == str(k)])
+                calc_estrato[str(k)]['sh'] = np.std(self.tabela_parcelas['volume'][self.tabela_parcelas['estrato'].astype(str) == str(k)],ddof = 1)**2
+            
+            Wh = np.array([calc_estrato[x]['Wh'] for x in calc_estrato.keys()])
+            Nh = np.array([calc_estrato[x]['Nh'] for x in calc_estrato.keys()])
+            nh = np.array([calc_estrato[x]['nh'] for x in calc_estrato.keys()])
+            Xh = np.array([calc_estrato[x]['Xh'] for x in calc_estrato.keys()])
+            sh = np.array([calc_estrato[x]['sh'] for x in calc_estrato.keys()])
+                
+            # calculando intensidade amostral
+            ia = (self.__area_parcela*sum(nh))/(area_total*10000)*100
+
+            # calculando média estratificada
+            media_estratificada =  sum(np.array(Wh)*np.array(Xh))
+
+            # calculando média da variancia estratificada
+
+            # população finita
+            if ia >= 2:
+                sy_estratificada = sum(((Wh**2*sh)/nh)*(1-(nh/Nh)))
+    
+            # população infinita
+            else:
+                sy_estratificada = sum((Wh**2*sh)/nh)
+                        
+            # calculando valor T
+            t = scipy.stats.t.ppf(q=1-((1-self.__p)/2),df=(sum(nh)-1))
+
+            # calculando erro relativo e absoluto
+
+            ea = t * sy_estratificada**(1/2)
+            er = ea/media_estratificada*100
+
+            id_estratos = list(self.tabela_parcelas['estrato'].unique())
+
+            # calculando fator
+            f = 10000/self.__area_parcela
+            
+            resultado_estrato = {'Estrato': [], 'Área (ha)': [], 'Volume/parcela (m³)': [],
+                                 'Volume/ha (m³)': [], 'Volume total (m³)': []}
+            
+            for i in np.sort(list(calc_estrato.keys())):
+                
+                resultado_estrato['Estrato'].append(i)
+                resultado_estrato['Área (ha)'].append(calc_estrato[i]['area'])
+                resultado_estrato['Volume/parcela (m³)'].append(calc_estrato[i]['Xh'])
+                resultado_estrato['Volume/ha (m³)'].append(calc_estrato[i]['Xh']*f)
+                resultado_estrato['Volume total (m³)'].append(calc_estrato[i]['Xh']*f*calc_estrato[i]['area'])
+                            
+            resultado_geral = {'Parâmetros': ['Àrea total','Parcelas alocadas','Parcelas cabíveis',
+                                              'Intensidade amostral','Volume total de madeira', 'Desvio Padrão',
+                                              'Variância da média','Erro absoluto', 'Erro relativo', 'IC por parcela',
+                                              'IC por hectare','IC total', 'Valor de t tabelado'],
+                               'Unidade': ['hectare','-','-','%','m³','m³','(m³)²','m³','%','m³','m³','m³','-'],
+                               'Resultados': [area_total, sum(nh), sum(Nh), ia, media_estratificada*f*area_total,
+                                             sy_estratificada**(1/2), sy_estratificada, ea, er, 
+                                             f'{media_estratificada:.2f} ± {ea:.2f}',
+                                             f'{media_estratificada*f:.2f} ± {ea*f:.2f}',
+                                             f'{media_estratificada*f*area_total:.2f} ± {ea*f*area_total:.2f}',
+                                                t]}
+            
+            return resultado_estrato, resultado_geral
+        
+        else:
+            
+            # calculado número de parcelas
+            n_parcelas = len(self.tabela_parcelas['parcela'])
+
+            # calculando área amostral, desvio padrão, média e coeficiente de variação
+            area_amostral = (n_parcelas*self.__area_parcela)/10000
+            desvio = np.std(self.tabela_parcelas.eval(self.tabela_parcelas['volume']),ddof=1)
+            media = np.mean(self.tabela_parcelas.eval(self.tabela_parcelas['volume']))
+            CV = desvio/media*100
+                        
+            # calculando intensidade amostral
+            ia = area_amostral/self.__area_total*100
+
+            # fator
+            f = 10000/self.__area_parcela
+
+            # população finita
+            if ia >= 2:
+                sy = np.sqrt(((desvio**2)/n_parcelas)*(1-(ia/100)))
+            
+            # população infinita
+            else:
+                sy = np.sqrt((desvio**2)/n_parcelas)
+
+            # calculando o valor T
+            t = scipy.stats.t.ppf(q=1-((1-self.__p)/2),df=(n_parcelas-1))
+            
+            # calculando erro absoluto e erro relativo
+            ea = (sy*t)
+            er = ((sy*t)/media)*100
+
+            resultado_geral = {'Parâmetros': ['Àrea total','Parcelas alocadas','Parcelas cabíveis',
+                                  'Intensidade amostral','Volume total de madeira', 'Desvio Padrão',
+                                  'Variância da média','Erro absoluto', 'Erro relativo', 'IC por parcela',
+                                  'IC por hectare','IC total', 'Valor de t tabelado'],
+                   'Unidade': ['hectare','-','-','%','m³','m³','(m³)²','m³','%','m³','m³','m³','-'],
+                   'Resultados': [self.__area_total, n_parcelas, round(self.__area_total/(self.__area_parcela/10000),2),
+                                  round(ia,2), media*f*self.__area_total,
+                                  desvio, desvio**2, ea, er, 
+                                 f'{media:.2f} ± {ea:.2f}',
+                                 f'{media*f:.2f} ± {ea*f:.2f}',
+                                 f'{media*f*self.__area_total:.2f} ± {ea*f*self.__area_total:.2f}',
+                                    t]}
+
+            return resultado_geral
+        
+    # função para gerar o gráfico de distribuição diâmetrica
+    def __grafico(coluna_dap, titulo, DAP_min, DAP_max, amplitude_classe, save = False):
+               
+        n_fustes = len(coluna_dap)
+        plt.figure(figsize=(6, 4))
+        plt.hist(coluna_dap, histtype='bar', stacked=False, fill=False, bins = np.arange(DAP_min,DAP_max,amplitude_classe))
+        plt.title(titulo)
+        plt.xlabel("Classe diâmetrica")
+        plt.ylabel("Número de fustes")
+        plt.xticks(np.arange(DAP_min + amplitude_classe/2,DAP_max - amplitude_classe/2,
+                             amplitude_classe))
+        plt.text(0.62, 0.91,f"Número de fustes: {n_fustes}",transform=plt.gca().transAxes,
+                bbox=dict(facecolor='white', edgecolor='black',boxstyle='round'))
+
+        if save == True:
+
+            nome = 'distribuicao_diametrica'
+            nome_arquivo = nome if titulo == 'Distribuição diâmetrica' else f'{nome}_{titulo[33:]}'
+            plt.savefig(f'{nome_arquivo}.png', dpi = 300)
+            plt.close()
+
+        else:
+
+            plt.show()
+
+    def __init__(self, 
+                 dados, # tabela com as informações das árvores
+                 parcela:str, # nome da coluna com identificação das parcelas
+                 dap:str, # nome da coluna com o diamêtro a altura do peito em cm
+                 area_parcela:float, # área de cada parcela
+                 ht:str = None, # nome da coluna com o diamêtro a altura do peito em m
+                 estrato:str = None, # nome da coluna com identificação dos estratos
+                 area_total: float = None, # área total em ha
+                 area_estratos: dict = None, # dicionário com identificacao do extrato e área em ha
+                 id_arvore:str = None, # nome da coluna identificação as árvores
+                 p:float = 0.95, # significância [0, 1]
+                 volume: float = None, # nome da coluna com volume em m³
+                 equacao_volume = None # função que cálcula o volume de madeira em m³
+                ):
+        tabelas = InventarioFlorestal._InventarioFlorestal__tratativa_tabelas(dados = dados, parcela = parcela, dap = dap, ht = ht,
+                                                            estrato = estrato, id_arvore = id_arvore,
+                                                            volume = volume, equacao_volume = equacao_volume)
+
+        self.tabela_dados = tabelas['tabela_dados']
+        self.tabela_parcelas = tabelas['tabela_parcelas']
+        
+        # salvando informações
+        self.__area_total = area_total
+        self.__area_estratos = area_estratos
+        self.__area_parcela = area_parcela
+        self.__p = p
+        
+        resultados = InventarioFlorestal._InventarioFlorestal__estatisticas(self)
+        
+        if area_estratos is not None:
+            
+            self.resultados_estratos = pd.DataFrame(resultados[0]).round(2)
+            self.resultados = pd.DataFrame(resultados[1]).round(2)
+            
+        else:
+            
+            self.resultados = pd.DataFrame(resultados).round(2)
+            
+    def distribuicao_diametrica(self, save = False):
+
+        # calculando dap min e max
+        DAP_min = np.floor(np.min(self.tabela_dados['dap']))
+        DAP_max = np.ceil(np.max(self.tabela_dados['dap']))
+
+        # calculando a amplitude de classe ideal para os dados
+        possiveis_ampli_classe = []
+        for i in np.arange(2,20,0.5):
+            
+            comprimento = len(list(np.arange(DAP_min,DAP_max,i)))
+            
+            if comprimento <= 7 and comprimento >= 5:
+                possiveis_ampli_classe.append(i)
+        
+        amplitude_classe = np.min(possiveis_ampli_classe)
+                
+        # gerando gráfico para área totoal
+        InventarioFlorestal._InventarioFlorestal__grafico(self.tabela_dados['dap'], 'Distribuição diâmetrica',
+                                                          DAP_min, DAP_max, amplitude_classe, save)
+
+        # gerando gráfico por estratos caso seja amostragem estratificada
+        if 'estrato' in self.tabela_dados.columns:
+
+            for estrato in np.sort(list(self.tabela_parcelas['estrato'].unique())):
+
+                coluna_filtrada = self.tabela_dados['dap'][self.tabela_dados['estrato'] == estrato]
+                InventarioFlorestal._InventarioFlorestal__grafico(coluna_filtrada,
+                                                                 f'Distribuição diâmetrica estrato: {estrato}',
+                                                                  DAP_min, DAP_max, amplitude_classe, save)                      
+    def salvar_resultados(self):
+        
+        if self.__area_estratos is not None:
+            
+            pd.DataFrame(self.resultados_estratos).round(2).to_csv('estatisticas_estrato.csv',
+                                                             encoding='utf-8-sig', index= False, sep = ';')
+            pd.DataFrame(self.resultados).round(2).to_csv('estatisticas_inventario.csv',
+                                                               encoding='utf-8-sig', index= False, sep = ';')
+            
+        else:
+            
+            pd.DataFrame(self.resultados).round(2).to_csv('estatisticas_inventario.csv',
+                                                          encoding='utf-8-sig', index= False, sep = ';')
+            
+        InventarioFlorestal.distribuicao_diametrica(self, True)
+        
+        print('Arquivos salvos com sucesso.')
+
+# %% ../nbs/00_InventarioFlorestal.ipynb 4
+#from ForestScience.InventarioFlorestal import *
+import pandas as pd
+import numpy as np
+import scipy.stats
+import matplotlib.pyplot as plt
+import types
```

### Comparing `ForestScience-0.0.8/ForestScience/_modidx.py` & `ForestScience-0.0.9/ForestScience/_modidx.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Autogenerated by nbdev
-
-d = { 'settings': { 'branch': 'main',
-                'doc_baseurl': '/ForestScience',
-                'doc_host': 'https://gabrielfbueno.github.io',
-                'git_url': 'https://github.com/gabrielfbueno/ForestScience',
-                'lib_path': 'ForestScience'},
-  'syms': { 'ForestScience.InventarioFlorestal': { 'ForestScience.InventarioFlorestal.InventarioFlorestal': ( 'inventarioflorestal.html#inventarioflorestal',
-                                                                                                              'ForestScience/InventarioFlorestal.py'),
-                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__estatisticas': ( 'inventarioflorestal.html#inventarioflorestal.__estatisticas',
-                                                                                                                             'ForestScience/InventarioFlorestal.py'),
-                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__grafico': ( 'inventarioflorestal.html#inventarioflorestal.__grafico',
-                                                                                                                        'ForestScience/InventarioFlorestal.py'),
-                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__init__': ( 'inventarioflorestal.html#inventarioflorestal.__init__',
-                                                                                                                       'ForestScience/InventarioFlorestal.py'),
-                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__tratativa_tabelas': ( 'inventarioflorestal.html#inventarioflorestal.__tratativa_tabelas',
-                                                                                                                                  'ForestScience/InventarioFlorestal.py'),
-                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.distribuicao_diametrica': ( 'inventarioflorestal.html#inventarioflorestal.distribuicao_diametrica',
-                                                                                                                                      'ForestScience/InventarioFlorestal.py'),
-                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.salvar_resultados': ( 'inventarioflorestal.html#inventarioflorestal.salvar_resultados',
-                                                                                                                                'ForestScience/InventarioFlorestal.py')}}}
+# Autogenerated by nbdev
+
+d = { 'settings': { 'branch': 'main',
+                'doc_baseurl': '/ForestScience',
+                'doc_host': 'https://gabrielfbueno.github.io',
+                'git_url': 'https://github.com/gabrielfbueno/ForestScience',
+                'lib_path': 'ForestScience'},
+  'syms': { 'ForestScience.InventarioFlorestal': { 'ForestScience.InventarioFlorestal.InventarioFlorestal': ( 'inventarioflorestal.html#inventarioflorestal',
+                                                                                                              'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__estatisticas': ( 'inventarioflorestal.html#inventarioflorestal.__estatisticas',
+                                                                                                                             'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__grafico': ( 'inventarioflorestal.html#inventarioflorestal.__grafico',
+                                                                                                                        'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__init__': ( 'inventarioflorestal.html#inventarioflorestal.__init__',
+                                                                                                                       'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.__tratativa_tabelas': ( 'inventarioflorestal.html#inventarioflorestal.__tratativa_tabelas',
+                                                                                                                                  'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.distribuicao_diametrica': ( 'inventarioflorestal.html#inventarioflorestal.distribuicao_diametrica',
+                                                                                                                                      'ForestScience/InventarioFlorestal.py'),
+                                                   'ForestScience.InventarioFlorestal.InventarioFlorestal.salvar_resultados': ( 'inventarioflorestal.html#inventarioflorestal.salvar_resultados',
+                                                                                                                                'ForestScience/InventarioFlorestal.py')}}}
```

### Comparing `ForestScience-0.0.8/ForestScience.egg-info/PKG-INFO` & `ForestScience-0.0.9/ForestScience.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestScience
-Version: 0.0.8
+Version: 0.0.9
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestScience
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: Engenharia Florestal Inventario python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ForestScience-0.0.8/LICENSE` & `ForestScience-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.8/PKG-INFO` & `ForestScience-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestScience
-Version: 0.0.8
+Version: 0.0.9
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestScience
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: Engenharia Florestal Inventario python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ForestScience-0.0.8/README.md` & `ForestScience-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ForestScience-0.0.8/settings.ini` & `ForestScience-0.0.9/settings.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[DEFAULT]
-repo = ForestScience
-lib_name = ForestScience
-version = 0.0.8
-min_python = 3.7
-license = apache2
-black_formatting = False
-doc_path = _docs
-lib_path = ForestScience
-nbs_path = nbs
-recursive = True
-tst_flags = notest
-put_version_in_init = True
-branch = main
-custom_sidebar = False
-doc_host = https://gabrielfbueno.github.io
-doc_baseurl = /ForestScience
-git_url = https://github.com/gabrielfbueno/ForestScience
-title = ForestScience
-audience = Developers
-author = gabrielfbueno
-author_email = gabrielfbueno@outlook.com
-copyright = 2023 onwards, gabrielfbueno
-description = A biblioteca Florestal
-keywords = Engenharia Florestal Inventario python
-language = Portuguese
-status = 3
-user = gabrielfbueno
-requirements = pandas numpy scipy matplotlib
-readme_nb = index.ipynb
-allowed_metadata_keys = 
-allowed_cell_metadata_keys = 
-jupyter_hooks = True
-clean_ids = True
-clear_all = False
-
+[DEFAULT]
+repo = ForestScience
+lib_name = ForestScience
+version = 0.0.9
+min_python = 3.7
+license = apache2
+black_formatting = False
+doc_path = _docs
+lib_path = ForestScience
+nbs_path = nbs
+recursive = True
+tst_flags = notest
+put_version_in_init = True
+branch = main
+custom_sidebar = False
+doc_host = https://gabrielfbueno.github.io
+doc_baseurl = /ForestScience
+git_url = https://github.com/gabrielfbueno/ForestScience
+title = ForestScience
+audience = Developers
+author = gabrielfbueno
+author_email = gabrielfbueno@outlook.com
+copyright = 2023 onwards, gabrielfbueno
+description = A biblioteca Florestal
+keywords = Engenharia Florestal Inventario python
+language = Portuguese
+status = 3
+user = gabrielfbueno
+requirements = pandas numpy scipy matplotlib
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `ForestScience-0.0.8/setup.py` & `ForestScience-0.0.9/setup.py`

 * *Files identical despite different names*

