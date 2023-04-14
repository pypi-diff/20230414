# Comparing `tmp/rpa_cooperativa-1.0.43.tar.gz` & `tmp/rpa_cooperativa-1.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.43.tar", last modified: Thu Apr 13 17:54:51 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.44.tar", last modified: Fri Apr 14 16:19:48 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.43.tar` & `rpa_cooperativa-1.0.44.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:54:51.305712 rpa_cooperativa-1.0.43/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.43/LICENSE
--rw-rw-rw-   0        0        0     6237 2023-04-13 17:54:51.284915 rpa_cooperativa-1.0.43/PKG-INFO
--rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.43/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:54:50.954987 rpa_cooperativa-1.0.43/rpa_coop/
--rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.43/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:54:51.172010 rpa_cooperativa-1.0.43/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.43/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.43/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.43/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siac_verde.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.43/rpa_coop/img/siat_verde.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.43/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.43/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    69808 2023-04-13 17:52:50.000000 rpa_cooperativa-1.0.43/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:54:51.268273 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6237 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-04-13 17:54:50.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 17:54:49.000000 rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 17:54:51.308832 rpa_cooperativa-1.0.43/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-04-13 17:54:17.000000 rpa_cooperativa-1.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.582793 rpa_cooperativa-1.0.44/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.44/LICENSE
+-rw-rw-rw-   0        0        0     6237 2023-04-14 16:19:48.571153 rpa_cooperativa-1.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.44/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.014308 rpa_cooperativa-1.0.44/rpa_coop/
+-rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.44/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.456875 rpa_cooperativa-1.0.44/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.44/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.44/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.44/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siac_verde.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siat_verde.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.44/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.44/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    71296 2023-04-14 13:41:26.000000 rpa_cooperativa-1.0.44/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.553872 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6237 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:19:48.587124 rpa_cooperativa-1.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-04-14 12:23:09.000000 rpa_cooperativa-1.0.44/setup.py
```

### Comparing `rpa_cooperativa-1.0.43/LICENSE` & `rpa_cooperativa-1.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/PKG-INFO` & `rpa_cooperativa-1.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.43
+Version: 1.0.44
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.43/README.md` & `rpa_cooperativa-1.0.44/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.44/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.44/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.44/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.44/rpa_coop/rpa_coop.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,15 @@
             banco = self.database_sistema_senhas
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
             # conexao = mysql.connect(host=self.ip_sistema_senhas, port=3307, database=banco, user=self.user_sistema_senhas, password=self.pw_bd_sistema_senhas)
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
-                
-                   
+                         
     def criar_conexao(self, db:str, user_db='user_opcional', password_db='senha_opcional', ip_ou_host_db='ip_host_opcional', porta='3306', library_sql='mysqlconnector'):
         '''
         retorna conexao com db, db='parametro_obrigatorio' \n
         schema planinng: db = ('planning', 'fluid', 'cronos', 'controles_internos') \n
         schema sistema_senhas: db = 'sistema_senhas' \n
         schema grafana: db = 'grafana' \n
         schema denodo: db = ('ldw', 'seguros', 'cooperativa', 'auditoria_7000') \n
@@ -170,15 +169,14 @@
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
             # conexao = mysql.connect(host=self.ip_sistema_senhas, port=3307, database=banco, user=self.user_sistema_senhas, password=self.pw_bd_sistema_senhas)
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
         
-        
     def api_consulta_denodo(self, database:str, tabela:str, colunas:str, filtro_where="opcional"):
         '''
         filtro = "coluna2 eq 'SIM' and coluna3 eq 'Ativo'" \n
         df = dados.api_consulta_denodo('ldw', 'nome_da_tabela', 'coluna1, coluna5', filtro) \n\n
         
         # operadores para filtro where: \n
         eq = igual \n
@@ -202,16 +200,15 @@
         rows = json.loads(response.content)
         try:
             df = pd.DataFrame(rows['elements'])
         except:
             print('erro ao converter para DataFrame, json retornou: \n', response.text.encode('utf8'))
         return df   
         
