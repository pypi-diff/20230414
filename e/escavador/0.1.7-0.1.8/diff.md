# Comparing `tmp/escavador-0.1.7.tar.gz` & `tmp/escavador-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escavador-0.1.7.tar", max compression
+gzip compressed data, was "escavador-0.1.8.tar", max compression
```

## Comparing `escavador-0.1.7.tar` & `escavador-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1065 2023-02-08 20:44:36.396986 escavador-0.1.7/LICENSE
--rw-r--r--   0        0        0     3791 2023-02-08 20:44:36.396986 escavador-0.1.7/README.md
--rw-r--r--   0        0        0      230 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/__init__.py
--rw-r--r--   0        0        0     1566 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/api.py
--rw-r--r--   0        0        0       52 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/exceptions.py
--rw-r--r--   0        0        0      528 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/method.py
--rw-r--r--   0        0        0      704 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/__init__.py
--rw-r--r--   0        0        0     1060 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/busca.py
--rw-r--r--   0        0        0      570 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/busca_assincrona.py
--rw-r--r--   0        0        0     1973 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/callback.py
--rw-r--r--   0        0        0     1518 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/diario_oficial.py
--rw-r--r--   0        0        0        0 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/helpers/__init__.py
--rw-r--r--   0        0        0      842 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/helpers/documento.py
--rw-r--r--   0        0        0      119 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/helpers/endpoint.py
--rw-r--r--   0        0        0      721 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/helpers/enums.py
--rw-r--r--   0        0        0     1567 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/instituicao.py
--rw-r--r--   0        0        0     2908 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/jurisprudencia.py
--rw-r--r--   0        0        0     2357 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/legislacao.py
--rw-r--r--   0        0        0     4144 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/monitoramento_diario.py
--rw-r--r--   0        0        0     2411 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/monitoramento_tribunal.py
--rw-r--r--   0        0        0      393 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/movimentacao.py
--rw-r--r--   0        0        0      938 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/pessoa.py
--rw-r--r--   0        0        0    10586 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/processo.py
--rw-r--r--   0        0        0      296 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/saldo.py
--rw-r--r--   0        0        0      602 2023-02-08 20:44:36.396986 escavador-0.1.7/escavador/resources/tribunal.py
--rw-r--r--   0        0        0      668 2023-02-08 20:44:36.396986 escavador-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4679 1970-01-01 00:00:00.000000 escavador-0.1.7/setup.py
--rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 escavador-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-14 19:57:07.301640 escavador-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3791 2023-04-14 19:57:07.301640 escavador-0.1.8/README.md
+-rw-r--r--   0        0        0      230 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/__init__.py
+-rw-r--r--   0        0        0     1675 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/api.py
+-rw-r--r--   0        0        0       52 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/exceptions.py
+-rw-r--r--   0        0        0      528 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/method.py
+-rw-r--r--   0        0        0      704 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/__init__.py
+-rw-r--r--   0        0        0     1060 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/busca.py
+-rw-r--r--   0        0        0      570 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/busca_assincrona.py
+-rw-r--r--   0        0        0     1973 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/callback.py
+-rw-r--r--   0        0        0     1518 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/diario_oficial.py
+-rw-r--r--   0        0        0        0 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/documento.py
+-rw-r--r--   0        0        0      119 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/endpoint.py
+-rw-r--r--   0        0        0      721 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/helpers/enums.py
+-rw-r--r--   0        0        0     1567 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/instituicao.py
+-rw-r--r--   0        0        0     3237 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/jurisprudencia.py
+-rw-r--r--   0        0        0     2357 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/legislacao.py
+-rw-r--r--   0        0        0     4144 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/monitoramento_diario.py
+-rw-r--r--   0        0        0     2411 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/monitoramento_tribunal.py
+-rw-r--r--   0        0        0      393 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/movimentacao.py
+-rw-r--r--   0        0        0      938 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/pessoa.py
+-rw-r--r--   0        0        0    10603 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/processo.py
+-rw-r--r--   0        0        0      296 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/saldo.py
+-rw-r--r--   0        0        0      602 2023-04-14 19:57:07.301640 escavador-0.1.8/escavador/resources/tribunal.py
+-rw-r--r--   0        0        0      693 2023-04-14 19:57:07.301640 escavador-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 escavador-0.1.8/PKG-INFO
```

### Comparing `escavador-0.1.7/LICENSE` & `escavador-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/README.md` & `escavador-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/api.py` & `escavador-0.1.8/escavador/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import requests
 
 import escavador
 from escavador.exceptions import ApiKeyNotFoundException
 from urllib import parse
 from dotenv import load_dotenv
