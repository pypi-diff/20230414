# Comparing `tmp/fastapi_users_db_beanie-1.1.4.tar.gz` & `tmp/fastapi_users_db_beanie-2.0.0.tar.gz`

## Comparing `fastapi_users_db_beanie-1.1.4.tar` & `fastapi_users_db_beanie-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.editorconfig
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/test_build.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.github/stale.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/fastapi_users_db_beanie/__init__.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/fastapi_users_db_beanie/access_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/fastapi_users_db_beanie/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/tests/conftest.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/tests/test_access_token.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/tests/test_fastapi_users_db_beanie.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/LICENSE
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/README.md
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/PKG-INFO
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-1.1.4/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/test_build.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/stale.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/__init__.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/access_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/test_access_token.py
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/test_fastapi_users_db_beanie.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/README.md
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/setup.py
```

### Comparing `fastapi_users_db_beanie-1.1.4/.github/stale.yml` & `fastapi_users_db_beanie-2.0.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-1.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `fastapi_users_db_beanie-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-1.1.4/.github/workflows/build.yml` & `fastapi_users_db_beanie-2.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-1.1.4/fastapi_users_db_beanie/__init__.py` & `fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """FastAPI Users database adapter for Beanie."""
-from typing import TYPE_CHECKING, Any, Dict, Generic, Optional, Type, TypeVar
+from typing import Any, Dict, Generic, Optional, Type, TypeVar
 
 import bson.errors
 from beanie import Document, PydanticObjectId
 from fastapi_users.db.base import BaseUserDatabase
 from fastapi_users.exceptions import InvalidID
 from fastapi_users.models import ID, OAP
 from pydantic import BaseModel, Field
 from pymongo import IndexModel
 from pymongo.collation import Collation
 
-__version__ = "1.1.4"
+__version__ = "2.0.0"
 
 
-class BeanieBaseUser(Generic[ID], Document):
-    if TYPE_CHECKING:
-        id: ID  # type: ignore # pragma: no cover
+class BeanieBaseUser(BaseModel):
     email: str
     hashed_password: str
     is_active: bool = True
     is_superuser: bool = False
     is_verified: bool = False
 
     class Settings:
@@ -28,28 +26,34 @@
             IndexModel("email", unique=True),
             IndexModel(
                 "email", name="case_insensitive_email_index", collation=email_collation
             ),
         ]
 
 
-UP_BEANIE = TypeVar("UP_BEANIE", bound=BeanieBaseUser)
+class BeanieBaseUserDocument(BeanieBaseUser, Document):  # type: ignore
+    pass
+
+
+UP_BEANIE = TypeVar("UP_BEANIE", bound=BeanieBaseUserDocument)
 
 
 class BaseOAuthAccount(BaseModel):
     id: PydanticObjectId = Field(default_factory=PydanticObjectId)
     oauth_name: str
     access_token: str
     account_id: str
     account_email: str
     expires_at: Optional[int] = None
     refresh_token: Optional[str] = None
 
 
-class BeanieUserDatabase(Generic[UP_BEANIE, ID], BaseUserDatabase[UP_BEANIE, ID]):
+class BeanieUserDatabase(
+    Generic[UP_BEANIE], BaseUserDatabase[UP_BEANIE, PydanticObjectId]
+):
     """
     Database adapter for Beanie.
 
     :param user_model: Beanie user model.
     :param oauth_account_model: Optional Beanie OAuth account model.
     """
 
@@ -85,21 +89,23 @@
                 "oauth_accounts.account_id": account_id,
             }
         )
 
     async def create(self, create_dict: Dict[str, Any]) -> UP_BEANIE:
         """Create a user."""
         user = self.user_model(**create_dict)
-        return await user.insert()
+        await user.create()
+        return user
 
     async def update(self, user: UP_BEANIE, update_dict: Dict[str, Any]) -> UP_BEANIE:
         """Update a user."""
         for key, value in update_dict.items():
             setattr(user, key, value)
-        return await user.save()
+        await user.save()
+        return user
 
     async def delete(self, user: UP_BEANIE) -> None:
         """Delete a user."""
         await user.delete()
 
     async def add_oauth_account(
         self, user: UP_BEANIE, create_dict: Dict[str, Any]
@@ -107,15 +113,16 @@
         """Create an OAuth account and add it to the user."""
         if self.oauth_account_model is None:
             raise NotImplementedError()
 
         oauth_account = self.oauth_account_model(**create_dict)
         user.oauth_accounts.append(oauth_account)  # type: ignore
 
-        return await user.save()
+        await user.save()
+        return user
 
     async def update_oauth_account(
         self, user: UP_BEANIE, oauth_account: OAP, update_dict: Dict[str, Any]
     ) -> UP_BEANIE:
         """Update an OAuth account on a user."""
         if self.oauth_account_model is None:
             raise NotImplementedError()
@@ -124,15 +131,16 @@
             if (
                 existing_oauth_account.oauth_name == oauth_account.oauth_name
                 and existing_oauth_account.account_id == oauth_account.account_id
             ):
                 for key, value in update_dict.items():
                     setattr(user.oauth_accounts[i], key, value)  # type: ignore
 
-        return await user.save()
+        await user.save()
+        return user
 
 
 class ObjectIDIDMixin:
     def parse_id(self, value: Any) -> PydanticObjectId:
         try:
             return PydanticObjectId(value)
         except (bson.errors.InvalidId, TypeError) as e:
```

