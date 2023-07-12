# Comparing `tmp/uagents-0.5.0.tar.gz` & `tmp/uagents-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents-0.5.0.tar", max compression
+gzip compressed data, was "uagents-0.5.1.tar", max compression
```

## Comparing `uagents-0.5.0.tar` & `uagents-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.5.0/LICENSE
--rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.5.0/README.md
--rw-r--r--   0        0        0      944 2023-06-15 09:54:04.795393 uagents-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.5.0/src/uagents/__init__.py
--rw-r--r--   0        0        0    16619 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/agent.py
--rw-r--r--   0        0        0     5669 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/asgi.py
--rw-r--r--   0        0        0     2363 2023-06-02 09:42:02.550506 uagents-0.5.0/src/uagents/config.py
--rw-r--r--   0        0        0     5880 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/context.py
--rw-r--r--   0        0        0        0 2023-06-14 08:44:04.646091 uagents-0.5.0/src/uagents/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/contrib/protocols/__init__.py
--rw-r--r--   0        0        0      751 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/contrib/protocols/protocol_query.py
--rw-r--r--   0        0        0     4148 2023-05-22 12:26:05.307659 uagents-0.5.0/src/uagents/crypto/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/dispatch.py
--rw-r--r--   0        0        0     1697 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/envelope.py
--rw-r--r--   0        0        0     6826 2023-06-15 09:54:04.799393 uagents-0.5.0/src/uagents/mailbox.py
--rw-r--r--   0        0        0      464 2023-05-06 15:29:54.115441 uagents-0.5.0/src/uagents/models.py
--rw-r--r--   0        0        0     1737 2023-06-02 09:42:02.554506 uagents-0.5.0/src/uagents/network.py
--rw-r--r--   0        0        0     6661 2023-05-06 15:29:54.115441 uagents-0.5.0/src/uagents/protocol.py
--rw-r--r--   0        0        0     2123 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/query.py
--rw-r--r--   0        0        0     1339 2023-06-02 09:42:02.558506 uagents-0.5.0/src/uagents/resolver.py
--rw-r--r--   0        0        0     1153 2023-05-06 15:29:54.115441 uagents-0.5.0/src/uagents/setup.py
--rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.5.0/src/uagents/storage/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 uagents-0.5.0/setup.py
--rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 uagents-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.5.1/README.md
+-rw-r--r--   0        0        0      944 2023-07-12 12:17:00.590353 uagents-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.5.1/src/uagents/__init__.py
+-rw-r--r--   0        0        0    17768 2023-07-12 12:09:18.215307 uagents-0.5.1/src/uagents/agent.py
+-rw-r--r--   0        0        0     5723 2023-07-12 08:25:20.419397 uagents-0.5.1/src/uagents/asgi.py
+-rw-r--r--   0        0        0     2491 2023-07-12 12:09:18.215307 uagents-0.5.1/src/uagents/config.py
+-rw-r--r--   0        0        0     6304 2023-07-12 12:09:18.215307 uagents-0.5.1/src/uagents/context.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:25:20.419397 uagents-0.5.1/src/uagents/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/contrib/protocols/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/contrib/protocols/protocol_query.py
+-rw-r--r--   0        0        0     4148 2023-07-12 12:09:18.215307 uagents-0.5.1/src/uagents/crypto/__init__.py
+-rw-r--r--   0        0        0     1154 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/dispatch.py
+-rw-r--r--   0        0        0     1697 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/envelope.py
+-rw-r--r--   0        0        0     6826 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/mailbox.py
+-rw-r--r--   0        0        0      464 2023-05-06 15:29:54.115441 uagents-0.5.1/src/uagents/models.py
+-rw-r--r--   0        0        0     5306 2023-07-12 12:09:18.215307 uagents-0.5.1/src/uagents/network.py
+-rw-r--r--   0        0        0     6661 2023-06-21 13:57:23.767799 uagents-0.5.1/src/uagents/protocol.py
+-rw-r--r--   0        0        0     2410 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/query.py
+-rw-r--r--   0        0        0     2661 2023-07-12 08:25:20.423397 uagents-0.5.1/src/uagents/resolver.py
+-rw-r--r--   0        0        0     1153 2023-05-06 15:29:54.115441 uagents-0.5.1/src/uagents/setup.py
+-rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.5.1/src/uagents/storage/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 uagents-0.5.1/setup.py
+-rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 uagents-0.5.1/PKG-INFO
```

### Comparing `uagents-0.5.0/LICENSE` & `uagents-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/README.md` & `uagents-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/pyproject.toml` & `uagents-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uagents"
-version = "0.5.0"
+version = "0.5.1"
 description = "Lightweight framework for rapid agent-based development"
 authors = ["Ed FitzGerald <edward.fitzgerald@fetch.ai>", "James Riehl <james.riehl@fetch.ai>", "Alejandro Morales <alejandro.madrigal@fetch.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `uagents-0.5.0/src/uagents/agent.py` & `uagents-0.5.1/src/uagents/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import asyncio
 import functools
 from typing import Dict, List, Optional, Set, Union, Type, Tuple, Any
 import uuid
 
 from cosmpy.aerial.wallet import LocalWallet, PrivateKey
 from cosmpy.crypto.address import Address
+from cosmpy.aerial.contract.cosmwasm import create_cosmwasm_execute_msg
+from cosmpy.aerial.client import prepare_and_broadcast_basic_transaction
+from cosmpy.aerial.tx import Transaction
+
 
 from uagents.asgi import ASGIServer
 from uagents.context import (
     Context,
     EventCallback,
     IntervalCallback,
     MessageCallback,
     MsgDigest,
 )
 from uagents.crypto import Identity, derive_key_from_seed, is_user_address
 from uagents.dispatch import Sink, dispatcher, JsonStr
 from uagents.models import Model, ErrorMessage
 from uagents.protocol import Protocol
-from uagents.resolver import Resolver, AlmanacResolver
+from uagents.resolver import Resolver, GlobalResolver
 from uagents.storage import KeyValueStore, get_or_create_private_keys
-from uagents.network import get_ledger, get_reg_contract, wait_for_tx_to_complete
+from uagents.network import (
+    get_ledger,
+    get_almanac_contract,
+    get_service_contract,
+    wait_for_tx_to_complete,
+)
 from uagents.mailbox import MailboxClient
 from uagents.config import (
+    CONTRACT_ALMANAC,
     REGISTRATION_FEE,
     REGISTRATION_DENOM,
+    MIN_REGISTRATION_TIME,
     LEDGER_PREFIX,
-    BLOCK_INTERVAL,
     parse_endpoint_config,
     parse_mailbox_config,
     get_logger,
 )
 
 
 async def _run_interval(func: IntervalCallback, ctx: Context, period: float):
@@ -59,34 +69,19 @@
         mailbox: Optional[Union[str, Dict[str, str]]] = None,
         resolve: Optional[Resolver] = None,
         version: Optional[str] = None,
     ):
         self._name = name
         self._port = port if port is not None else 8000
         self._background_tasks: Set[asyncio.Task] = set()