+from importlib_metadata import version
 
 load_dotenv()
 
 
 class Api(object):
 
     def __init__(self):
@@ -18,14 +19,15 @@
             try:
                 self.api_key = os.environ['ESCAVADOR_API_KEY']
             except KeyError:
                 raise ApiKeyNotFoundException("Nenhuma chave da API foi informada")
 
     def headers(self):
         return {
+            'User-Agent': 'escavador-python/' + version('escavador'),
             'Authorization': 'Bearer ' + self.api_key,
             'X-Requested-With': 'XMLHttpRequest'
         }
 
     def request(self, method, url, **kwargs):
         url = parse.urljoin(self.base_url, url)
         data = kwargs.get('data')
```

### Comparing `escavador-0.1.7/escavador/method.py` & `escavador-0.1.8/escavador/method.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/__init__.py` & `escavador-0.1.8/escavador/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/busca.py` & `escavador-0.1.8/escavador/resources/busca.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/busca_assincrona.py` & `escavador-0.1.8/escavador/resources/busca_assincrona.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/callback.py` & `escavador-0.1.8/escavador/resources/callback.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/diario_oficial.py` & `escavador-0.1.8/escavador/resources/diario_oficial.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/helpers/documento.py` & `escavador-0.1.8/escavador/resources/helpers/documento.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/helpers/enums.py` & `escavador-0.1.8/escavador/resources/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/instituicao.py` & `escavador-0.1.8/escavador/resources/instituicao.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/jurisprudencia.py` & `escavador-0.1.8/escavador/resources/jurisprudencia.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from escavador.resources.helpers.endpoint import Endpoint
 from escavador.resources.helpers.documento import Documento
-from typing import Optional, Dict
+from typing import Optional, Dict, List
 from datetime import  datetime
 
 
 class Jurisprudencia(Endpoint):
 
     def filtros_busca_jurisprudencia(self) -> Dict:
         """
-        Lista de filtros disponíveis para a busca de jurisprudências
+        Lista de filtros disponíveis para a busca de jurisprudências,
+        Para cada item da lista de filtros, o campo filtro representa a chave (key) da query.
+        No campo opcoes, listamos todas as opções de valor para aquele filtro, e, para cada opção,
+         o campo valor representa o valor (value) da query.
         :return: Dict
         """
         return self.methods.get("jurisprudencias")
 
     def busca_por_jurisprudencias(self, termo: str, *, ordena_por: Optional[str] = None, de_data: Optional[datetime] = None,
                                   ate_data: Optional[datetime] = None, pagina: Optional[int] = None,
-                                  filtro: Optional[str] = None) -> Dict:
+                                  filtros: Optional[List[Dict]] = None) -> Dict:
         """
         Traz a lista paginada dos itens encontrados na busca.
-        :param filtro: Um dos filtros listados pelo método filtros_busca_jurisprudencia()
+        :param filtros: filtros listados pelo método filtros_busca_jurisprudencia()
         :param pagina: lista os itens de uma página
         :param ate_data: filtra os resultados com data de julgamento limite até a data informada
         :param de_data: filtra os resultados com data de julgamento a partir da data informada
         :param ordena_por: modifica a forma como o retorno da busca será ordenado
         :param termo: o termo a ser pesquisado
         :return: Dict
         """
 
         data = {
             'q': termo,
             'ordena_por': ordena_por,
             'de_data': de_data.strftime("%Y%m%d") if de_data else None,
             'ate_data': ate_data.strftime("%Y%m%d") if ate_data else None,
             'pagina': pagina,
-            'filtro': filtro
         }
 