-    
-        
+     
     def consultar_banco_dados(self, conexao_engine, query_sql:str, retorna_DataFrame=True):
         '''
         retorna um DataFrame pandas \n
         exemplo de query: \n
         SELECT * FROM rpa_historico WHERE cod_rpa = "3000" \n
         '''
         if retorna_DataFrame:
@@ -254,14 +251,28 @@
                 
         
     def insert_DataFrame_to_db(self, df, engine, nome_da_tabela:str, if_existir='append', mostrar_index=False):
         df.to_sql(nome_da_tabela, engine, if_exists=if_existir, index = mostrar_index)
         print('Inserção realizada com sucesso')
 
 
+    def delete_linhas_banco_dados(self, conexao_engine, query_sql):
+        '''
+        realiza delete na tabela do banco de dados \n
+        exemplo de query: \n
+        "DELETE FROM rpa_fila WHERE id_fila = 9161" \n
+        '''
+        aux_query = str(query_sql).upper()
+        if 'WHERE' in aux_query:
+            conexao_engine.execute(query_sql)
+            print('Exclusão realizada com sucesso')
+        else:
+            print('Não foi possível realizar a exclusão, é necessário informar o WHERE na query')
+            
+
 
 class Fluid:
     
     def __init__(self):
         
         self.id_usuario = str(gerador_pwd('fluid_cod_user', 'senha'))
         self.token_fluid = str(gerador_pwd('token_api_fluid', 'senha'))
@@ -517,39 +528,41 @@
             # print(msg)
             # print(response.text)  
             # print('processo identificado como novo') 
             # print()
             return msg, acao 
         
     
-    def criar_processo_rascunho(self, id_tipo_processo:str, id_empresa_origem=1, id_empresa_destino=1, responsavel_destino=2735, arvore=0):
+    def criar_processo_rascunho(self, id_tipo_processo:str, id_empresa_origem=1, id_empresa_destino=1, id_usuario=0, responsavel_destino=0, arvore=0):
         '''
             id_processo, nodo_inicial = post_criar_processo(id_tipo_processo)\n
             ou\n
             id_processo, nodo_inicial = post_criar_processo(id_tipo_processo, id_empresa_origem=cod_agencia, id_empresa_destino=cod_agencia)
         '''
         url_final = f'{self.url_api}/processos/novo'
         headers = {"Content-Type": "application/json; charset=utf-8", "organization": self.organizacao, "Authorization": self.token_fluid }
         
         if id_empresa_origem != 1: id_empresa_origem = self.depara(id_empresa_origem)
         if id_empresa_destino != 1: id_empresa_destino = self.depara(id_empresa_destino)
+        if id_usuario == 0: id_usuario = self.id_usuario
+        if responsavel_destino == 0: responsavel_destino = self.id_usuario
         
         time.sleep(1)
         id_versao_arvore = 0
         if arvore == 0:
             id_versao_arvore, nodo_inicial = self.nodo_e_arvore_para_novo_processo(str(id_tipo_processo)) # pega a arvore vigente, ou em criação
         else:
             id_versao_arvore = arvore
         tempo_minutos = self.get_sla(id_tipo_processo)
         
         obj_acao = {
             "tipo_processo": id_tipo_processo, # id do tipo de processo fluid
             "tempo": tempo_minutos, # tempo em minutos
-            "responsavel_criacao": self.id_usuario, # id do usuário fluid
-            "responsavel_origem": self.id_usuario, # id do usuário fluid
+            "responsavel_criacao": id_usuario, # id do usuário fluid
+            "responsavel_origem": id_usuario, # id do usuário fluid
             "responsavel_destino": responsavel_destino,
             "empresa_origem": id_empresa_origem, 
             "empresa_destino": id_empresa_destino,
             "versao_processo": id_versao_arvore # versao da arvore do processo, abra a arvore e veja no final da url o id
             }
         
         # no Método POST passar os parametros {url, headers, json}
@@ -800,23 +813,27 @@
         if res.status_code != 204:
             raise Exception(f'Erro ao gravar dados no processo {cod_processo}: {res.text}')
         else:
             print(f'Dados gravados com sucesso no processo fluid {cod_processo}')
             return res.status_code
     
     
