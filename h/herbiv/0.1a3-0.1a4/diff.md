# Comparing `tmp/herbiv-0.1a3.tar.gz` & `tmp/herbiv-0.1a4.tar.gz`

## Comparing `herbiv-0.1a3.tar` & `herbiv-0.1a4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 herbiv-0.1a3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/__init__.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/analysis.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/compute.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/get.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/output.py
--rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_chemical_protein_links.csv
--rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_chemicals.csv
--rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_tcm.csv
--rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a3/src/herbiv/data/HerbiV_tcm_chemical_links.csv
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a3/LICENSE
--rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 herbiv-0.1a3/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 herbiv-0.1a3/pyproject.toml
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 herbiv-0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 herbiv-0.1a4/setup.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/analysis.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/compute.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/get.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/output.py
+-rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_chemical_protein_links.csv
+-rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_chemicals.csv
+-rw-r--r--   0        0        0  1978068 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_proteins.csv
+-rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_tcm.csv
+-rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a4/src/herbiv/data/HerbiV_tcm_chemical_links.csv
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a4/LICENSE
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 herbiv-0.1a4/README.md
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 herbiv-0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 herbiv-0.1a4/PKG-INFO
```

### Comparing `herbiv-0.1a3/setup.py` & `herbiv-0.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="herbiv",
-    version="0.1a3",
+    version="0.1a4",
     description="HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology.",
     # Optional
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV",
     author="王皓阳",
     author_email="Wesady@qq.com",
```

### Comparing `herbiv-0.1a3/src/herbiv/compute.py` & `herbiv-0.1a4/src/herbiv/compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,13 +37,12 @@
 
     tcm_info1 = get.get_tcm('cn_name', ['柴胡'])
     tcm_chem_links_info1 = get.get_tcm_chem_links('HVMID', tcm_info1['HVMID'])
     chem_info1 = get.get_chemicals('HVCID', tcm_chem_links_info1['HVCID'])
     chem_protein_links1 = get.get_chem_protein_links('HVCID', chem_info1['HVCID'])
     chem_info1, tcm_info1 = score(chem_protein_links1, chem_info1, tcm_chem_links_info1, tcm_info1)
 
-    chem_protein_links2 = get.get_chem_protein_links('Ensembl_ID',
-                                                     {'ENSP0000026332': 'ACACA', 'ENSP00000398698': 'TNF'}, 0)
+    chem_protein_links2 = get.get_chem_protein_links('Ensembl_ID', ['ENSP0000026332', 'ENSP00000398698'], 0)
     chem_info2 = get.get_chemicals('HVCID', chem_protein_links2['HVCID'])
     tcm_chem_links_info2 = get.get_tcm_chem_links('HVCID', chem_info2['HVCID'])
     tcm_info2 = get.get_tcm('HVMID', tcm_chem_links_info2['HVMID'])
     chem_info2, tcm_info2 = score(chem_protein_links2, chem_info2, tcm_chem_links_info2, tcm_info2)
```

### Comparing `herbiv-0.1a3/src/herbiv/get.py` & `herbiv-0.1a4/src/herbiv/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,17 +86,41 @@
 
     # 重新设置索引
     chem_protein_links.index = range(chem_protein_links.shape[0])
 
     return chem_protein_links
 
 
+def get_proteins(by, items):
+    r"""
+    从HerbiV_proteins中获得基因名与其对应的Ensemble_ID,从而可以被from_genes函数所调用，这样直接输入基因名即可
+    :param by: str类型，数据集中与items相匹配的列的列名
+    :param items: pd.DataFrame或其他任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的蛋白质
+    :return:返回一个包含对应信息的字典
+    :return:返回一个数据框
+    """
+
+    # 数据的输入
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    proteins_all = pd.read_csv(current_directory + r'/data/HerbiV_proteins.csv')
+
+    # 在HerbiV_chemical_proteins中获取items中化合物的信息
+    proteins = proteins_all.loc[proteins_all[by].isin(items)].drop_duplicates(subset=['Ensembl_ID'])
+
+    # 重置索引
+    proteins.index = range(proteins.shape[0])
+
+    return proteins
+
+
 if __name__ == '__main__':
     tcm_info1 = get_tcm('cn_name', ['柴胡'])
     tcm_chem_links_info1 = get_tcm_chem_links('HVMID', tcm_info1['HVMID'])
     chem_info1 = get_chemicals('HVCID', tcm_chem_links_info1['HVCID'])
     chem_protein_links1 = get_chem_protein_links('HVCID', chem_info1['HVCID'])
+    protein1 = get_proteins('Ensembl_ID', chem_protein_links1['Ensembl_ID'])
 
