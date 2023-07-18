# Comparing `tmp/escavador-0.3.0.tar.gz` & `tmp/escavador-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escavador-0.3.0.tar", max compression
+gzip compressed data, was "escavador-0.4.0.tar", max compression
```

## Comparing `escavador-0.3.0.tar` & `escavador-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1065 2023-06-14 23:04:22.198392 escavador-0.3.0/LICENSE
--rw-r--r--   0        0        0     8408 2023-06-14 23:04:22.198392 escavador-0.3.0/README.md
--rw-r--r--   0        0        0      724 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/__init__.py
--rw-r--r--   0        0        0     3180 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/api.py
--rw-r--r--   0        0        0     1444 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/exceptions.py
--rw-r--r--   0        0        0     3037 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/method.py
--rw-r--r--   0        0        0      503 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/__init__.py
--rw-r--r--   0        0        0     1379 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/consume_cursor.py
--rw-r--r--   0        0        0      774 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/documento.py
--rw-r--r--   0        0        0     1193 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/endpoint.py
--rw-r--r--   0        0        0       47 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/enums.py
--rw-r--r--   0        0        0      721 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/enums_v1.py
--rw-r--r--   0        0        0     2314 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/enums_v2.py
--rw-r--r--   0        0        0     1481 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/resources/helpers/lista_resultados.py
--rw-r--r--   0        0        0      664 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/__init__.py
--rw-r--r--   0        0        0     1131 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/busca.py
--rw-r--r--   0        0        0      657 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/busca_assincrona.py
--rw-r--r--   0        0        0     2074 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/callback.py
--rw-r--r--   0        0        0     1614 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/diario_oficial.py
--rw-r--r--   0        0        0     1668 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/instituicao.py
--rw-r--r--   0        0        0     3352 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/jurisprudencia.py
--rw-r--r--   0        0        0     2473 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/legislacao.py
--rw-r--r--   0        0        0     4325 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/monitoramento_diario.py
--rw-r--r--   0        0        0     2545 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/monitoramento_tribunal.py
--rw-r--r--   0        0        0      464 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/movimentacao.py
--rw-r--r--   0        0        0     1024 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/pessoa.py
--rw-r--r--   0        0        0    10785 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/processo.py
--rw-r--r--   0        0        0      368 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/saldo.py
--rw-r--r--   0        0        0      689 2023-06-14 23:04:22.198392 escavador-0.3.0/escavador/v1/resources/tribunal.py
--rw-r--r--   0        0        0      174 2023-06-14 23:04:22.202393 escavador-0.3.0/escavador/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 23:04:22.202393 escavador-0.3.0/escavador/v2/resources/__init__.py
--rw-r--r--   0        0        0     7149 2023-06-14 23:04:22.202393 escavador-0.3.0/escavador/v2/resources/envolvido.py
--rw-r--r--   0        0        0     4664 2023-06-14 23:04:22.202393 escavador-0.3.0/escavador/v2/resources/movimentacao.py
--rw-r--r--   0        0        0    24070 2023-06-14 23:04:22.202393 escavador-0.3.0/escavador/v2/resources/processo.py
--rw-r--r--   0        0        0      978 2023-06-14 23:04:22.202393 escavador-0.3.0/escavador/v2/resources/tribunal.py
--rw-r--r--   0        0        0      743 2023-06-14 23:04:22.202393 escavador-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9493 1970-01-01 00:00:00.000000 escavador-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 22:25:48.504826 escavador-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8368 2023-07-18 22:25:48.504826 escavador-0.4.0/README.md
+-rw-r--r--   0        0        0      724 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/__init__.py
+-rw-r--r--   0        0        0     3180 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/api.py
+-rw-r--r--   0        0        0     1444 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/exceptions.py
+-rw-r--r--   0        0        0     3037 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/method.py
+-rw-r--r--   0        0        0      503 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/__init__.py
+-rw-r--r--   0        0        0     1588 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/consume_cursor.py
+-rw-r--r--   0        0        0      774 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/documento.py
+-rw-r--r--   0        0        0     1193 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/endpoint.py
+-rw-r--r--   0        0        0       47 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/enums.py
+-rw-r--r--   0        0        0      721 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/enums_v1.py
+-rw-r--r--   0        0        0     2314 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/enums_v2.py
+-rw-r--r--   0        0        0     1481 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/resources/helpers/lista_resultados.py
+-rw-r--r--   0        0        0      664 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/__init__.py
+-rw-r--r--   0        0        0     1137 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/busca.py
+-rw-r--r--   0        0        0      657 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/busca_assincrona.py
+-rw-r--r--   0        0        0     2080 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/callback.py
+-rw-r--r--   0        0        0     1620 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/diario_oficial.py
+-rw-r--r--   0        0        0     1680 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/instituicao.py
+-rw-r--r--   0        0        0     3360 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/jurisprudencia.py
+-rw-r--r--   0        0        0     2479 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/legislacao.py
+-rw-r--r--   0        0        0     4325 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/monitoramento_diario.py
+-rw-r--r--   0        0        0     2545 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/monitoramento_tribunal.py
+-rw-r--r--   0        0        0      464 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/movimentacao.py
+-rw-r--r--   0        0        0     1030 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/pessoa.py
+-rw-r--r--   0        0        0    10809 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/processo.py
+-rw-r--r--   0        0        0      368 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/saldo.py
+-rw-r--r--   0        0        0      689 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v1/resources/tribunal.py
+-rw-r--r--   0        0        0      174 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v2/resources/__init__.py
+-rw-r--r--   0        0        0     7532 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v2/resources/envolvido.py
+-rw-r--r--   0        0        0     4664 2023-07-18 22:25:48.504826 escavador-0.4.0/escavador/v2/resources/movimentacao.py
+-rw-r--r--   0        0        0    24856 2023-07-18 22:25:48.508826 escavador-0.4.0/escavador/v2/resources/processo.py
+-rw-r--r--   0        0        0     2780 2023-07-18 22:25:48.508826 escavador-0.4.0/escavador/v2/resources/tribunal.py
+-rw-r--r--   0        0        0      743 2023-07-18 22:25:48.508826 escavador-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9453 1970-01-01 00:00:00.000000 escavador-0.4.0/PKG-INFO
```

### Comparing `escavador-0.3.0/LICENSE` & `escavador-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/README.md` & `escavador-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -189,10 +189,11 @@
 | Pessoa                | https://api.escavador.com/v1/docs/#pessoas                           |
 | Tribunal              | https://api.escavador.com/v1/docs/#tribunais                         |
 | Saldo                 | https://api.escavador.com/v1/docs/#saldo-da-api                      |
 
 
 #### V2:
 
