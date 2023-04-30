# Comparing `tmp/elliptic_sdk-0.0.3.tar.gz` & `tmp/elliptic_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elliptic_sdk-0.0.3.tar", max compression
+gzip compressed data, was "elliptic_sdk-0.0.4.tar", max compression
```

## Comparing `elliptic_sdk-0.0.3.tar` & `elliptic_sdk-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1075 2023-04-19 13:23:40.198775 elliptic_sdk-0.0.3/LICENSE
--rw-r--r--   0        0        0       21 2023-04-19 13:32:23.004077 elliptic_sdk-0.0.3/elliptic_sdk/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-19 14:15:46.386875 elliptic_sdk-0.0.3/elliptic_sdk/aml.py
--rw-r--r--   0        0        0      165 2023-04-19 13:47:35.835487 elliptic_sdk-0.0.3/elliptic_sdk/enums.py
--rw-r--r--   0        0        0     1479 2023-04-26 10:56:28.366239 elliptic_sdk-0.0.3/elliptic_sdk/schemas.py
--rw-r--r--   0        0        0      310 2023-04-19 13:30:59.908133 elliptic_sdk-0.0.3/elliptic_sdk/settings.py
--rw-r--r--   0        0        0     1044 2023-04-26 11:29:27.668205 elliptic_sdk-0.0.3/elliptic_sdk/test_aml.py
--rw-r--r--   0        0        0      440 2023-04-26 11:29:54.300864 elliptic_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 elliptic_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-19 13:23:40.198775 elliptic_sdk-0.0.4/LICENSE
+-rw-r--r--   0        0        0       66 2023-04-30 16:15:34.229645 elliptic_sdk-0.0.4/elliptic_sdk/__init__.py
+-rw-r--r--   0        0        0     1538 2023-04-30 16:15:34.230285 elliptic_sdk-0.0.4/elliptic_sdk/aml.py
+-rw-r--r--   0        0        0     1947 2023-04-30 16:15:34.230389 elliptic_sdk-0.0.4/elliptic_sdk/auth.py
+-rw-r--r--   0        0        0      329 2023-04-30 16:15:34.230482 elliptic_sdk-0.0.4/elliptic_sdk/client.py
+-rw-r--r--   0        0        0      446 2023-04-30 16:15:34.230615 elliptic_sdk-0.0.4/elliptic_sdk/enums.py
+-rw-r--r--   0        0        0     1766 2023-04-30 16:15:34.230754 elliptic_sdk-0.0.4/elliptic_sdk/schemas.py
+-rw-r--r--   0        0        0      379 2023-04-30 16:15:34.230977 elliptic_sdk-0.0.4/elliptic_sdk/settings.py
+-rw-r--r--   0        0        0      484 2023-04-30 16:15:50.386263 elliptic_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 elliptic_sdk-0.0.4/PKG-INFO
```

### Comparing `elliptic_sdk-0.0.3/LICENSE` & `elliptic_sdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.3/elliptic_sdk/schemas.py` & `elliptic_sdk-0.0.4/elliptic_sdk/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,85 @@
+"""Elliptic SDK elliptic_sdk/schemas.py."""
 import uuid
 from datetime import datetime
 from typing import Any
-from typing import List
-from pydantic import BaseModel
-from pydantic import Field
-from .enums import LegacyWalletTypeEnum
-from .enums import LegacyWalletPayloadTypeEnum
+
+from pydantic import BaseModel, Field
+
+from .enums import LegacyWalletPayloadTypeEnum, WalletAnalysisSubjectTypeEnum
 
 
 class LegacyWalletSubject(BaseModel):
-    type: LegacyWalletTypeEnum = Field(default=LegacyWalletTypeEnum.ADDRESS)
+    """LegacyWalletSubject schema."""
+
     asset: str
-    blockchain: str
+    type: WalletAnalysisSubjectTypeEnum = Field(
+        default=WalletAnalysisSubjectTypeEnum.ADDRESS,
+    )
     hash: str
+    blockchain: str
 
     class Config:
+        """Config."""
+
         use_enum_values = True
 
 
 class LegacyWalletPayload(BaseModel):
+    """LegacyWalletPayload schema."""
+
     subject: LegacyWalletSubject
     type: LegacyWalletPayloadTypeEnum = Field(
-        default=LegacyWalletPayloadTypeEnum.WALLET_EXPOSURE)
+        default=LegacyWalletPayloadTypeEnum.WALLET_EXPOSURE,
+    )
     customer_reference: str
 
     class Config:
+        """Config."""
+
         use_enum_values = True
 
 
 class AnalysedBy(BaseModel):
+    """AnalysedBy schema."""
+
     id: uuid.UUID
     type: str
 
 
 class ClusterEntity(BaseModel):
+    """ClusterEntity schema."""
+
     name: str
     category: str
-    actor_id: int
     is_primary_entity: bool
     is_vasp: Any
+    actor_id: int
     is_after_sanction_date: bool
 
 
 class Customer(BaseModel):
+    """Customer schema."""
+
     reference: str
 
 
 class LegacyWalletResponse(BaseModel):
-    analysed_by: AnalysedBy
-    cluster_entities: List[ClusterEntity]
+    """LegacyWalletResponse schema."""
+
     id: uuid.UUID
-    subject: LegacyWalletSubject
     type: LegacyWalletPayloadTypeEnum
+    subject: LegacyWalletSubject
     customer: Customer
     created_at: datetime
     updated_at: datetime
     analysed_at: datetime
-    process_status: str
-    process_status_id: int
-    workflow_status_id: int
-    workflow_status: str
-    error: str | None
-    team_id: uuid.UUID
+    analysed_by: AnalysedBy
     asset_tier: str
+    cluster_entities: list[ClusterEntity]
+    team_id: uuid.UUID
     risk_score: float | None
+    error: str | None
+    workflow_status: str
+    workflow_status_id: int
+    process_status: str
+    process_status_id: int
```

