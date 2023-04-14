# Comparing `tmp/inpost-0.0.7.tar.gz` & `tmp/inpost-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.0.7.tar", max compression
+gzip compressed data, was "inpost-0.0.8.tar", max compression
```

## Comparing `inpost-0.0.7.tar` & `inpost-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       31 2023-01-08 12:39:56.709189 inpost-0.0.7/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.0.7/inpost/__init__.py
--rw-r--r--   0        0        0    48756 2023-03-04 13:36:20.317795 inpost-0.0.7/inpost/api.py
--rw-r--r--   0        0        0     1090 2023-03-04 13:33:30.719374 inpost-0.0.7/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.0.7/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.0.7/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.0.7/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.0.7/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.0.7/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.0.7/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.0.7/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0     1771 2023-03-04 13:33:30.709374 inpost-0.0.7/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.0.7/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.0.7/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.0.7/inpost/static/headers.py
--rw-r--r--   0        0        0    25234 2023-02-01 10:22:10.763474 inpost-0.0.7/inpost/static/parcels.py
--rw-r--r--   0        0        0     6871 2023-03-04 12:24:05.776170 inpost-0.0.7/inpost/static/statuses.py
--rw-r--r--   0        0        0     1026 2023-03-04 14:11:36.407651 inpost-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 inpost-0.0.7/setup.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 inpost-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-01-08 12:39:56.709189 inpost-0.0.8/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.0.8/inpost/__init__.py
+-rw-r--r--   0        0        0    48840 2023-04-14 09:52:35.751540 inpost-0.0.8/inpost/api.py
+-rw-r--r--   0        0        0     1105 2023-04-14 08:22:00.444589 inpost-0.0.8/inpost/static/__init__.py
+-rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.0.8/inpost/static/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.0.8/inpost/static/__pycache__/endpoints.cpython-310.pyc
+-rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.0.8/inpost/static/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.0.8/inpost/static/__pycache__/friends.cpython-310.pyc
+-rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.0.8/inpost/static/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.0.8/inpost/static/__pycache__/parcels.cpython-310.pyc
+-rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.0.8/inpost/static/__pycache__/statuses.cpython-310.pyc
+-rw-r--r--   0        0        0     1771 2023-03-04 13:33:30.709374 inpost-0.0.8/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.0.8/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.0.8/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.0.8/inpost/static/headers.py
+-rw-r--r--   0        0        0    27154 2023-04-14 08:23:52.935000 inpost-0.0.8/inpost/static/parcels.py
+-rw-r--r--   0        0        0     7066 2023-04-14 08:22:00.461255 inpost-0.0.8/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1026 2023-04-14 09:59:13.882104 inpost-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 inpost-0.0.8/setup.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 inpost-0.0.8/PKG-INFO
```

### Comparing `inpost-0.0.7/inpost/api.py` & `inpost-0.0.8/inpost/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -958,14 +958,15 @@
         self._log.info(f'sharing parcel: {shipment_number}')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
         async with await self.sess.post(url=shared,
+                                        headers={'Authorization': self.auth_token},
                                         json={
                                             'parcels': [
                                                 {
                                                     'shipmentNumber': shipment_number,
                                                     'friendUuids': [
                                                         uuid
                                                     ]
```

### Comparing `inpost-0.0.7/inpost/static/__init__.py` & `inpost-0.0.8/inpost/static/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .parcels import Parcel, Receiver, Sender, PickupPoint, MultiCompartment, Operations, EventLog, SharedTo, \
     QRCode, CompartmentLocation, CompartmentProperties
 from .headers import appjson
 from .statuses import ParcelCarrierSize, ParcelLockerSize, ParcelDeliveryType, ParcelShipmentType, \
     ParcelAdditionalInsurance, ParcelType, ParcelOwnership, CompartmentExpectedStatus, CompartmentActualStatus, \
-    ParcelServiceName, ParcelStatus
+    ParcelServiceName, ParcelStatus, ReturnsStatus
 from .exceptions import NoParcelError, UnidentifiedParcelError, ParcelTypeError, NotAuthenticatedError, ReAuthenticationError, \
     PhoneNumberError, SmsCodeError, RefreshTokenError, UnidentifiedAPIError, UserLocationError, \
     UnidentifiedError, NotFoundError, UnauthorizedError, SingleParamError, MissingParamsError
 from .endpoints import login, send_sms_code, confirm_sms_code, refresh_token, parcels, parcel, collect, \
     compartment_open, compartment_status, terminate_collect_session, friendship, shared, sent, returns, parcel_prices, \
     tickets, logout, multi, validate_friendship, accept_friendship
 from .friends import Friend
```

### Comparing `inpost-0.0.7/inpost/static/__pycache__/__init__.cpython-310.pyc` & `inpost-0.0.8/inpost/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/__pycache__/endpoints.cpython-310.pyc` & `inpost-0.0.8/inpost/static/__pycache__/endpoints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/__pycache__/exceptions.cpython-310.pyc` & `inpost-0.0.8/inpost/static/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/__pycache__/friends.cpython-310.pyc` & `inpost-0.0.8/inpost/static/__pycache__/friends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/__pycache__/parcels.cpython-310.pyc` & `inpost-0.0.8/inpost/static/__pycache__/parcels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/__pycache__/statuses.cpython-310.pyc` & `inpost-0.0.8/inpost/static/__pycache__/statuses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/endpoints.py` & `inpost-0.0.8/inpost/static/endpoints.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/exceptions.py` & `inpost-0.0.8/inpost/static/exceptions.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/friends.py` & `inpost-0.0.8/inpost/static/friends.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.7/inpost/static/parcels.py` & `inpost-0.0.8/inpost/static/parcels.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,46 +5,60 @@
 
 import qrcode
 from arrow import get, arrow
 
 from inpost.static.statuses import *
 
 
-class Parcel:
+class BaseParcel:
+    def __init__(self, parcel_data: dict, logger: logging.Logger):
+        self.shipment_number: str = parcel_data['shipmentNumber']
+        self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
+        self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
+        # self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
+        #     if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
+        self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
+        self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
+        self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
+                                          for event in parcel_data['eventLog']]
+
+
+class Parcel(BaseParcel):
     """Object representation of :class:`inpost.api.Inpost` compartment properties
 
     :param parcel_data: :class:`dict` containing all parcel data
     :type parcel_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         """Constructor method"""
-        self.shipment_number: str = parcel_data['shipmentNumber']
+        super().__init__(parcel_data, logger)
+        # self.shipment_number: str = parcel_data['shipmentNumber']
         self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
         self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data['shipmentType']]
         self._open_code: str | None = parcel_data['openCode'] if 'openCode' in parcel_data else None
         self._qr_code: QRCode | None = QRCode(qrcode_data=parcel_data['qrCode'], logger=self._log) \
             if 'qrCode' in parcel_data else None
         self.stored_date: arrow | None = get(parcel_data['storedDate']) if 'storedDate' in parcel_data else None
         self.pickup_date: arrow | None = get(parcel_data['pickUpDate']) if 'pickUpDate' in parcel_data else None
-        self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
+        # self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
         self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
             if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
         self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log)
         self.sender: Sender = Sender(sender_data=parcel_data['sender'], logger=self._log)
         self.pickup_point: PickupPoint = PickupPoint(pickuppoint_data=parcel_data['pickUpPoint'], logger=self._log) \
             if 'pickUpPoint' in parcel_data else None
         self.multi_compartment: MultiCompartment | None = MultiCompartment(
             parcel_data['multiCompartment'], logger=self._log) if 'multiCompartment' in parcel_data else None
         self.is_end_off_week_collection: bool = parcel_data['endOfWeekCollection']
-        self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
+        # self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
         self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
-        self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
-                                          for event in parcel_data['eventLog']]
+        # self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
+        #                                   for event in parcel_data['eventLog']]
         self.avizo_transaction_status: str = parcel_data['avizoTransactionStatus']
         self.shared_to: List[SharedTo] = [SharedTo(sharedto_data=person, logger=self._log)
                                           for person in parcel_data['sharedTo']]
         self.ownership_status: ParcelOwnership = ParcelOwnership[parcel_data['ownershipStatus']]
         self._compartment_properties: CompartmentProperties | None = None
 
         self._log.debug(f'created parcel with shipment number {self.shipment_number}')
@@ -232,14 +246,32 @@
         return None
 
     # @property
     # def get_from_multicompartment(self):
     #     return
 
 
+class ReturnParcel(BaseParcel):
+    def __init__(self, parcel_data: dict, logger: logging.Logger):
+        super().__init__(parcel_data, logger)
+        self.uuid: str = parcel_data['uuid']
+        self.rma: str = parcel_data['rma']
+        self.organization_name: str = parcel_data['organizationName']
+        self.created_date: arrow = parcel_data['createdDate']
+        self.accepted_date: arrow = parcel_data['acceptedDate']
+        self.expiry_date: arrow = parcel_data['expiryDate']
+        self.sent_date: arrow = parcel_data['sentDate']
+        self.delivered_date: arrow = parcel_data['deliveredDate']
+        self.order_number: str = parcel_data['orderNumber']
+        self.form_type: str = parcel_data['formType']
+
+
+
+
+
 class Receiver:
     """Object representation of :class:`Parcel` receiver
 
     :param receiver_data: :class:`dict` containing sender data for :class:`Parcel`
     :type receiver_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
@@ -376,14 +408,15 @@
         self.highlight: bool = operations_data['highlight']
         self.refresh_until: arrow = get(operations_data['refreshUntil'])
         self.request_easy_access_zone: str = operations_data['requestEasyAccessZone']
         self.is_voicebot: bool = operations_data['voicebot']
         self.can_share_to_observe: bool = operations_data['canShareToObserve']
         self.can_share_open_code: bool = operations_data['canShareOpenCode']
         self.can_share_parcel: bool = operations_data['canShareParcel']
+        self.send: bool = operations_data['send']
 
         self._log: logging.Logger = logger.getChild(__class__.__name__)
         self._log.debug('created')
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
@@ -396,22 +429,22 @@
     :type eventlog_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, eventlog_data: dict, logger: logging.Logger):
         """Constructor method"""
         self.type: str = eventlog_data['type']
-        self.name: ParcelStatus = ParcelStatus[eventlog_data['name']]
+        self.name: ParcelStatus | ReturnsStatus = ParcelStatus[eventlog_data['name']] if self.type == 'PARCEL_STATUS' else ReturnsStatus[eventlog_data['name']]
         self.date: arrow = get(eventlog_data['date'])
 
         self._log: logging.Logger = logger.getChild(__class__.__name__)
         self._log.debug('created')
 
-        if self.name == ParcelStatus.UNKNOWN:
-            self._log.debug(f'unknown parcel status: {eventlog_data["name"]}')
+        if self.name == ParcelStatus.UNKNOWN or self.name == ReturnsStatus.UNKNOWN:
+            self._log.debug(f'unknown {self.type}: {eventlog_data["name"]}')
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
 
 
 class SharedTo:
```

### Comparing `inpost-0.0.7/inpost/static/statuses.py` & `inpost-0.0.8/inpost/static/statuses.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,21 @@
     PICKUP_REMINDER_SENT_ADDRESS = 'Wysłano przypomnienie o odbiorze'  # TODO: translate from app
     UNDELIVERED_WRONG_ADDRESS = 'Nie dostarczono z powodu złego adresu'  # TODO: translate from app
     UNDELIVERED_COD_CASH_RECEIVER = 'Nie dostarczono z powodu nieopłacenia'  # TODO: translate from app
     REDIRECT_TO_BOX = 'Przekierowana do paczkomatu'  # TODO: translate from app
     CANCELED_REDIRECT_TO_BOX = 'Anulowano przekierowanie do paczkomatu'  # TODO: translate from app
 
 
+class ReturnsStatus(ParcelBase):  # TODO: translate from app and fill missing ones
+    ACCEPTED = 'Zaakceptowano'
+    USED = 'Nadano'
+    DELIVERED = 'Dostarczono'
+    UNKNOWN = 'UNKNOWN DATA'
+
+
 class ParcelOwnership(ParcelBase):
     """:class:`Enum` that holds parcel ownership types"""
     UNKNOWN = 'UNKNOWN DATA'
     FRIEND = 'Zaprzyjaźniona'
     OWN = 'Własna'
```

### Comparing `inpost-0.0.7/pyproject.toml` & `inpost-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inpost"
-version = "0.0.7"
+version = "0.0.8"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
```

### Comparing `inpost-0.0.7/setup.py` & `inpost-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.4.0,<10.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'arrow>=1.2.3,<2.0.0',
  'qrcode>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'inpost',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app',
     'long_description': 'Fully async Inpost API library\n',
     'author': 'loboda4450',
     'author_email': 'loboda4450@gmail.com',
     'maintainer': 'loboda4450',
     'maintainer_email': 'loboda4450@gmail.com',
     'url': 'https://github.com/IFOSSA/inpost-python',
```

### Comparing `inpost-0.0.7/PKG-INFO` & `inpost-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.0.7
+Version: 0.0.8
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
```