-        self._resolver = resolve if resolve is not None else AlmanacResolver()
+        self._resolver = resolve if resolve is not None else GlobalResolver()
         self._loop = asyncio.get_event_loop_policy().get_event_loop()
 
         # initialize wallet and identity
-        if seed is None:
-            if name is None:
-                self._wallet = LocalWallet.generate()
-                self._identity = Identity.generate()
-            else:
-                identity_key, wallet_key = get_or_create_private_keys(name)
-                self._wallet = LocalWallet(PrivateKey(wallet_key))
-                self._identity = Identity.from_string(identity_key)
-        else:
-            self._identity = Identity.from_seed(seed, 0)
-            self._wallet = LocalWallet(
-                PrivateKey(derive_key_from_seed(seed, LEDGER_PREFIX, 0)),
-                prefix=LEDGER_PREFIX,
-            )
-        if name is None:
-            self._name = self.address[0:16]
+        self._initialize_wallet_and_identity(seed, name)
         self._logger = get_logger(self.name)
 
         # configure endpoints and mailbox
         self._endpoints = parse_endpoint_config(endpoint)
         self._use_mailbox = mailbox is not None
         if self._use_mailbox:
             self._mailbox = parse_mailbox_config(mailbox)
@@ -99,15 +94,16 @@
                 }
             ]
         else:
             self._mailbox = None
             self._mailbox_client = None
 
         self._ledger = get_ledger()
