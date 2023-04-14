# Comparing `tmp/mo_json-6.368.23092-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.370.23104-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 30709 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat    13276 b- defN 23-Apr-02 13:57 mo_json/__init__.py
--rw-rw-rw-  2.0 fat      381 b- defN 20-Jan-29 03:13 mo_json/decoder.py
--rw-rw-rw-  2.0 fat    15497 b- defN 23-Apr-02 13:57 mo_json/encoder.py
--rw-rw-rw-  2.0 fat    16253 b- defN 23-Apr-02 13:57 mo_json/stream.py
--rw-rw-rw-  2.0 fat    17984 b- defN 23-Apr-02 13:57 mo_json/typed_encoder.py
--rw-rw-rw-  2.0 fat     9850 b- defN 23-Apr-02 13:57 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-02 13:57 mo_json-6.368.23092.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11641 b- defN 23-Apr-02 13:57 mo_json-6.368.23092.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-02 13:57 mo_json-6.368.23092.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-02 13:57 mo_json-6.368.23092.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      875 b- defN 23-Apr-02 13:57 mo_json-6.368.23092.dist-info/RECORD
-11 files, 102600 bytes uncompressed, 29249 bytes compressed:  71.5%
+Zip file size: 30545 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    13208 b- defN 23-Apr-14 10:26 mo_json/__init__.py
+-rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
+-rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
+-rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
+-rw-rw-rw-  2.0 fat    17916 b- defN 23-Apr-14 10:26 mo_json/typed_encoder.py
+-rw-rw-rw-  2.0 fat     9865 b- defN 23-Apr-14 10:26 mo_json/types.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11641 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      875 b- defN 23-Apr-14 10:26 mo_json-6.370.23104.dist-info/RECORD
+11 files, 102275 bytes uncompressed, 29085 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mo_json/typed_encoder.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.368.23092.dist-info/LICENSE
+Filename: mo_json-6.370.23104.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.368.23092.dist-info/METADATA
+Filename: mo_json-6.370.23104.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.368.23092.dist-info/WHEEL
+Filename: mo_json-6.370.23104.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.368.23092.dist-info/top_level.txt
+Filename: mo_json-6.370.23104.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.368.23092.dist-info/RECORD
+Filename: mo_json-6.370.23104.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_json/__init__.py

```diff
@@ -3,16 +3,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
-
 import math
 from datetime import timedelta, timezone
 
 from hjson import loads as hjson2value
 from mo_dots import (
     Data,
     FlatList,
```

## mo_json/decoder.py

```diff
@@ -3,12 +3,10 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
-
 import json
 
 json_decoder = json.loads
```

## mo_json/encoder.py

```diff
@@ -3,16 +3,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
-
 import json
 import math
 import time
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 from math import floor
```

## mo_json/stream.py

```diff
@@ -3,16 +3,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
-
 import json
 from types import GeneratorType
 
 from mo_dots import (
     Data,
     Null,
     is_data,
```

## mo_json/typed_encoder.py

```diff
@@ -3,16 +3,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-from __future__ import absolute_import, division, unicode_literals
-
 import re
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 
 from mo_dots import (
     CLASS,
     Data,
```

## mo_json/types.py

```diff
@@ -258,14 +258,15 @@
 JSON_TYPES = (BOOLEAN, INTEGER, NUMBER, STRING, OBJECT)
 NUMBER_TYPES = (INTEGER, NUMBER, TIME, INTERVAL)
 PRIMITIVE = (EXISTS, BOOLEAN, INTEGER, NUMBER, TIME, INTERVAL, STRING)
 INTERNAL = (EXISTS, OBJECT, ARRAY)
 STRUCT = (OBJECT, ARRAY)
 
 _B, _I, _N, _T, _D, _S, _A, _J = "~b~", "~i~", "~n~", "~t~", "~d~", "~s~", "~a~", "~j~"
+ARRAY_KEY = _A
 IS_PRIMITIVE_KEY = re.compile(r"^~[bintds]~$")
 
 JX_IS_NULL = _new(JxType)
 JX_BOOLEAN = _primitive(_B, BOOLEAN)
 JX_INTEGER = _primitive(_I, INTEGER)
 JX_NUMBER = _primitive(_N, NUMBER)
 JX_TIME = _primitive(_T, TIME)
```

## Comparing `mo_json-6.368.23092.dist-info/LICENSE` & `mo_json-6.370.23104.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.368.23092.dist-info/METADATA` & `mo_json-6.370.23104.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.368.23092
+Version: 6.370.23104
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