-    chem_protein_links2 = get_chem_protein_links('Ensembl_ID', {'ENSP0000026332': 'ACACA', 'ENSP00000398698': 'TNF'}, 0)
+    protein2 = get_proteins('Ensembl_ID', ['ENSP00000252519', 'ENSP00000381588'])
+    chem_protein_links2 = get_chem_protein_links('Ensembl_ID', protein2['Ensembl_ID'], 0)
     chem_info2 = get_chemicals('HVCID', chem_protein_links2['HVCID'])
     tcm_chem_links_info2 = get_tcm_chem_links('HVCID', chem_info2['HVCID'])
-    tcm_info2 = get_tcm('HVMID', tcm_chem_links_info2['HVMID'])
+    tcm_info2 = get_tcm('HVMID', tcm_chem_links_info2['HVMID'])
```

### Comparing `herbiv-0.1a3/src/herbiv/output.py` & `herbiv-0.1a4/src/herbiv/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def out_for_cyto(chem_protein_links, chem, genes, tcm_chem_links, tcm, path='result/'):
     r"""
     输出Cytoscape用于作图的网络文件和属性文件
     :param chem_protein_links: pd.DataFrame类型，HerbiV_chemical_protein_links数据集数据集中包含目标基因且Combined_score大于等于score的记录
     :param chem: pd.DataFrame类型，chem_protein_links中化合物的信息及其Importance Score
-    :param genes: 字典类型，存储拟分析蛋白（基因）在STITCH中的ID与其名称的对应关系
+    :param genes: pd.DataFrame类型，存储拟分析蛋白（基因）在STITCH中的ID与其名称的对应关系
     :param tcm_chem_links: pd.DataFrame类型，包含filtered_chem中化合物的名称、STITCH数据库中的CID和HERB数据库中对应的中药
     :param tcm: pd.DataFrame类型，tcm_chem_links中中药的信息及其Importance Score
     :param path: 字符串类型，存放结果的目录
     """
 
     chem_protein_links_c = chem_protein_links.copy()
     chem_c = chem.copy()
@@ -20,49 +20,67 @@
     tcm_c = tcm.copy()
 
     # 若无path目录，先创建该目录
     if not os.path.exists(path):
         os.mkdir(path)
     out_chem_protein_links = chem_protein_links_c.iloc[:, 0:2]
     out_chem_protein_links.columns = ['SourceNode', 'TargetNode']
+
     out_chem_protein_links.loc[:, 'SourceNode'] = out_chem_protein_links.loc[:, 'SourceNode'].apply(
-        lambda x: chem_c.loc[chem_c['HVCID'] == x]['Name'].iloc[0])
+        lambda x: chem_c.loc[chem_c['HVCID'] == x]['Name'].iloc[0] if len(
+            chem_c.loc[chem_c['HVCID'] == x]['Name']) > 0 else None)
+
+    out_chem_protein_links.dropna(subset=['SourceNode'], inplace=True)
+
     out_chem_protein_links.loc[:, 'TargetNode'] = out_chem_protein_links.loc[:, 'TargetNode'].apply(
-        lambda x: genes_c.get(x))
+        lambda x: genes_c.loc[genes_c['Ensembl_ID'] == x]['gene_name'].iloc[0] if len(
+            genes_c.loc[genes_c['Ensembl_ID'] == x]['gene_name']) > 0 else None)
+
+    out_chem_protein_links.dropna(subset=['TargetNode'], inplace=True)
 
     out_tcm_chem = tcm_chem_links_c.iloc[:, 0:2]
     out_tcm_chem.columns = ['SourceNode', 'TargetNode']
+
     out_tcm_chem.loc[:, 'SourceNode'] = out_tcm_chem.loc[:, 'SourceNode'].apply(
-        lambda x: tcm_c.loc[tcm_c['HVMID'] == x]['cn_name'].iloc[0])
+        lambda x: tcm_c.loc[tcm_c['HVMID'] == x]['cn_name'].iloc[0] if len(
+            tcm_c.loc[tcm_c['HVMID'] == x]['cn_name']) > 0 else None)
+
+    out_tcm_chem.dropna(subset=['SourceNode'], inplace=True)
+
     out_tcm_chem.loc[:, 'TargetNode'] = out_tcm_chem.loc[:, 'TargetNode'].apply(
-        lambda x: chem_c.loc[chem_c['HVCID'] == x]['Name'].iloc[0])
+        lambda x: chem_c.loc[chem_c['HVCID'] == x]['Name'].iloc[0] if len(
+            chem_c.loc[chem_c['HVCID'] == x]['Name']) > 0 else None)
+
+    out_tcm_chem.dropna(subset=['TargetNode'], inplace=True)
 
     out_chem = chem_c.loc[:, ['Name']]
     out_chem.columns = ['Key']
     out_chem['Attribute'] = 'Chemicals'
 
     out_tcm = tcm_c.loc[:, ['cn_name']]
     out_tcm.columns = ['Key']
     out_tcm['Attribute'] = 'TCM'
 