+        if filtros:
+            for filtro in filtros:
+                data.update(filtro)
+
         return self.methods.get('jurisprudencias/busca', data=data)
 
     def get_documento_jurisprudencia(self, tipo_documento: str, id_documento: int) -> Dict:
         """
         Traz informações sobre um documento de Jurisprudência em específico
         :param tipo_documento: o tipo de documento
         :param id_documento: o ID do documento
```

### Comparing `escavador-0.1.7/escavador/resources/legislacao.py` & `escavador-0.1.8/escavador/resources/legislacao.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/monitoramento_diario.py` & `escavador-0.1.8/escavador/resources/monitoramento_diario.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/monitoramento_tribunal.py` & `escavador-0.1.8/escavador/resources/monitoramento_tribunal.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/pessoa.py` & `escavador-0.1.8/escavador/resources/pessoa.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/escavador/resources/processo.py` & `escavador-0.1.8/escavador/resources/processo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from __future__ import annotations
+# from __future__ import annotations
 from escavador.resources.helpers.endpoint import Endpoint
 from escavador.resources.helpers.enums import TiposBusca
 from escavador.resources.helpers.documento import Documento
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Union
 
 
 class Processo(Endpoint):
 
     def informacoes_no_tribunal(self, numero_unico: str, *, send_callback: Optional[bool] = None,
                            wait: Optional[bool] = None,
                            autos: Optional[bool] = None, documentos_publicos:  Optional[bool] = None,
@@ -115,15 +115,15 @@
             'wait': wait,
             'tentativas': tentativas
         }
 
         return self.methods.post(f"tribunal/{origem.upper()}/busca-por-oab/async", data=data)
 
     def busca_em_lote_no_tribunal(self, tipo_busca: TiposBusca, origens: List[str], *, send_callback: Optional[bool] = None,
-                      numero_oab: Optional[str | int] = None, estado_oab: Optional[str] = None,
+                      numero_oab: Union[str, int, None] = None, estado_oab: Optional[str] = None,
                       numero_documento: Optional[str] = None, nome: Optional[str] = None) -> Dict:
         """
         Cria buscas do mesmo tipo para todos os tribunais enviados
         :param nome: o nome que será pesquisado
         :param numero_documento: o documento que será pesquisado
         :param estado_oab:  o estado da oab enviada
         :param numero_oab:  o numero da oab que será pesquisado
@@ -143,15 +143,15 @@
             'numero_oab': numero_oab,
             'estado_oab': estado_oab,
             'send_callback': send_callback
         }
 
         return self.methods.post("tribunal/async/lote", data=data)
 
-    def processos_por_oab_em_diarios(self, estado_oab: str, numero_oab: str | int, *, page: Optional[int] = None) -> Dict:
+    def processos_por_oab_em_diarios(self, estado_oab: str, numero_oab: Union[str, int], *, page: Optional[int] = None) -> Dict:
         """
         Busca processos que estão nos Diários Oficiais do Escavador que estão relacionados ao OAB informado
         :param page: número da página
         :param estado_oab: sigla do estado da OAB
         :param numero_oab: número da OAB
         :return: Dict
         """
```

### Comparing `escavador-0.1.7/escavador/resources/tribunal.py` & `escavador-0.1.8/escavador/resources/tribunal.py`

 * *Files identical despite different names*

### Comparing `escavador-0.1.7/pyproject.toml` & `escavador-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "escavador"
-version = "0.1.7"
+version = "0.1.8"
 description = "A library to  interact with Escavador API"
 authors = [
     "Rafael <rafaelcampos@escavador.com>",
     "Gabriel <gabriel@escavador.com>"
 ]
 readme = "README.md"
 homepage = "https://www.escavador.com"