-| Módulo                | Link API                                                             |
-|-----------------------|----------------------------------------------------------------------|
-| v2.Processo           | https://api.escavador.com/v2/docs/#processos                         |
+| Módulo      | Link API                                     |
+|-------------|----------------------------------------------|
+| v2.Processo | https://api.escavador.com/v2/docs/#processos |
+| v2.Tribunal | https://api.escavador.com/v2/docs/#tribunais |
```

### Comparing `escavador-0.3.0/escavador/__init__.py` & `escavador-0.4.0/escavador/__init__.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/api.py` & `escavador-0.4.0/escavador/api.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/exceptions.py` & `escavador-0.4.0/escavador/exceptions.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/method.py` & `escavador-0.4.0/escavador/method.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/resources/helpers/consume_cursor.py` & `escavador-0.4.0/escavador/resources/helpers/consume_cursor.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,22 @@
     """Instancia os itens de uma resposta a partir de um construtor
 
     :param resposta: a resposta da primeira requisição, onde 'items' é uma lista de dicts (jsons)
     :param constructor: método para construir um objeto da resposta a partir do json
     :param add_cursor: se True, adiciona o cursor da resposta ao objeto instanciado
     :return: uma lista de objetos instanciados
     """
-    items = resposta["resposta"]["items"]
-    cursor_url = resposta["resposta"].get("links", {}).get("next", "")
+    if isinstance(resposta, dict):
+        resposta = resposta["resposta"]
+        items, cursor_url = resposta["items"], resposta.get("links", {}).get("next", "")
+    else:
+        items, cursor_url = resposta, ""
+
     return ListaResultados(
-        [constructor(item, ultimo_cursor=cursor_url) for item in items]
-        if add_cursor
-        else [constructor(item) for item in items]
+        result
+        for result in (
+            [constructor(item, ultimo_cursor=cursor_url) for item in items]
+            if add_cursor and cursor_url
+            else [constructor(item) for item in items]
+        )
+        if result is not None
     )