-    out_gene = pd.DataFrame({'Key': [*genes_c.values()]})
+    out_gene = genes_c.loc[:, ['gene_name']]
+    out_gene.columns = ['Key']
     out_gene['Attribute'] = 'gene'
 
     # 输出Network文件
     pd.concat([out_chem_protein_links, out_tcm_chem]).to_csv(path + 'Network.csv', index=False)
 
     # 输出Type文件
     pd.concat([out_tcm, out_chem, out_gene]).to_csv(path + 'Type.csv', index=False)
 
 
 if __name__ == '__main__':
     import get
     import compute
 
-    genes_info = {'ENSP0000026332': 'ACACA', 'ENSP00000398698': 'TNF'}
+    genes_info = ['ENSP0000026332', 'ENSP00000398698']
+    proteins = get.get_proteins('Ensembl_ID', genes_info)
     chem_protein_links_info = get.get_chem_protein_links('Ensembl_ID', genes_info, 0)
     chem_info = get.get_chemicals('HVCID', chem_protein_links_info['HVCID'])
     tcm_chem_links_info = get.get_tcm_chem_links('HVCID', chem_info['HVCID'])
     tcm_info = get.get_tcm('HVMID', tcm_chem_links_info['HVMID'])
-    chem_protein_links_info, chem_info, tcm_info = compute.score(chem_protein_links_info, chem_info, tcm_chem_links_info, tcm_info)
+    chem_info, tcm_info = compute.score(chem_protein_links_info, chem_info, tcm_chem_links_info, tcm_info)
 
-    out_for_cyto(chem_protein_links_info, chem_info, genes_info, tcm_chem_links_info, tcm_info)
+    out_for_cyto(chem_protein_links_info, chem_info, genes_info, tcm_chem_links_info, tcm_info)
```

### Comparing `herbiv-0.1a3/src/herbiv/data/HerbiV_chemical_protein_links.csv` & `herbiv-0.1a4/src/herbiv/data/HerbiV_chemical_protein_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a3/src/herbiv/data/HerbiV_chemicals.csv` & `herbiv-0.1a4/src/herbiv/data/HerbiV_chemicals.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a3/src/herbiv/data/HerbiV_tcm.csv` & `herbiv-0.1a4/src/herbiv/data/HerbiV_tcm.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a3/src/herbiv/data/HerbiV_tcm_chemical_links.csv` & `herbiv-0.1a4/src/herbiv/data/HerbiV_tcm_chemical_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a3/LICENSE` & `herbiv-0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a3/README.md` & `herbiv-0.1a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+<h1 align="center">
+<img src="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV/blob/main/logo.svg" width="200l0">
+</h1>
+
 [![Downloads](https://static.pepy.tech/personalized-badge/herbiv?period=total&units=international_system&left_color=green&right_color=blue&left_text=Downloads)](https://pepy.tech/project/herbiv)
 [![Downloads](https://static.pepy.tech/personalized-badge/pharmastar?period=month&units=international_system&left_color=green&right_color=blue&left_text=Old%20Version(Pharmastar)%20Downloads)](https://pepy.tech/project/pharmastar)
 
 HerbiV一个开发中的具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。
 
 HerbiV is a multifunctional traditional chinese medicine network pharmacology analysis tool 
 under development for classical network pharmacology and reverse network pharmacology.
```

### Comparing `herbiv-0.1a3/pyproject.toml` & `herbiv-0.1a4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
 requires = [
     "hatchling",
-    "numpy",
     "pandas",
     "typing-extensions",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "herbiv"
-version = "0.1a3"
+version = "0.1a4"
 authors = [
   { name="王皓阳", email="Wesady@qq.com" },
 ]
 description = "药理大师是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。Pharmastar is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `herbiv-0.1a3/PKG-INFO` & `herbiv-0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herbiv
-Version: 0.1a3
+Version: 0.1a4
 Summary: 药理大师是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。Pharmastar is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology.
 Project-URL: Homepage, https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar
 Project-URL: Bug Tracker, https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar/issues
 Author-email: 王皓阳 <Wesady@qq.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Healthcare Industry
@@ -15,14 +15,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
+<h1 align="center">
+<img src="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV/blob/main/logo.svg" width="200l0">
+</h1>
+
 [![Downloads](https://static.pepy.tech/personalized-badge/herbiv?period=total&units=international_system&left_color=green&right_color=blue&left_text=Downloads)](https://pepy.tech/project/herbiv)
 [![Downloads](https://static.pepy.tech/personalized-badge/pharmastar?period=month&units=international_system&left_color=green&right_color=blue&left_text=Old%20Version(Pharmastar)%20Downloads)](https://pepy.tech/project/pharmastar)
 
 HerbiV一个开发中的具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。
 
 HerbiV is a multifunctional traditional chinese medicine network pharmacology analysis tool 
 under development for classical network pharmacology and reverse network pharmacology.
```