@@ -14,13 +14,14 @@
 keywords = ["escavador", "api", "python"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 requests = "^2.27.1"
 cchardet = "^2.1.7"
 python-dotenv = "^0.19.2"
+importlib_metadata = "*"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `escavador-0.1.7/setup.py` & `escavador-0.1.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,111 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['escavador', 'escavador.resources', 'escavador.resources.helpers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cchardet>=2.1.7,<3.0.0',
- 'python-dotenv>=0.19.2,<0.20.0',
- 'requests>=2.27.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'escavador',
-    'version': '0.1.7',
-    'description': 'A library to  interact with Escavador API',
-    'long_description': '## SDK em python para utilizar a API do Escavador\n\n### Instalação\n    \nInstale utilizando o pip:\n```bash\npip install escavador\n```\n\n### Como Configurar\n\n- Crie no `.env` do seu projeto uma variável `ESCAVADOR_API_KEY` com seu token da API\n- ou\n- utilize a função `config()`\n```py\nimport escavador\nescavador.config("API_KEY")\n```\n\n- para obter seu token da API, acesse o [painel de tokens](https://api.escavador.com/tokens)\n\n### Exemplo de como utilizar\n[Buscando informações do processo no sistema do Tribunal](https://api.escavador.com/docs/#pesquisar-processo-no-site-do-tribunal-assncrono) (Assíncrono)\n```py\nfrom escavador import Processo, BuscaAssincrona\nimport time\n\nresultado_busca = Processo().informacoes_no_tribunal("0078700-86.2008.5.17.0009")  # Gera uma busca assíncrona\n\nwhile resultado_busca[\'resposta\'][\'status\'] == \'PENDENTE\':\n    # Aguarda para checar novamente\n    print("Está pendente")\n    time.sleep(20)\n\n    id_async = resultado_busca[\'resposta\'][\'id\']\n    resultado_busca = BuscaAssincrona().por_id(id_async)\n\n# Checa a saida do processso\nif resultado_busca[\'resposta\'][\'status\'] == \'ERRO\':\n    print("Deu erro, tentar novamente")\n    exit(0)\n\nif resultado_busca[\'resposta\'][\'status\'] == \'SUCESSO\':\n    busca_async = resultado_busca[\'resposta\']\n    for instancia in busca_async[\'resposta\'][\'instancias\']:\n        print(instancia[\'assunto\'])  # Imprime os assuntos das instâncias do processo\n```\n\n### Criando Monitoramentos\n```py\nfrom escavador import MonitoramentoTribunal, MonitoramentoDiario, TiposMonitoramentosTribunal, TiposMonitoramentosDiario,FrequenciaMonitoramentoTribunal\n\n# Monitoramento nos sisteams dos Tribunais\nmonitoramento_tribunal = MonitoramentoTribunal().criar(tipo_monitoramento=TiposMonitoramentosTribunal.UNICO,\n                                                                     valor="8809061-58.2022.8.10.3695",tribunal=\'TJSP\', \n                                                                     frequencia=FrequenciaMonitoramentoTribunal.SEMANAL)\n\n# Monitoramento em Diários Oficiais\nmonitoramento_diario = MonitoramentoDiario().criar(TiposMonitoramentosDiario.PROCESSO, processo_id=2, origens_ids=[2,4,6])\n```\n\n### Consultando os Tribunais e sistemas disponíveis\n```py\nfrom escavador import Tribunal\n\ntribunais_disponiveis = Tribunal().sistemas_disponiveis()\n```\n\n### Módulos Disponíveis e Referência da API\n\n| Módulo                | Link API                                                          |\n|-----------------------|-------------------------------------------------------------------|\n| Busca                 | https://api.escavador.com/docs/#busca                             |\n| Processo              | https://api.escavador.com/docs/#processos                         |\n| Callback              | https://api.escavador.com/docs/#callback                          |\n| DiarioOficial         | https://api.escavador.com/docs/#dirios-oficiais                   |\n| Instituicao           | https://api.escavador.com/docs/#instituies                        |\n| Legislacao            | https://api.escavador.com/docs/#legislao                          |\n| Jurisprudencia        | https://api.escavador.com/docs/#jurisprudncias                    |\n| MonitoramentoDiario   | https://api.escavador.com/docs/#monitoramento-de-dirios-oficiais  |\n| MonitoramentoTribunal | https://api.escavador.com/docs/#monitoramento-no-site-do-tribunal |\n| Movimentacao          | https://api.escavador.com/docs/#movimentaes                       |\n| Pessoa                | https://api.escavador.com/docs/#pessoas                           |\n| Tribunal              | https://api.escavador.com/docs/#tribunais                         |\n| Saldo                 | https://api.escavador.com/docs/#saldo-da-api                      | ',
-    'author': 'Rafael',
-    'author_email': 'rafaelcampos@escavador.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://www.escavador.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: escavador
+Version: 0.1.8
+Summary: A library to  interact with Escavador API
+Home-page: https://www.escavador.com
+License: MIT
+Keywords: escavador,api,python
+Author: Rafael
+Author-email: rafaelcampos@escavador.com
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cchardet (>=2.1.7,<3.0.0)
+Requires-Dist: importlib_metadata
+Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Documentation, https://api.escavador.com/docs/
+Project-URL: Repository, https://github.com/Escavador/escavador-python
+Description-Content-Type: text/markdown
+
+## SDK em python para utilizar a API do Escavador
+
+### Instalação
+    
+Instale utilizando o pip:
+```bash
+pip install escavador
+```
+
+### Como Configurar
+
+- Crie no `.env` do seu projeto uma variável `ESCAVADOR_API_KEY` com seu token da API
+- ou
+- utilize a função `config()`
+```py
+import escavador
+escavador.config("API_KEY")
+```
+
+- para obter seu token da API, acesse o [painel de tokens](https://api.escavador.com/tokens)
+
+### Exemplo de como utilizar
+[Buscando informações do processo no sistema do Tribunal](https://api.escavador.com/docs/#pesquisar-processo-no-site-do-tribunal-assncrono) (Assíncrono)
+```py
+from escavador import Processo, BuscaAssincrona
+import time
+
+resultado_busca = Processo().informacoes_no_tribunal("0078700-86.2008.5.17.0009")  # Gera uma busca assíncrona
+
+while resultado_busca['resposta']['status'] == 'PENDENTE':
+    # Aguarda para checar novamente
+    print("Está pendente")
+    time.sleep(20)
+
+    id_async = resultado_busca['resposta']['id']
+    resultado_busca = BuscaAssincrona().por_id(id_async)
+
+# Checa a saida do processso
+if resultado_busca['resposta']['status'] == 'ERRO':
+    print("Deu erro, tentar novamente")
+    exit(0)
+
+if resultado_busca['resposta']['status'] == 'SUCESSO':
+    busca_async = resultado_busca['resposta']
+    for instancia in busca_async['resposta']['instancias']:
+        print(instancia['assunto'])  # Imprime os assuntos das instâncias do processo
+```
+
+### Criando Monitoramentos
+```py
+from escavador import MonitoramentoTribunal, MonitoramentoDiario, TiposMonitoramentosTribunal, TiposMonitoramentosDiario,FrequenciaMonitoramentoTribunal
+
+# Monitoramento nos sisteams dos Tribunais
+monitoramento_tribunal = MonitoramentoTribunal().criar(tipo_monitoramento=TiposMonitoramentosTribunal.UNICO,
+                                                                     valor="8809061-58.2022.8.10.3695",tribunal='TJSP', 
+                                                                     frequencia=FrequenciaMonitoramentoTribunal.SEMANAL)
+
+# Monitoramento em Diários Oficiais
+monitoramento_diario = MonitoramentoDiario().criar(TiposMonitoramentosDiario.PROCESSO, processo_id=2, origens_ids=[2,4,6])
+```
+
+### Consultando os Tribunais e sistemas disponíveis
+```py
+from escavador import Tribunal
+
+tribunais_disponiveis = Tribunal().sistemas_disponiveis()
+```
+
+### Módulos Disponíveis e Referência da API
+
+| Módulo                | Link API                                                          |
+|-----------------------|-------------------------------------------------------------------|
+| Busca                 | https://api.escavador.com/docs/#busca                             |
+| Processo              | https://api.escavador.com/docs/#processos                         |
+| Callback              | https://api.escavador.com/docs/#callback                          |
+| DiarioOficial         | https://api.escavador.com/docs/#dirios-oficiais                   |
+| Instituicao           | https://api.escavador.com/docs/#instituies                        |
+| Legislacao            | https://api.escavador.com/docs/#legislao                          |
+| Jurisprudencia        | https://api.escavador.com/docs/#jurisprudncias                    |
+| MonitoramentoDiario   | https://api.escavador.com/docs/#monitoramento-de-dirios-oficiais  |
+| MonitoramentoTribunal | https://api.escavador.com/docs/#monitoramento-no-site-do-tribunal |
+| Movimentacao          | https://api.escavador.com/docs/#movimentaes                       |
+| Pessoa                | https://api.escavador.com/docs/#pessoas                           |
+| Tribunal              | https://api.escavador.com/docs/#tribunais                         |
+| Saldo                 | https://api.escavador.com/docs/#saldo-da-api                      |
```