```

### Comparing `escavador-0.3.0/escavador/resources/helpers/documento.py` & `escavador-0.4.0/escavador/resources/helpers/documento.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/resources/helpers/endpoint.py` & `escavador-0.4.0/escavador/resources/helpers/endpoint.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/resources/helpers/enums_v1.py` & `escavador-0.4.0/escavador/resources/helpers/enums_v1.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/resources/helpers/enums_v2.py` & `escavador-0.4.0/escavador/resources/helpers/enums_v2.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/resources/helpers/lista_resultados.py` & `escavador-0.4.0/escavador/resources/helpers/lista_resultados.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v1/__init__.py` & `escavador-0.4.0/escavador/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v1/resources/busca.py` & `escavador-0.4.0/escavador/v1/resources/busca.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,14 @@
         *i* -- apenas instituições
         *pa* -- apenas patentes
         *d* -- apenas diários oficiais
         *en* -- apenas pessoas e instituições envolvidas em processos)
         :return: Dict
         """
 
-        data = {
+        params = {
             'q': termo,
             'qo': tipo_termo.value,
             'limit': limit,
             'page': page
         }
-        return cls.methods.get("busca", data=data)
+        return cls.methods.get("busca", params=params)
```

### Comparing `escavador-0.3.0/escavador/v1/resources/busca_assincrona.py` & `escavador-0.4.0/escavador/v1/resources/busca_assincrona.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v1/resources/callback.py` & `escavador-0.4.0/escavador/v1/resources/callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,24 +22,24 @@
         :param evento: o evento do callback
         :param data_minima: a data mínima do callback
         :param data_maxima: a data máxima do callback
         :param status: status do callback
         :return: Dict
         """
 