### Comparing `fastapi_users_db_beanie-1.1.4/fastapi_users_db_beanie/access_token.py` & `fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/access_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from datetime import datetime, timezone
-from typing import Any, Dict, Generic, Optional, Type, TypeVar
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    Optional,
+    Type,
+    TypeVar,
+)
 
-from beanie import Document
+from beanie import Document, PydanticObjectId
 from fastapi_users.authentication.strategy.db import AccessTokenDatabase
-from fastapi_users.models import ID
-from pydantic import Field
+from pydantic import BaseModel, Field
 from pymongo import IndexModel
 
 
-class BeanieBaseAccessToken(Generic[ID], Document):
+class BeanieBaseAccessToken(BaseModel):
     token: str
-    user_id: ID
+    user_id: PydanticObjectId
     created_at: datetime = Field(default_factory=lambda: datetime.now(timezone.utc))
 
     class Settings:
         indexes = [IndexModel("token", unique=True)]
 
 
-AP_BEANIE = TypeVar("AP_BEANIE", bound=BeanieBaseAccessToken)
+class BeanieBaseAccessTokenDocument(BeanieBaseAccessToken, Document):  # type: ignore
+    pass
+
+
+AP_BEANIE = TypeVar("AP_BEANIE", bound=BeanieBaseAccessTokenDocument)
 
 
 class BeanieAccessTokenDatabase(Generic[AP_BEANIE], AccessTokenDatabase[AP_BEANIE]):
     """
     Access token database adapter for Beanie.
 
     :param access_token_model: Beanie access token model.
@@ -36,18 +46,20 @@
         query: Dict[str, Any] = {"token": token}
         if max_age is not None:
             query["created_at"] = {"$gte": max_age}
         return await self.access_token_model.find_one(query)
 
     async def create(self, create_dict: Dict[str, Any]) -> AP_BEANIE:
         access_token = self.access_token_model(**create_dict)
-        return await access_token.save()
+        await access_token.create()
+        return access_token
 
     async def update(
         self, access_token: AP_BEANIE, update_dict: Dict[str, Any]
     ) -> AP_BEANIE:
         for key, value in update_dict.items():
             setattr(access_token, key, value)
-        return await access_token.save()
+        await access_token.save()
+        return access_token
 
     async def delete(self, access_token: AP_BEANIE) -> None:
         await access_token.delete()
```

### Comparing `fastapi_users_db_beanie-1.1.4/tests/test_access_token.py` & `fastapi_users_db_beanie-2.0.0/tests/test_access_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime, timedelta, timezone
 from typing import AsyncGenerator
 
 import pymongo.errors
 import pytest
-from beanie import PydanticObjectId, init_beanie
+from beanie import Document, PydanticObjectId, init_beanie
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase
 
 from fastapi_users_db_beanie.access_token import (
     BeanieAccessTokenDatabase,
     BeanieBaseAccessToken,
 )
 
 
-class AccessToken(BeanieBaseAccessToken[PydanticObjectId]):
+class AccessToken(BeanieBaseAccessToken, Document):
     pass
 
 
 @pytest.fixture(scope="module")
 async def mongodb_client():
     client = AsyncIOMotorClient(
         "mongodb://localhost:27017",
@@ -59,19 +59,22 @@
 
     # Create
     access_token = await beanie_access_token_db.create(access_token_create)
     assert access_token.token == "TOKEN"
     assert access_token.user_id == user_id
 
     # Update
-    update_dict = {"created_at": datetime.now(timezone.utc)}
+    updated_created_at = datetime.now(timezone.utc)
+    update_dict = {"created_at": updated_created_at}
     updated_access_token = await beanie_access_token_db.update(
         access_token, update_dict
     )
-    assert updated_access_token.created_at == update_dict["created_at"]
+    assert updated_access_token.created_at == update_dict["created_at"].replace(
+        microsecond=int(updated_created_at.microsecond / 1000) * 1000, tzinfo=None
+    )
 
     # Get by token
     access_token_by_token = await beanie_access_token_db.get_by_token(
         access_token.token
     )
     assert access_token_by_token is not None
```

### Comparing `fastapi_users_db_beanie-1.1.4/tests/test_fastapi_users_db_beanie.py` & `fastapi_users_db_beanie-2.0.0/tests/test_fastapi_users_db_beanie.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, AsyncGenerator, Dict, List, Optional
 
 import pymongo.errors
 import pytest
-from beanie import PydanticObjectId, init_beanie
+from beanie import Document, PydanticObjectId, init_beanie
 from fastapi_users import InvalidID
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase
 from pydantic import Field
 
 from fastapi_users_db_beanie import (
     BaseOAuthAccount,
     BeanieBaseUser,
     BeanieUserDatabase,
     ObjectIDIDMixin,
 )
 
 
-class User(BeanieBaseUser[PydanticObjectId]):
+class User(Document, BeanieBaseUser):
     first_name: Optional[str] = None
 
 
 class OAuthAccount(BaseOAuthAccount):
     pass
 
 
@@ -66,15 +66,15 @@
     yield BeanieUserDatabase(UserOAuth, OAuthAccount)
 
     await mongodb_client.drop_database("test_database")
 
 
 @pytest.mark.asyncio
 async def test_queries(
-    beanie_user_db: BeanieUserDatabase[User, PydanticObjectId],
+    beanie_user_db: BeanieUserDatabase[User],
     oauth_account1: Dict[str, Any],
 ):
     user_create = {
         "email": "lancelot@camelot.bt",
         "hashed_password": "guinevere",
     }
 
@@ -136,15 +136,15 @@
         ("lancelot+guinevere@camelot.bt", "lancelot+guinevere@camelot.bt", True),
         ("lancelot+guinevere@camelot.bt", "lancelot.*", False),
         ("квіточка@пошта.укр", "квіточка@пошта.укр", True),
         ("квіточка@пошта.укр", "КВІТОЧКА@ПОШТА.УКР", True),
     ],
 )
 async def test_email_query(
-    beanie_user_db: BeanieUserDatabase[User, PydanticObjectId],
+    beanie_user_db: BeanieUserDatabase[User],
     email: str,
     query: str,
     found: bool,
 ):
     user_create = {
         "email": email,
         "hashed_password": "guinevere",
@@ -157,30 +157,28 @@
         assert email_user is not None
         assert email_user.id == user.id
     else:
         assert email_user is None
 
 
 @pytest.mark.asyncio
-async def test_insert_existing_email(
-    beanie_user_db: BeanieUserDatabase[User, PydanticObjectId]
-):
+async def test_insert_existing_email(beanie_user_db: BeanieUserDatabase[User]):
     user_create = {
         "email": "lancelot@camelot.bt",
         "hashed_password": "guinevere",
     }
     await beanie_user_db.create(user_create)
 
     with pytest.raises(pymongo.errors.DuplicateKeyError):
         await beanie_user_db.create(user_create)
 
 
 @pytest.mark.asyncio
 async def test_queries_custom_fields(
-    beanie_user_db: BeanieUserDatabase[User, PydanticObjectId],
+    beanie_user_db: BeanieUserDatabase[User],
 ):
     """It should output custom fields in query result."""
     user_create = {
         "email": "lancelot@camelot.bt",
         "hashed_password": "guinevere",
         "first_name": "Lancelot",
     }
@@ -191,15 +189,15 @@
     assert id_user is not None
     assert id_user.id == user.id
     assert id_user.first_name == user.first_name
 
 
 @pytest.mark.asyncio
 async def test_queries_oauth(
-    beanie_user_db_oauth: BeanieUserDatabase[UserOAuth, PydanticObjectId],
+    beanie_user_db_oauth: BeanieUserDatabase[UserOAuth],
     oauth_account1: Dict[str, Any],
     oauth_account2: Dict[str, Any],
 ):
     user_create = {
         "email": "lancelot@camelot.bt",
         "hashed_password": "guinevere",
     }
```

### Comparing `fastapi_users_db_beanie-1.1.4/.gitignore` & `fastapi_users_db_beanie-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-1.1.4/LICENSE` & `fastapi_users_db_beanie-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-1.1.4/README.md` & `fastapi_users_db_beanie-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users-db-beanie/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie)
 [![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)](https://badge.fury.io/py/fastapi-users-db-beanie)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-users-db-beanie)
 <p align="center">
-<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
+<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>
 
 **Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [!
 [codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/
 master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 beanie) [![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)]
 (https://badge.fury.io/py/fastapi-users-db-beanie) [![Downloads](https://
 pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-
 users-db-beanie)
-                           [https://md-btn.deta.dev/
+                    [https://md-buttons.francoisvoron.com/
 button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. **Sub-package for Beanie support in
 FastAPI Users.** ## Development ### Setup environment We use [Hatch](https://
```

### Comparing `fastapi_users_db_beanie-1.1.4/pyproject.toml` & `fastapi_users_db_beanie-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 [tool.hatch.envs.default]
 dependencies = [
     "pytest",
     "pytest-asyncio",
     "black",
     "mypy",
-    "codecov",
     "pytest-cov",
     "pytest-mock",
     "asynctest",
     "httpx",
     "asgi_lifespan",
     "ruff",
 ]
```

### Comparing `fastapi_users_db_beanie-1.1.4/PKG-INFO` & `fastapi_users_db_beanie-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-users-db-beanie
-Version: 1.1.4
+Version: 2.0.0
 Summary: FastAPI Users database adapter for Beanie
 Project-URL: Documentation, https://fastapi-users.github.io/fastapi-users
 Project-URL: Source, https://github.com/fastapi-users/fastapi-users-db-beanie
 Author-email: François Voron <fvoron@gmail.com>, Schwannden Kuo <schwannden@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
@@ -34,15 +34,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users-db-beanie/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie)
 [![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)](https://badge.fury.io/py/fastapi-users-db-beanie)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-users-db-beanie)
 <p align="center">
-<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
+<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>
 
 **Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-users-db-beanie Version: 1.1.4 Summary:
+Metadata-Version: 2.1 Name: fastapi-users-db-beanie Version: 2.0.0 Summary:
 FastAPI Users database adapter for Beanie Project-URL: Documentation, https://
 fastapi-users.github.io/fastapi-users Project-URL: Source, https://github.com/
 fastapi-users/fastapi-users-db-beanie Author-email: FranÃ§ois Voron
 gmail.com>, Schwannden Kuo
 gmail.com> License-File: LICENSE Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Framework ::
 FastAPI Classifier: Intended Audience :: Developers Classifier: License :: OSI
@@ -20,15 +20,15 @@
 Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [!
 [codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/
 master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 beanie) [![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)]
 (https://badge.fury.io/py/fastapi-users-db-beanie) [![Downloads](https://
 pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-
 users-db-beanie)
-                           [https://md-btn.deta.dev/
+                    [https://md-buttons.francoisvoron.com/
 button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. **Sub-package for Beanie support in
 FastAPI Users.** ## Development ### Setup environment We use [Hatch](https://
```

### Comparing `fastapi_users_db_beanie-1.1.4/setup.py` & `fastapi_users_db_beanie-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='fastapi-users-db-beanie',
-    version='1.1.4',
+    version='2.0.0',
     description='FastAPI Users database adapter for Beanie',
-    long_description='# FastAPI Users - Database adapter for Beanie\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">\n</p>\n\n<p align="center">\n    <em>Ready-to-use and customizable users management for FastAPI</em>\n</p>\n\n[![build](https://github.com/fastapi-users/fastapi-users-db-beanie/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie)\n[![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)](https://badge.fury.io/py/fastapi-users-db-beanie)\n[![Downloads](https://pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-users-db-beanie)\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>\n\n**Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>\n\n---\n\nAdd quickly a registration and authentication system to your [FastAPI](https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as customizable and adaptable as possible.\n\n**Sub-package for Beanie support in FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    long_description='# FastAPI Users - Database adapter for Beanie\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">\n</p>\n\n<p align="center">\n    <em>Ready-to-use and customizable users management for FastAPI</em>\n</p>\n\n[![build](https://github.com/fastapi-users/fastapi-users-db-beanie/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie)\n[![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)](https://badge.fury.io/py/fastapi-users-db-beanie)\n[![Downloads](https://pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-users-db-beanie)\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>\n\n**Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>\n\n---\n\nAdd quickly a registration and authentication system to your [FastAPI](https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as customizable and adaptable as possible.\n\n**Sub-package for Beanie support in FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     author_email='François Voron <fvoron@gmail.com>, Schwannden Kuo <schwannden@gmail.com>',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: AsyncIO',
         'Framework :: FastAPI',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*- from setuptools import setup setup( name='fastapi-
-users-db-beanie', version='1.1.4', description='FastAPI Users database adapter
+users-db-beanie', version='2.0.0', description='FastAPI Users database adapter
 for Beanie', long_description='# FastAPI Users - Database adapter for
 Beanie\n\n
                              \n [FastAPI Users]\n
 \n\n
         \n Ready-to-use and customizable users management for FastAPI\n
 \n\n[![build](https://github.com/fastapi-users/fastapi-users-db-beanie/
 workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/
 actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 beanie/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/
 fastapi-users-db-beanie)\n[![PyPI version](https://badge.fury.io/py/fastapi-
 users-db-beanie.svg)](https://badge.fury.io/py/fastapi-users-db-beanie)\n[!
 [Downloads](https://pepy.tech/badge/fastapi-users-db-beanie)](https://
 pepy.tech/project/fastapi-users-db-beanie)\n
-                          \n[https://md-btn.deta.dev/
+                   \n[https://md-buttons.francoisvoron.com/
 button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]\n
 \n\n---\n\n**Documentation**: https://fastapi-users.github.io/fastapi-users/
 \n\n**Source Code**: https://github.com/fastapi-users/fastapi-users\n\n---
 \n\nAdd quickly a registration and authentication system to your [FastAPI]
 (https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible.\n\n**Sub-package for Beanie support in
 FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe use [Hatch]
```