-    def protocolar_processo_fluid(self, cod_processo: str, id_tipo_processo: str,  mensagem: str, id_empresa_origem='1', id_empresa_destino='1', nome_do_nodo ='selecionado_proximo_nodo', abertura_de_processo= False, cod_nodo=0, cod_acao = 0, usuario_destino=2735):
+    def protocolar_processo_fluid(self, cod_processo: str, id_tipo_processo: str,  mensagem: str, id_empresa_origem='1', id_empresa_destino='1', nome_do_nodo ='selecionado_proximo_nodo', abertura_de_processo= False, cod_nodo=0, cod_acao = 0, id_usuario=0, usuario_destino=0):
         ''' 
             post_protocolar_processo_fluid(processo, id_tipo_processo, msg, nome_nodo_destino, empresa_orig, empresa_dest) \n
             post_protocolar_processo_fluid('497305', '945', 'automação realizada') \n
             post_protocolar_processo_fluid('497305', '945', 'automação realizada', empresa_orig=68, empresa_dest=68) \n
             post_protocolar_processo_fluid('497305', '945', 'automação realizada', 'Devolver') \n
             post_protocolar_processo_fluid('497305', '945', 'automação realizada', 'Concluir') \n
             
         '''
+        
+        if id_usuario == 0: id_usuario = self.id_usuario
+        if usuario_destino == 0: usuario_destino = self.id_usuario
+        
         url = f'{self.url_api}/processos/protocolar'
         headers = { "Content-Type": "application/json; charset=utf-8", "organization": self.organizacao, "Authorization": self.token_fluid }
         if id_empresa_origem  != 1: id_empresa_origem = self.depara(id_empresa_origem)
         if id_empresa_destino != 1: id_empresa_destino = self.depara(id_empresa_destino)
         
         if cod_nodo == 0:
             nodo, acao = self.get_nodo_possiveis_destinos(cod_processo, nome_do_nodo)
@@ -829,15 +846,15 @@
         
         obj_acao = {
             "acao": acao, # ação 0, protocolar normal com mensagem
             "processo": cod_processo,
             "destino": nodo, # nodo destino da arvore do processo, para onde vai qdo protocolar
             "parecer": mensagem, # mensagem para escrever no parecer ao protocolar
             "parecer_restrito": 0,
-            "usuario": self.id_usuario, # id usuario fluid que esta realizando a operacao por api
+            "usuario": id_usuario, # id usuario fluid que esta realizando a operacao por api
             "empresa_origem": id_empresa_origem, # empresa 1
             "empresa_destino": id_empresa_destino, # usar zero para sede, e para agencia passar cod_fluid referente a agencia , fazer depara. 
             "usuario_destino": usuario_destino
             }
 
         response = requests.post(url, headers=headers, json=obj_acao)    
         cod_res_api = str(response.status_code)
@@ -851,14 +868,28 @@
         if (cod_res_api == '204'):
             print(f'processo fluid {cod_processo} protocolado com sucesso')
             return cod_res_api
         else:
             raise Exception(f'Erro ao protocolar processo {cod_processo}: {response.text}')
 
 
+    def tomar_posse(self, cod_processo:str, empresa=1, id_usuario=0):
+        time.sleep(1)        
+        url = f'{self.url_api}/processos/tomar-posse'
+        if id_usuario == 0: id_usuario = self.id_usuario
+        
+        headers = {"organization": self.organizacao, "Authorization": self.token_fluid }
+        param = {"usuario": id_usuario, "empresa": empresa, "processo": cod_processo}
+        res = requests.post(url, headers=headers, json=param)
+
+        if res.status_code != 204: raise Exception(f'Erro ao gravar dados no processo {cod_processo}, {res.text}')
+        print(f'Ok, tomou posse do processo: {cod_processo}')
+        return res.status_code
+
+
 
 class Whatsapp:
  
     def __init__(self):
         self.url_api_whats = str(gerador_pwd('url_api_whats', 'sistema'))
         self.token_api_whats = str(gerador_pwd('url_api_whats', 'senha'))
         self.template_informa_novo = str(gerador_pwd('template_informa_novo', 'sistema'))
```

### Comparing `rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.43
+Version: 1.0.44
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.43/setup.py` & `rpa_cooperativa-1.0.44/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.43",
+    version="1.0.44",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