-        data = {
+        params = {
             "data_maxima": data_maxima.strftime("%Y-%m-%d %H:%M:%S") if data_maxima else None,
             "data_minima": data_minima.strftime("%Y-%m-%d %H:%M:%S") if data_minima else None,
             "evento": evento,
             "item_tipo": item_tipo,
             "item_id": item_id,
             "status": status.value
         }
 
-        return cls.methods.get('callbacks', data=data)
+        return cls.methods.get('callbacks', params=params)
 
     @classmethod
     def marcarRecebido(cls, ids: List) -> Dict:
         """
         Marca callbacks como recebidos
         :param ids:lista com ids dos callbacks que serão marcados como recebidos
         :return: Dict
```

### Comparing `escavador-0.3.0/escavador/v1/resources/diario_oficial.py` & `escavador-0.4.0/escavador/v1/resources/diario_oficial.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     def pagina(cls, id_diario: int, *, page: Optional[int] = None) -> Dict:
         """
         Retorna uma página específica do Diário Oficial pelo seu identificador no Escavador.
         :param id_diario: o ID do diario oficial
         :param page: número da página do diário oficial
         :return: Dict
         """
-        data = {
+        params = {
             "page": page
         }
 
-        return cls.methods.get(f"diarios/{id_diario}", data=data)
+        return cls.methods.get(f"diarios/{id_diario}", params=params)
 
     @classmethod
     def download_pdf_pagina(cls, id_diario: int, page: int, path: str, nome_arquivo: str) -> Dict:
         """
         Retorna em formato PDF, uma página do Diário Oficial pelo seu identificador
         :param nome_arquivo:nome para o arquivo baixado
         :param path: diretorio onde o arquivo será salvo
```

### Comparing `escavador-0.3.0/escavador/v1/resources/instituicao.py` & `escavador-0.4.0/escavador/v1/resources/instituicao.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         Retorna os processos de uma instituição
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :argument id_instituicao: o ID da instituição
         :return Dict
         """
 
-        data = {
+        params = {
             'limit': limit,
             'page': page
         }
-        return cls.methods.get(f"instituicoes/{id_instituicao}/processos", data=data)
+        return cls.methods.get(f"instituicoes/{id_instituicao}/processos", params=params)
 
     @classmethod
     def get_pessoas_instituicao(cls, id_instituicao: int, *, limit: Optional[int] = None,
                                 page: Optional[int] = None) -> Dict:
         """
         Retorna as pessoas de uma instituição
         :param id_instituicao: o ID da instituição
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :return Dict
         """
 
-        data = {
+        params = {
             'limit': limit,
             'page': page
         }
-        return cls.methods.get(f"instituicoes/{id_instituicao}/pessoas", data=data)
+        return cls.methods.get(f"instituicoes/{id_instituicao}/pessoas", params=params)
```

### Comparing `escavador-0.3.0/escavador/v1/resources/jurisprudencia.py` & `escavador-0.4.0/escavador/v1/resources/jurisprudencia.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,27 @@
         :param ate_data: filtra os resultados com data de julgamento limite até a data informada
         :param de_data: filtra os resultados com data de julgamento a partir da data informada
         :param ordena_por: modifica a forma como o retorno da busca será ordenado
         :param termo: o termo a ser pesquisado
         :return: Dict
         """
 
-        data = {
+        params = {
             'q': termo,
             'ordena_por': ordena_por,
             'de_data': de_data.strftime("%Y%m%d") if de_data else None,
             'ate_data': ate_data.strftime("%Y%m%d") if ate_data else None,
             'pagina': pagina,
         }
 
         if filtros:
             for filtro in filtros:
-                data.update(filtro)
+                params.update(filtro)
 
-        return cls.methods.get('jurisprudencias/busca', data=data)
+        return cls.methods.get('jurisprudencias/busca', params=params)
 
     @classmethod
     def get_documento_jurisprudencia(cls, tipo_documento: str, id_documento: int) -> Dict:
         """
         Traz informações sobre um documento de Jurisprudência em específico
         :param tipo_documento: o tipo de documento
         :param id_documento: o ID do documento
```

### Comparing `escavador-0.3.0/escavador/v1/resources/legislacao.py` & `escavador-0.4.0/escavador/v1/resources/legislacao.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,24 +27,24 @@
         :param ate_data: filtra os resultados com data de julgamento limite até a data informada
         :param de_data: filtra os resultados com data de julgamento a partir da data informada
         :param ordena_por: modifica a forma como o retorno da busca será ordenado
         :param termo: o termo a ser pesquisado
         :return: Dict
         """
 
-        data = {
+        params = {
             'q': termo,
             'ordena_por': ordena_por,
             'de_data': de_data.strftime("%Y%m%d") if de_data else None,
             'ate_data': ate_data.strftime("%Y%m%d") if ate_data else None,
             'pagina': pagina,
             'filtro': filtro
         }
 
-        return cls.methods.get('legislacoes/busca', data=data)
+        return cls.methods.get('legislacoes/busca', params=params)
 
     @classmethod
     def get_documento_legislacao(cls, tipo_documento: str, id_documento: int) -> Dict:
         """
         Traz informações sobre um documento de Legislação
         :param tipo_documento: O tipo do Documento
         :param id_documento: O ID do documento
```

### Comparing `escavador-0.3.0/escavador/v1/resources/monitoramento_diario.py` & `escavador-0.4.0/escavador/v1/resources/monitoramento_diario.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v1/resources/monitoramento_tribunal.py` & `escavador-0.4.0/escavador/v1/resources/monitoramento_tribunal.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v1/resources/pessoa.py` & `escavador-0.4.0/escavador/v1/resources/pessoa.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,13 +22,13 @@
         """
         Retorna os processos de uma pessoa baseado no ID da pessoa.
         :param id_pessoa: o ID da pessoa
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :return: Dict
         """
-        data = {
+        params = {
             'limit': limit,
             'page': page
         }
 
-        return cls.methods.get(f"pessoas/{id_pessoa}/processos", data=data)
+        return cls.methods.get(f"pessoas/{id_pessoa}/processos", params=params)
```

### Comparing `escavador-0.3.0/escavador/v1/resources/processo.py` & `escavador-0.4.0/escavador/v1/resources/processo.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,19 +160,19 @@
         Busca processos que estão nos Diários Oficiais do Escavador que estão relacionados ao OAB informado
         :param page: número da página
         :param estado_oab: sigla do estado da OAB
         :param numero_oab: número da OAB
         :return: Dict
         """
 
-        data = {
+        params = {
             'page': page
         }
 
-        return cls.methods.get(f"oab/{estado_oab}/{numero_oab}/processos", data=data)
+        return cls.methods.get(f"oab/{estado_oab}/{numero_oab}/processos", params=params)
 
     @classmethod
     def por_id_em_diarios(cls, id_processo: int) -> Dict:
         """
         Retorna um processo pelo seu identificador no Escavador.
         :param id_processo: o ID do processo
         :return: Dict
@@ -187,53 +187,53 @@
         Retorna as movimentações de um Processo pelo identificador do processo no Escavador.
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :param id_processo:  o ID do processo
         :return: Dict
         """
 
-        data = {
+        params = {
             'limit': limit,
             'page': page
         }
 
-        return cls.methods.get(f"processos/{id_processo}/movimentacoes", data=data)
+        return cls.methods.get(f"processos/{id_processo}/movimentacoes", params=params)
 
     @classmethod
     def processo_por_numero_em_diarios(cls, numero_unico: str, *, match_exato: Optional[bool] = None) -> Dict:
         """
         Busca processos que estão nos Diários Oficiais do Escavador. e contenham o número único informado.
         :param match_exato: a busca será feita pelo número inteiro do processo pesquisado.
         :param numero_unico: número único do processo
         :return: Dict
         """
 
-        data = {
+        params = {
             'match_exato': match_exato
         }
 
-        return cls.methods.get(f"processos/numero/{numero_unico}", data=data)
+        return cls.methods.get(f"processos/numero/{numero_unico}", params=params)
 
     @classmethod
     def get_envolvidos_processo(cls, id_processo: int, *, limit: Optional[int] = None,
                                 page: Optional[int] = None) -> Dict:
         """
        Retorna os envolvidos de um Processo pelo identificador do processo no Escavador.
         :param id_processo:  o ID do processo
         :param page: número da página
         :param limit: limita a quantidade de registros retornados
         :return: Dict
         """
 
-        data = {
+        params = {
             'limit': limit,
             'page': page
         }
 
-        return cls.methods.get(f"processos/{id_processo}/envolvidos", data=data)
+        return cls.methods.get(f"processos/{id_processo}/envolvidos", params=params)
 
     @classmethod
     def get_pdf(cls, link_pdf: str, path: str, nome_arquivo: str) -> Dict:
         """
         Baixa um pdf de autos de acordo com seu link e salva no caminho enviado, com o nome enviado
         :param nome_arquivo: nome do arquivo a ser criado
         :param link_pdf: link do documento
```

### Comparing `escavador-0.3.0/escavador/v1/resources/tribunal.py` & `escavador-0.4.0/escavador/v1/resources/tribunal.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v2/resources/envolvido.py` & `escavador-0.4.0/escavador/v2/resources/envolvido.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,20 +40,22 @@
 @dataclass
 class EnvolvidoEncontrado:
     """Representação do envolvido encontrado na busca por envolvido.
 
     :attr nome: nome do envolvido
     :attr tipo_pessoa: tipo de pessoa do envolvido (ex: "FISICA")
     :attr quantidade_processos: quantidade de processos onde o envolvido apareceu
+    :attr cpfs_com_esse_nome: quantidade de CPFs homônimos do envolvido
     :attr last_valid_cursor: cursor válido para a próxima página de resultados
     """
 
     nome: str
     tipo_pessoa: str
-    quantidade_processos: int
+    quantidade_processos: int = field(hash=False, compare=False)
+    cpfs_com_esse_nome: int = field(default=0, hash=False, compare=False)
     last_valid_cursor: str = field(default="None", hash=False, compare=False)
     _classe_buscada: Type["DataEndpoint"] = field(
         default=None, hash=False, compare=False
     )
 
     @classmethod
     def from_json(
@@ -61,20 +63,24 @@
         json_dict: Optional[Dict],
         last_cursor: str = "",
         classe_buscada: Type["DataEndpoint"] = None,
     ) -> Optional["EnvolvidoEncontrado"]:
         if json_dict is None:
             return None
 
+        tipo_pessoa = json_dict.get(
+            "tipo_pessoa", "FISICA"
+        )  # Se não houver tipo_pessoa, assume-se que é advogado, isto é, pessoa física.
         return cls(
             nome=json_dict["nome"],
-            tipo_pessoa=json_dict.get(
-                "tipo_pessoa", "FISICA"
-            ),  # Se não houver tipo_pessoa, assume-se que é advogado.
+            tipo_pessoa=tipo_pessoa,
             quantidade_processos=json_dict["quantidade_processos"],
+            cpfs_com_esse_nome=json_dict.get(
+                "cpfs_com_esse_nome", 1 if tipo_pessoa == "FISICA" else 0
+            ),
             last_valid_cursor=last_cursor,
             _classe_buscada=classe_buscada,
         )
 
     def continuar_busca(self) -> Union[ListaResultados["DataEndpoint"], FailedRequest]:
         """Retorna mais resultados para a busca que gerou o objeto atual.
 
@@ -90,15 +96,15 @@
             self.last_valid_cursor = (
                 resposta["resposta"].get("links", {}).get("next", "")
             )
             return json_to_class(
                 resposta, self._classe_buscada.from_json, add_cursor=True
             )
 
-        return []
+        return ListaResultados()
 
 
 @dataclass
 class Envolvido(DataEndpoint):
     """Representação de um envolvido em um processo, seja ele um advogado, um polo, um juiz, ou um terceiro.
 
     :attr id: id do envolvido no sistema do Escavador
```

### Comparing `escavador-0.3.0/escavador/v2/resources/movimentacao.py` & `escavador-0.4.0/escavador/v2/resources/movimentacao.py`

 * *Files identical despite different names*

### Comparing `escavador-0.3.0/escavador/v2/resources/processo.py` & `escavador-0.4.0/escavador/v2/resources/processo.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,18 +108,18 @@
         Busca as movimentações de um processo pelo seu número único do CNJ.
 
         :param numero_cnj: o número único do CNJ do processo
         :return: uma lista de movimentacoes, ou FailedRequest caso ocorra algum erro
 
         >>> Processo.movimentacoes("0000000-00.0000.0.00.0000") # doctest: +SKIP
         """
-        data = kwargs
+        params = kwargs
 
         first_response = Processo.methods.get(
-            f"processos/numero_cnj/{numero_cnj}/movimentacoes", data=data, **kwargs
+            f"processos/numero_cnj/{numero_cnj}/movimentacoes", params=params, **kwargs
         )
 
         if not first_response["sucesso"]:
             conteudo = first_response.get("resposta", {})
             return FailedRequest(status=first_response["http_status"], **conteudo)
 
         return json_to_class(
@@ -163,42 +163,48 @@
 
     @staticmethod
     def por_cpf(
         cpf: str,
         ordena_por: Optional[CriterioOrdenacao] = None,
         ordem: Optional[Ordem] = None,
         tribunais: Optional[List[SiglaTribunal]] = None,
+        incluir_homonimos: Optional[bool] = None,
         **kwargs,
     ) -> Union[
         Tuple[Optional[EnvolvidoEncontrado], ListaResultados["Processo"]], FailedRequest
     ]:
         """
         Busca os processos envolvendo uma pessoa a partir de seu CPF.
 
         É possível filtrar por tribunal ou ordenar os resultados.
 
         :param cpf: o CPF da pessoa
         :param ordena_por: critério de ordenação
         :param ordem: determina ordenação ascendente ou descendente
         :param tribunais: lista de siglas de tribunais para filtrar a busca
+        :param incluir_homonimos: especifica se a busca por CPF deve incluir processos onde o CPF
+        especificado não está associado, mas há envolvido com o nome igual e não associado a um CPF
+        diferente. Só é permitido se cpf_cnpj for informado.
         :return: tupla com os dados do envolvido encontrado e uma lista de processos,
         ou FailedRequest caso ocorra algum erro
 
         >>> Processo.por_cpf("123.456.789-99") # doctest: +SKIP
 
         >>> Processo.por_cpf("12345678999",
         ...                  ordena_por=CriterioOrdenacao.ULTIMA_MOVIMENTACAO,
         ...                  ordem=Ordem.ASC,
-        ...                  tribunais=[SiglaTribunal.STF]) # doctest: +SKIP
+        ...                  tribunais=[SiglaTribunal.STF],
+        ...                  incluir_homonimos=True) # doctest: +SKIP
         """
         return Processo.por_envolvido(
             cpf_cnpj=cpf,
             ordena_por=ordena_por,
             ordem=ordem,
             tribunais=tribunais,
+            incluir_homonimos=incluir_homonimos,
             **kwargs,
         )
 
     @staticmethod
     def por_cnpj(
         cnpj: str,
         ordena_por: Optional[CriterioOrdenacao] = None,
@@ -238,51 +244,56 @@
     @staticmethod
     def por_envolvido(
         cpf_cnpj: Optional[str] = None,
         nome: Optional[str] = None,
         ordena_por: Optional[CriterioOrdenacao] = None,
         ordem: Optional[Ordem] = None,
         tribunais: Optional[List[SiglaTribunal]] = None,
+        incluir_homonimos: Optional[bool] = None,
         **kwargs,
     ) -> Union[
         Tuple[Optional[EnvolvidoEncontrado], ListaResultados["Processo"]], FailedRequest
     ]:
         """
         Busca os processos envolvendo uma pessoa ou instituição a partir de seu nome e/ou CPF/CNPJ.
 
         É possível filtrar por tribunal e ordenar os resultados.
 
         :param nome: o nome da pessoa ou instituição. Obrigatório se não for informado o CPF/CNPJ
         :param cpf_cnpj: o CPF/CNPJ da pessoa ou instituição. Obrigatório se não for informado o nome
         :param ordena_por: critério de ordenação
         :param ordem: determina ordenação ascendente ou descendente
         :param tribunais: lista de siglas de tribunais para filtrar a busca
+        :param incluir_homonimos: especifica se a busca por CPF deve incluir processos onde o CPF
+        especificado não está associado, mas há envolvido com o nome igual e não associado a um CPF
+        diferente. Só é permitido se cpf_cnpj for informado.
         :return: tupla com os dados do envolvido encontrado e uma lista de processos,
         ou FailedRequest caso ocorra algum erro
 
         >>> Processo.por_envolvido(cpf_cnpj="07.838.351/0021.60") # doctest: +SKIP
 
         >>> Processo.por_envolvido(nome='Escavador Engenharia e Construcoes Ltda',
         ...                             ordena_por=CriterioOrdenacao.ULTIMA_MOVIMENTACAO,
         ...                             ordem=Ordem.ASC,
         ...                             tribunais=[SiglaTribunal.TJBA]) # doctest: +SKIP
         """
-        data = {
+
+        params = {
             "nome": nome,
             "cpf_cnpj": cpf_cnpj,
             "tribunais": tribunais,
-        }
-
-        params = {
             "ordena_por": ordena_por.value if ordena_por else None,
             "ordem": ordem.value if ordem else None,
+            "incluir_homonimos": int(incluir_homonimos)
+            if incluir_homonimos is not None
+            else None,
         }
 
         first_response = Processo.methods.get(
-            "envolvido/processos", data=data, params=params, **kwargs
+            "envolvido/processos", params=params, **kwargs
         )
 
         if not first_response["sucesso"]:
             conteudo = first_response.get("resposta", {})
             return FailedRequest(status=first_response["http_status"], **conteudo)
 
         envolvido_encontrado = EnvolvidoEncontrado.from_json(
@@ -317,25 +328,23 @@
         >>> Processo.por_oab(1234, "AC") # doctest: +SKIP
 
         >>> Processo.por_oab(numero="12345",
         ...                  estado="SP",
         ...                  ordena_por=CriterioOrdenacao.ULTIMA_MOVIMENTACAO,
         ...                  ordem=Ordem.DESC) # doctest: +SKIP
         """
-        data = {
+        params = {
             "oab_numero": f"{numero}",
             "oab_estado": estado,
-        }
-        params = {
             "ordena_por": ordena_por.value if ordena_por else None,
             "ordem": ordem.value if ordem else None,
         }
 
         first_response = Processo.methods.get(
-            "advogado/processos", data=data, params=params, **kwargs
+            "advogado/processos", params=params, **kwargs
         )
 
         if not first_response["sucesso"]:
             conteudo = first_response.get("resposta", {})
             return FailedRequest(status=first_response["http_status"], **conteudo)
 
         advogado_encontrado = EnvolvidoEncontrado.from_json(
```

### Comparing `escavador-0.3.0/pyproject.toml` & `escavador-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "escavador"
-version = "0.3.0"
+version = "0.4.0"
 description = "A library to  interact with Escavador API"
 authors = [
     "Rafael <rafaelcampos@escavador.com>",
     "Gabriel <gabriel@escavador.com>"
 ]
 readme = "README.md"
 homepage = "https://www.escavador.com"
```

### Comparing `escavador-0.3.0/PKG-INFO` & `escavador-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escavador
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library to  interact with Escavador API
 Home-page: https://www.escavador.com
 License: MIT
 Keywords: escavador,api,python
 Author: Rafael
 Author-email: rafaelcampos@escavador.com
 Requires-Python: >=3.6,<4.0
@@ -218,11 +218,11 @@
 | Pessoa                | https://api.escavador.com/v1/docs/#pessoas                           |
 | Tribunal              | https://api.escavador.com/v1/docs/#tribunais                         |
 | Saldo                 | https://api.escavador.com/v1/docs/#saldo-da-api                      |
 
 
 #### V2:
 
-| Módulo                | Link API                                                             |
-|-----------------------|----------------------------------------------------------------------|
-| v2.Processo           | https://api.escavador.com/v2/docs/#processos                         |
-
+| Módulo      | Link API                                     |
+|-------------|----------------------------------------------|
+| v2.Processo | https://api.escavador.com/v2/docs/#processos |
+| v2.Tribunal | https://api.escavador.com/v2/docs/#tribunais |
```