-        self._reg_contract = get_reg_contract()
+        self._almanac_contract = get_almanac_contract()
+        self._service_contract = get_service_contract()
         self._storage = KeyValueStore(self.address[0:16])
         self._interval_handlers: List[Tuple[IntervalCallback, float]] = []
         self._interval_messages: Set[str] = set()
         self._signed_message_handlers: Dict[str, MessageCallback] = {}
         self._unsigned_message_handlers: Dict[str, MessageCallback] = {}
         self._models: Dict[str, Type[Model]] = {}
         self._replies: Dict[str, Set[Type[Model]]] = {}
@@ -143,14 +139,32 @@
         self._dispatcher.register(self.address, self)
 
         if not self._use_mailbox:
             self._server = ASGIServer(
                 self._port, self._loop, self._queries, logger=self._logger
             )
 
+    def _initialize_wallet_and_identity(self, seed, name):
+        if seed is None:
+            if name is None:
+                self._wallet = LocalWallet.generate()
+                self._identity = Identity.generate()
+            else:
+                identity_key, wallet_key = get_or_create_private_keys(name)
+                self._wallet = LocalWallet(PrivateKey(wallet_key))
+                self._identity = Identity.from_string(identity_key)
+        else:
+            self._identity = Identity.from_seed(seed, 0)
+            self._wallet = LocalWallet(
+                PrivateKey(derive_key_from_seed(seed, LEDGER_PREFIX, 0)),
+                prefix=LEDGER_PREFIX,
+            )
+        if name is None:
+            self._name = self.address[0:16]
+
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def address(self) -> str:
         return self._identity.address
@@ -178,17 +192,18 @@
     def sign(self, data: bytes) -> str:
         return self._identity.sign(data)
 
     def sign_digest(self, digest: bytes) -> str:
         return self._identity.sign_digest(digest)
 
     def sign_registration(self) -> str:
-        assert self._reg_contract.address is not None
+        assert self._almanac_contract.address is not None
         return self._identity.sign_registration(
-            str(self._reg_contract.address), self.get_registration_sequence()
+            str(self._almanac_contract.address),
+            self._almanac_contract.get_sequence(self.address),
         )
 
     def update_endpoints(self, endpoints: List[Dict[str, Any]]):
         self._endpoints = endpoints
 
     def update_loop(self, loop):
         self._loop = loop
@@ -204,58 +219,64 @@
                 f"I do not have enough funds to register on Almanac contract\
                     \nFund using wallet address: {self.wallet.address()}"
             )
             return
 
         signature = self.sign_registration()
 
-        msg = {
-            "register": {
-                "record": {
-                    "service": {
-                        "protocols": list(
-                            map(lambda x: x.digest, self.protocols.values())
-                        ),
-                        "endpoints": self._endpoints,
-                    }
-                },
-                "signature": signature,
-                "sequence": self.get_registration_sequence(),
-                "agent_address": self.address,
-            }
-        }
-
-        self._logger.info("Registering on Almanac contract...")
-        transaction = self._reg_contract.execute(
-            msg,
-            ctx.wallet,
-            funds=f"{REGISTRATION_FEE}{REGISTRATION_DENOM}",
+        self._logger.info("Registering on almanac contract...")
+
+        transaction = Transaction()
+
+        almanac_msg = self._almanac_contract.get_registration_msg(
+            self.protocols, self._endpoints, signature, self.address
+        )
+
+        transaction.add_message(
+            create_cosmwasm_execute_msg(
+                ctx.wallet.address(),
+                CONTRACT_ALMANAC,
+                almanac_msg,
+                funds=f"{REGISTRATION_FEE}{REGISTRATION_DENOM}",
+            )
+        )
+
+        transaction = prepare_and_broadcast_basic_transaction(
+            ctx.ledger, transaction, ctx.wallet
         )
         await wait_for_tx_to_complete(transaction.tx_hash)
-        self._logger.info("Registering on Almanac contract...complete")
+        self._logger.info("Registering on almanac contract...complete")
 
     def _schedule_registration(self):
-        query_msg = {"query_records": {"agent_address": self.address}}
-        response = self._reg_contract.query(query_msg)
+        return self._almanac_contract.get_expiry(self.address)
 
-        if not response["record"]:
-            contract_state = self._reg_contract.query({"query_contract_state": {}})
-            expiry = contract_state.get("state").get("expiry_height")
-            return expiry * BLOCK_INTERVAL
+    async def register_name(self):
+        self._logger.info("Registering name...")
 
-        expiry = response.get("record")[0].get("expiry")
-        height = response.get("height")
+        if not self._almanac_contract.is_registered(self.address):
+            self._logger.warning(
+                f"Agent {self.name} needs to be registered in almanac contract to register its name"
+            )
+            return
 
-        return (expiry - height) * BLOCK_INTERVAL
+        transaction = self._service_contract.get_registration_tx(
+            self.name, str(self.wallet.address()), self.address
+        )
 
-    def get_registration_sequence(self) -> int:
-        query_msg = {"query_sequence": {"agent_address": self.address}}
-        sequence = self._reg_contract.query(query_msg)["sequence"]
+        if transaction is None:
+            self._logger.error(
+                f"Please select another name, {self.name} is owned by another address"
+            )
 
-        return sequence
+            return
+        transaction = prepare_and_broadcast_basic_transaction(
+            self._ledger, transaction, self.wallet
+        )
+        await wait_for_tx_to_complete(transaction.tx_hash)
+        self._logger.info("Registering name...complete")
 
     def on_interval(
         self,
         period: float,
         messages: Optional[Union[Type[Model], Set[Type[Model]]]] = None,
     ):
         return self._protocol.on_interval(period, messages)
@@ -360,16 +381,29 @@
         # start the background message queue processor
         task = self._loop.create_task(self._process_message_queue())
         self._background_tasks.add(task)
         task.add_done_callback(self._background_tasks.discard)
 
         # start the contract registration update loop
         if self._endpoints is not None:
-            self._loop.create_task(
-                _run_interval(self._register, self._ctx, self._schedule_registration())
+            if (
+                not self._almanac_contract.is_registered(self.address)
+                or self._schedule_registration() < MIN_REGISTRATION_TIME
+                or self._endpoints != self._almanac_contract.get_endpoints(self.address)
+            ):
+                self._loop.create_task(
+                    _run_interval(
+                        self._register, self._ctx, self._schedule_registration()
+                    )
+                )
+            else:
+                self._logger.info("Registration up to date!")
+        else:
+            self._logger.warning(
+                "I have no endpoint and won't be able to receive external messages"
             )
 
     def run(self):
         self.setup()
         try:
             if self._use_mailbox:
                 self._loop.create_task(self._mailbox_client.process_deletion_queue())
```

### Comparing `uagents-0.5.0/src/uagents/asgi.py` & `uagents-0.5.1/src/uagents/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import pydantic
 import uvicorn
 
 from uagents.config import get_logger
 from uagents.crypto import is_user_address
 from uagents.dispatch import dispatcher
 from uagents.envelope import Envelope
-from uagents.models import Model, ErrorMessage
-from uagents.query import enclose_response
+from uagents.models import ErrorMessage
+from uagents.query import enclose_response_raw
 
 
 HOST = "0.0.0.0"
 
 
 async def _read_asgi_body(receive):
     body = b""
@@ -159,20 +159,22 @@
 
         await dispatcher.dispatch(
             env.sender, env.target, env.schema_digest, env.decode_payload(), env.session
         )
 
         # wait for any queries to be resolved
         if expects_response:
-            response_msg: Model = await self._queries[env.sender]
+            response_msg, schema_digest = await self._queries[env.sender]
             if env.expires is not None:
                 if datetime.now() > datetime.fromtimestamp(env.expires):
                     response_msg = ErrorMessage(error="Query envelope expired")
             sender = env.target
-            response = enclose_response(response_msg, sender, str(env.session))
+            response = enclose_response_raw(
+                response_msg, schema_digest, sender, str(env.session)
+            )
         else:
             response = "{}"
 
         await send(
             {
                 "type": "http.response.start",
                 "status": 200,
```

### Comparing `uagents-0.5.0/src/uagents/config.py` & `uagents-0.5.1/src/uagents/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,20 @@
     FETCHAI_MAINNET = 2
 
 
 AGENT_PREFIX = "agent"
 LEDGER_PREFIX = "fetch"
 USER_PREFIX = "user"
 CONTRACT_ALMANAC = "fetch1tjagw8g8nn4cwuw00cf0m5tl4l6wfw9c0ue507fhx9e3yrsck8zs0l3q4w"
+CONTRACT_NAME_SERVICE = (
+    "fetch1mxz8kn3l5ksaftx8a9pj9a6prpzk2uhxnqdkwuqvuh37tw80xu6qges77l"
+)
 REGISTRATION_FEE = 500000000000000000
 REGISTRATION_DENOM = "atestfet"
+MIN_REGISTRATION_TIME = 3600
 BLOCK_INTERVAL = 5
 AGENT_NETWORK = AgentNetwork.FETCHAI_TESTNET
 
 MAILBOX_SERVER_URL = "wss://agentverse.ai"
 MAILBOX_POLL_INTERVAL_SECONDS = 1.0
 
 DEFAULT_ENVELOPE_TIMEOUT_SECONDS = 30
```

### Comparing `uagents-0.5.0/src/uagents/context.py` & `uagents-0.5.1/src/uagents/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import aiohttp
 from cosmpy.aerial.client import LedgerClient
 from cosmpy.aerial.wallet import LocalWallet
 
 from uagents.config import DEFAULT_ENVELOPE_TIMEOUT_SECONDS
 from uagents.crypto import Identity
-from uagents.dispatch import dispatcher
+from uagents.dispatch import JsonStr, dispatcher
 from uagents.envelope import Envelope
 from uagents.models import Model, ErrorMessage
 from uagents.resolver import Resolver
 from uagents.storage import KeyValueStore
 
 if TYPE_CHECKING:
     from uagents.protocol import Protocol
@@ -99,71 +99,84 @@
 
     async def send(
         self,
         destination: str,
         message: Model,
         timeout: Optional[int] = DEFAULT_ENVELOPE_TIMEOUT_SECONDS,
     ):
-        # convert the message into object form
-        json_message = message.json()
         schema_digest = Model.build_schema_digest(message)
+        await self.send_raw(
+            destination,
+            message.json(),
+            schema_digest,
+            message_type=type(message),
+            timeout=timeout,
+        )
 
+    async def send_raw(
+        self,
+        destination: str,
+        json_message: JsonStr,
+        schema_digest: str,
+        message_type: Optional[Type[Model]] = None,
+        timeout: Optional[int] = DEFAULT_ENVELOPE_TIMEOUT_SECONDS,
+    ):
         # check if this message is a reply
         if (
             self._message_received is not None
             and self._replies
             and schema_digest != ERROR_MESSAGE_DIGEST
         ):
             received = self._message_received
             if received.schema_digest in self._replies:
                 # ensure the reply is valid
                 if schema_digest not in self._replies[received.schema_digest]:
                     self._logger.exception(
-                        f"Outgoing message {type(message)} "
+                        f"Outgoing message {message_type or ''} "
                         f"is not a valid reply to {received.message}"
                     )
                     return
 
         # check if this message is a valid interval message
         if self._message_received is None and self._interval_messages:
             if schema_digest not in self._interval_messages:
                 self._logger.exception(
-                    f"Outgoing message {type(message)} is not a valid interval message"
+                    f"Outgoing message {message_type} is not a valid interval message"
                 )
                 return
 
         # handle local dispatch of messages
         if dispatcher.contains(destination):
             await dispatcher.dispatch(
                 self.address, destination, schema_digest, json_message, self._session
             )
             return
 
         # handle queries waiting for a response
         if destination in self._queries:
-            self._queries[destination].set_result(message)
+            self._queries[destination].set_result((json_message, schema_digest))
             del self._queries[destination]
             return
 
         # resolve the endpoint
-        endpoint = await self._resolver.resolve(destination)
+        destination_address, endpoint = await self._resolver.resolve(destination)
         if endpoint is None:
             self._logger.exception(
                 f"Unable to resolve destination endpoint for address {destination}"
             )
             return
 
         # calculate when envelope expires
         expires = int(time()) + timeout
 
         # handle external dispatch of messages
         env = Envelope(
             version=1,
             sender=self.address,
-            target=destination,
+            target=destination_address,
             session=self._session,
             schema_digest=schema_digest,
             protocol_digest=self.get_message_protocol(schema_digest),
             expires=expires,
         )
         env.encode_payload(json_message)
         env.sign(self._identity)
@@ -172,9 +185,9 @@
             async with session.post(
                 endpoint, headers={"content-type": "application/json"}, data=env.json()
             ) as resp:
                 success = resp.status == 200
 
         if not success:
             self._logger.exception(
-                f"Unable to send envelope to {destination} @ {endpoint}"
+                f"Unable to send envelope to {destination_address} @ {endpoint}"
             )
```

### Comparing `uagents-0.5.0/src/uagents/contrib/protocols/protocol_query.py` & `uagents-0.5.1/src/uagents/contrib/protocols/protocol_query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/crypto/__init__.py` & `uagents-0.5.1/src/uagents/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/dispatch.py` & `uagents-0.5.1/src/uagents/dispatch.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/envelope.py` & `uagents-0.5.1/src/uagents/envelope.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/mailbox.py` & `uagents-0.5.1/src/uagents/mailbox.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/protocol.py` & `uagents-0.5.1/src/uagents/protocol.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/query.py` & `uagents-0.5.1/src/uagents/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,51 +2,52 @@
 from time import time
 from typing import Optional
 
 import aiohttp
 
 from uagents.config import get_logger
 from uagents.crypto import generate_user_address
+from uagents.dispatch import JsonStr
 from uagents.envelope import Envelope
 from uagents.models import Model
-from uagents.resolver import Resolver, AlmanacResolver
+from uagents.resolver import Resolver, GlobalResolver
 
 
 LOGGER = get_logger("query")
 
 
 async def query(
     destination: str,
     message: Model,
     resolver: Optional[Resolver] = None,
     timeout: Optional[int] = 30,
 ) -> Optional[Envelope]:
     if resolver is None:
-        resolver = AlmanacResolver()
+        resolver = GlobalResolver()
 
     # convert the message into object form
     json_message = message.json()
     schema_digest = Model.build_schema_digest(message)
 
     # resolve the endpoint
-    endpoint = await resolver.resolve(destination)
+    destination_address, endpoint = await resolver.resolve(destination)
     if endpoint is None:
         LOGGER.exception(
             f"Unable to resolve destination endpoint for address {destination}"
         )
         return
 
     # calculate when envelope expires
     expires = int(time()) + timeout
 
     # handle external dispatch of messages
     env = Envelope(
         version=1,
         sender=generate_user_address(),
-        target=destination,
+        target=destination_address,
         session=uuid.uuid4(),
         schema_digest=schema_digest,
         expires=expires,
     )
     env.encode_payload(json_message)
 
     async with aiohttp.ClientSession() as session:
@@ -64,16 +65,23 @@
             if success:
                 return Envelope.parse_obj(await resp.json())
 
     LOGGER.exception(f"Unable to query {destination} @ {endpoint}")
 
 
 def enclose_response(message: Model, sender: str, session: str) -> str:
+    schema_digest = Model.build_schema_digest(message)
+    return enclose_response_raw(message.json(), schema_digest, sender, session)
+
+
+def enclose_response_raw(
+    json_message: JsonStr, schema_digest: str, sender: str, session: str
+) -> str:
     response_env = Envelope(
         version=1,
         sender=sender,
         target="",
         session=session,
-        schema_digest=Model.build_schema_digest(message),
+        schema_digest=schema_digest,
     )
-    response_env.encode_payload(message.json())
+    response_env.encode_payload(json_message)
     return response_env.json()
```

### Comparing `uagents-0.5.0/src/uagents/resolver.py` & `uagents-0.5.1/src/uagents/resolver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,86 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Optional
 import random
 
-from uagents.network import get_reg_contract
+from uagents.network import get_almanac_contract, get_service_contract
 
 
-def _query_record(agent_address: str, service: str) -> dict:
-    contract = get_reg_contract()
+def query_record(agent_address: str, service: str) -> dict:
+    contract = get_almanac_contract()
     query_msg = {
         "query_record": {"agent_address": agent_address, "record_type": service}
     }
     result = contract.query(query_msg)
     return result
 
 
+def get_agent_address(name: str) -> str:
+    query_msg = {"domain_record": {"domain": f"{name}.agent"}}
+    result = get_service_contract().query(query_msg)
+    if result["record"] is not None:
+        registered_address = result["record"]["records"][0]["agent_address"]["records"]
+        if len(registered_address) > 0:
+            return registered_address[0]["address"]
+        return 0
+    return 1
+
+
+def is_agent_address(address):
+    if not isinstance(address, str):
+        return False
+
+    prefix = "agent"
+    expected_length = 65
+
+    return address.startswith(prefix) and len(address) == expected_length
+
+
 class Resolver(ABC):
     @abstractmethod
-    async def resolve(self, address: str) -> Optional[str]:
+    async def resolve(self, destination: str) -> Optional[str]:
         pass
 
 
+class GlobalResolver(Resolver):
+    async def resolve(self, destination: str) -> Optional[str]:
+        almanac_resolver = AlmanacResolver()
+        name_service_resolver = NameServiceResolver()
+        address = (
+            destination
+            if is_agent_address(destination)
+            else await name_service_resolver.resolve(destination)
+        )
+
+        if is_agent_address(address):
+            return await almanac_resolver.resolve(address)
+        return None, None
+
+
 class AlmanacResolver(Resolver):
-    async def resolve(self, address: str) -> Optional[str]:
-        result = _query_record(address, "service")
+    async def resolve(self, destination: str) -> Optional[str]:
+        result = query_record(destination, "service")
         if result is not None:
             record = result.get("record") or {}
             endpoint_list = (
                 record.get("record", {}).get("service", {}).get("endpoints", [])
             )
 
             if len(endpoint_list) > 0:
                 endpoints = [val.get("url") for val in endpoint_list]
                 weights = [val.get("weight") for val in endpoint_list]
-                return random.choices(endpoints, weights=weights)[0]
-        return None
+                return destination, random.choices(endpoints, weights=weights)[0]
+
+        return None, None
+
+
+class NameServiceResolver(Resolver):
+    async def resolve(self, destination: str) -> Optional[str]:
+        return get_agent_address(destination)
 
 
 class RulesBasedResolver(Resolver):
     def __init__(self, rules: Dict[str, str]):
         self._rules = rules
 
-    async def resolve(self, address: str) -> Optional[str]:
-        return self._rules.get(address)
+    async def resolve(self, destination: str) -> Optional[str]:
+        return self._rules.get(destination)
```

### Comparing `uagents-0.5.0/src/uagents/setup.py` & `uagents-0.5.1/src/uagents/setup.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/src/uagents/storage/__init__.py` & `uagents-0.5.1/src/uagents/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.5.0/setup.py` & `uagents-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'msgpack>=1.0.4,<2.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'uvicorn>=0.19.0,<0.20.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'uagents',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Lightweight framework for rapid agent-based development',
     'long_description': 'The **μAgents** (micro-Agents) project is a fast and lightweight framework that makes it easy to build agents for all kinds of decentralised use cases.\n\n## Installation\n\nInstall μAgents for Python 3.8, 3.9, or 3.10:\n\n```bash\npoetry install\npoetry shell\n```\n\n## Documentation\n\nBuild and run the docs locally with:\n\n```bash\nmkdocs serve\n```\n\nOr go to the official docs site: https://docs.fetch.ai/uAgents.\n\n## Examples\n\nThe [`examples`](https://github.com/fetchai/uAgents/tree/main/examples) folder contains several examples of how to create and run various types of agents.\n\n## Contributing\n\nAll contributions are welcome! Remember, contribution includes not only code, but any help with docs or issues raised by other developers. See our [contribution guidelines](https://github.com/fetchai/uAgents/blob/main/CONTRIBUTING.md) for more details.\n\n### Development Guidelines\n\nRead our [development guidelines](https://github.com/fetchai/uAgents/blob/main/DEVELOPING.md) to learn some useful tips related to development.\n\n### Issues, Questions and Discussions\n\nWe use [GitHub Issues](https://github.com/fetchai/uAgents/issues) for tracking requests and bugs, and [GitHub Discussions](https://github.com/fetchai/uAgents/discussions) for general questions and discussion.\n\n## License\n\nThe μAgents project is licensed under [Apache License 2.0](https://github.com/fetchai/uAgents/blob/main/LICENSE).\n\n',
     'author': 'Ed FitzGerald',
     'author_email': 'edward.fitzgerald@fetch.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `uagents-0.5.0/PKG-INFO` & `uagents-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lightweight framework for rapid agent-based development
 License: Apache 2.0
 Author: Ed FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

