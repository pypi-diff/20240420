# Comparing `tmp/fleece_network-0.2.0rc3.tar.gz` & `tmp/fleece_network-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleece_network-0.2.0rc3.tar", max compression
+gzip compressed data, was "fleece_network-0.2.1.tar", max compression
```

## Comparing `fleece_network-0.2.0rc3.tar` & `fleece_network-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      327 2024-04-12 12:24:35.837670 fleece_network-0.2.0rc3/README.md
--rw-r--r--   0        0        0        0 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/__init__.py
--rw-r--r--   0        0        0      349 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/candidate.py
--rw-r--r--   0        0        0    41823 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/ice.py
--rw-r--r--   0        0        0     6655 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/mdns.py
--rw-r--r--   0        0        0    12369 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/stun.py
--rw-r--r--   0        0        0    15077 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/turn.py
--rw-r--r--   0        0        0      264 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/utils.py
--rw-r--r--   0        0        0     1226 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/__init__.py
--rw-r--r--   0        0        0      824 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/clock.py
--rw-r--r--   0        0        0      180 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/exceptions.py
--rw-r--r--   0        0        0    21027 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rate.py
--rw-r--r--   0        0        0     1040 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcconfiguration.py
--rw-r--r--   0        0        0     6531 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdatachannel.py
--rw-r--r--   0        0        0    13595 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdtlstransport.py
--rw-r--r--   0        0        0    11425 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcicetransport.py
--rw-r--r--   0        0        0    32180 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcpeerconnection.py
--rw-r--r--   0        0        0     4612 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcrtpparameters.py
--rw-r--r--   0        0        0    61924 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcsctptransport.py
--rw-r--r--   0        0        0      500 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcsessiondescription.py
--rw-r--r--   0        0        0    24050 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtp.py
--rw-r--r--   0        0        0    21763 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/sdp.py
--rw-r--r--   0        0        0     2879 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/stats.py
--rw-r--r--   0        0        0      978 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/utils.py
--rw-r--r--   0        0        0      716 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/messages.py
--rw-r--r--   0        0        0    21803 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/peer.py
--rw-r--r--   0        0        0        0 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/py.typed
--rw-r--r--   0        0        0     2144 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/signaling.py
--rw-r--r--   0        0        0      479 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      327 2024-04-19 14:14:38.305768 fleece_network-0.2.1/README.md
+-rw-r--r--   0        0        0       66 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/candidate.py
+-rw-r--r--   0        0        0    41823 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/ice.py
+-rw-r--r--   0        0        0     6655 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/mdns.py
+-rw-r--r--   0        0        0    12369 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/stun.py
+-rw-r--r--   0        0        0    15054 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/turn.py
+-rw-r--r--   0        0        0      264 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aioice/utils.py
+-rw-r--r--   0        0        0     1375 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/clock.py
+-rw-r--r--   0        0        0      180 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/exceptions.py
+-rw-r--r--   0        0        0    21027 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rate.py
+-rw-r--r--   0        0        0     1040 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rtcconfiguration.py
+-rw-r--r--   0        0        0     6531 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rtcdatachannel.py
+-rw-r--r--   0        0        0    13289 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rtcdtlstransport.py
+-rw-r--r--   0        0        0    11425 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rtcicetransport.py
+-rw-r--r--   0        0        0    31914 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rtcpeerconnection.py
+-rw-r--r--   0        0        0     4612 2024-04-19 14:14:38.305768 fleece_network-0.2.1/fleece_network/aiortc/rtcrtpparameters.py
+-rw-r--r--   0        0        0    61882 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/aiortc/rtcsctptransport.py
+-rw-r--r--   0        0        0      500 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/aiortc/rtcsessiondescription.py
+-rw-r--r--   0        0        0    24050 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/aiortc/rtp.py
+-rw-r--r--   0        0        0    21790 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/aiortc/sdp.py
+-rw-r--r--   0        0        0     2879 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/aiortc/stats.py
+-rw-r--r--   0        0        0      978 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/aiortc/utils.py
+-rw-r--r--   0        0        0      718 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/messages.py
+-rw-r--r--   0        0        0    21922 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/peer.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/py.typed
+-rw-r--r--   0        0        0      641 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/sede.py
+-rw-r--r--   0        0        0     2150 2024-04-19 14:14:38.309768 fleece_network-0.2.1/fleece_network/signaling.py
+-rw-r--r--   0        0        0      619 2024-04-19 14:14:38.309768 fleece_network-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fleece_network-0.2.1/PKG-INFO
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aioice/candidate.py` & `fleece_network-0.2.1/fleece_network/aioice/candidate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aioice/ice.py` & `fleece_network-0.2.1/fleece_network/aioice/ice.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import enum
 import ipaddress
 import logging
 import random
 import secrets
 import socket
 import threading
-from itertools import count
 import time
+from itertools import count
 from typing import Dict, List, Optional, Set, Text, Tuple, Union, cast
 
 import ifaddr
 
 from . import mdns, stun, turn
 from .candidate import Candidate, candidate_foundation, candidate_priority
 from .utils import random_string
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aioice/mdns.py` & `fleece_network-0.2.1/fleece_network/aioice/mdns.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aioice/stun.py` & `fleece_network-0.2.1/fleece_network/aioice/stun.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from abc import abstractmethod
 import asyncio
 import binascii
 import enum
 import hmac
 import ipaddress
+import time
+from abc import abstractmethod
 from collections import OrderedDict
 from struct import pack, unpack
-import time
 from typing import Callable, Dict, List, Optional, Protocol, Tuple
 
 from .utils import random_transaction_id
 
 COOKIE = 0x2112A442
 FINGERPRINT_LENGTH = 8
 FINGERPRINT_XOR = 0x5354554E
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aioice/turn.py` & `fleece_network-0.2.1/fleece_network/aioice/turn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-import traceback
 import asyncio
 import hashlib
 import logging
 import socket
 import struct
 import time
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Text,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
+import traceback
+from typing import (Any, Callable, Dict, List, Optional, Text, Tuple, TypeVar,
+                    Union, cast)
 
 from . import stun
 from .utils import random_transaction_id
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_CHANNEL_REFRESH_TIME = 500
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/__init__.py` & `fleece_network-0.2.1/fleece_network/aiortc/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,27 @@
 # ruff: noqa: F401
 import logging
 
 from .exceptions import InvalidAccessError, InvalidStateError
 from .rtcconfiguration import RTCConfiguration, RTCIceServer
 from .rtcdatachannel import RTCDataChannel, RTCDataChannelParameters
-from .rtcdtlstransport import (
-    RTCCertificate,
-    RTCDtlsFingerprint,
-    RTCDtlsParameters,
-    RTCDtlsTransport,
-)
-from .rtcicetransport import (
-    RTCIceCandidate,
-    RTCIceGatherer,
-    RTCIceParameters,
-    RTCIceTransport,
-)
+from .rtcdtlstransport import (RTCCertificate, RTCDtlsFingerprint,
+                               RTCDtlsParameters, RTCDtlsTransport)
+from .rtcicetransport import (RTCIceCandidate, RTCIceGatherer,
+                              RTCIceParameters, RTCIceTransport)
 from .rtcpeerconnection import RTCPeerConnection
-from .rtcrtpparameters import (
-    RTCRtcpParameters,
-    RTCRtpCapabilities,
-    RTCRtpCodecCapability,
-    RTCRtpCodecParameters,
-    RTCRtpHeaderExtensionCapability,
-    RTCRtpHeaderExtensionParameters,
-    RTCRtpParameters,
-)
+from .rtcrtpparameters import (RTCRtcpParameters, RTCRtpCapabilities,
+                               RTCRtpCodecCapability, RTCRtpCodecParameters,
+                               RTCRtpHeaderExtensionCapability,
+                               RTCRtpHeaderExtensionParameters,
+                               RTCRtpParameters)
 from .rtcsctptransport import RTCSctpCapabilities, RTCSctpTransport
 from .rtcsessiondescription import RTCSessionDescription
-from .stats import (
-    RTCInboundRtpStreamStats,
-    RTCOutboundRtpStreamStats,
-    RTCRemoteInboundRtpStreamStats,
-    RTCRemoteOutboundRtpStreamStats,
-    RTCStatsReport,
-    RTCTransportStats,
-)
+from .stats import (RTCInboundRtpStreamStats, RTCOutboundRtpStreamStats,
+                    RTCRemoteInboundRtpStreamStats,
+                    RTCRemoteOutboundRtpStreamStats, RTCStatsReport,
+                    RTCTransportStats)
 
 __version__ = "1.8.0"
 
 # Set default logging handler to avoid "No handler found" warnings.
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/clock.py` & `fleece_network-0.2.1/fleece_network/aiortc/clock.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rate.py` & `fleece_network-0.2.1/fleece_network/aiortc/rate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcconfiguration.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcconfiguration.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdatachannel.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcdatachannel.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdtlstransport.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcdtlstransport.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,41 +2,28 @@
 import binascii
 import datetime
 import enum
 import logging
 import os
 import traceback
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Set, Type, TypeVar
-import pylibsrtp
+from typing import TYPE_CHECKING, List, Optional, Type, TypeVar
+
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from OpenSSL import SSL, crypto
 from pyee.asyncio import AsyncIOEventEmitter
-from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .rtcsctptransport import RTCSctpTransport
 
 from . import clock, rtp
 from .rtcicetransport import RTCIceTransport
-from .rtcrtpparameters import RTCRtpReceiveParameters, RTCRtpSendParameters
-from .rtp import (
-    AnyRtcpPacket,
-    RtcpByePacket,
-    RtcpPacket,
-    RtcpPsfbPacket,
-    RtcpRrPacket,
-    RtcpRtpfbPacket,
-    RtcpSrPacket,
-    RtpPacket,
-    is_rtcp,
-)
 from .stats import RTCStatsReport, RTCTransportStats
 
 CERTIFICATE_T = TypeVar("CERTIFICATE_T", bound="RTCCertificate")
 
 logger = logging.getLogger(__name__)
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcicetransport.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcicetransport.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import logging
 import re
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
-from ..aioice import Candidate, Connection, ConnectionClosed
 from pyee.asyncio import AsyncIOEventEmitter
 
+from ..aioice import Candidate, Connection, ConnectionClosed
 from .exceptions import InvalidStateError
 from .rtcconfiguration import RTCIceServer
 
 STUN_REGEX = re.compile(
     r"(?P<scheme>stun|stuns)\:(?P<host>[^?:]+)(\:(?P<port>[0-9]+?))?"
     # RFC 7064 does not define a "transport" option but some providers
     # include it, so just ignore it
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcpeerconnection.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcpeerconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,25 @@
 import asyncio
-import copy
 import logging
 import uuid
-from typing import Any, Dict, List, Optional, Set, Union
+from typing import Any, Dict, List, Optional, Set
 
 from pyee.asyncio import AsyncIOEventEmitter
 
-from . import clock, rtp, sdp
-from .exceptions import (
-    InternalError,
-    InvalidAccessError,
-    InvalidStateError,
-    OperationError,
-)
+from . import clock, sdp
+from .exceptions import InternalError, InvalidStateError
 from .rtcconfiguration import RTCConfiguration
 from .rtcdatachannel import RTCDataChannel, RTCDataChannelParameters
-from .rtcdtlstransport import RTCCertificate, RTCDtlsParameters, RTCDtlsTransport
-from .rtcicetransport import (
-    RTCIceCandidate,
-    RTCIceGatherer,
-    RTCIceParameters,
-    RTCIceTransport,
-)
-from .rtcrtpparameters import (
-    RTCRtpCodecCapability,
-    RTCRtpCodecParameters,
-    RTCRtpDecodingParameters,
-    RTCRtpHeaderExtensionParameters,
-    RTCRtpParameters,
-    RTCRtpReceiveParameters,
-    RTCRtpRtxParameters,
-    RTCRtpSendParameters,
-)
+from .rtcdtlstransport import (RTCCertificate, RTCDtlsParameters,
+                               RTCDtlsTransport)
+from .rtcicetransport import (RTCIceCandidate, RTCIceGatherer,
+                              RTCIceParameters, RTCIceTransport)
+from .rtcrtpparameters import RTCRtpHeaderExtensionParameters
 from .rtcsctptransport import RTCSctpTransport
 from .rtcsessiondescription import RTCSessionDescription
-from .stats import RTCStatsReport
 
 DISCARD_HOST = "0.0.0.0"
 DISCARD_PORT = 9
 MEDIA_KINDS = ["audio", "video"]
 
 logger = logging.getLogger(__name__)
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcrtpparameters.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcsctptransport.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtcsctptransport.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,29 +4,18 @@
 import logging
 import math
 import os
 import time
 from collections import deque
 from dataclasses import dataclass, field
 from struct import pack, unpack_from
-from typing import (
-    Any,
-    Callable,
-    Deque,
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    cast,
-    no_type_check,
-)
+from typing import (Any, Callable, Deque, Dict, Iterator, List, Optional, Set,
+                    Tuple, cast, no_type_check)
 
-from google_crc32c import value as crc32c # type: ignore
+from google_crc32c import value as crc32c  # type: ignore
 from pyee.asyncio import AsyncIOEventEmitter
 
 from .exceptions import InvalidStateError
 from .rtcdatachannel import RTCDataChannel, RTCDataChannelParameters
 from .rtcdtlstransport import RTCDtlsTransport
 from .utils import random32, uint16_add, uint16_gt, uint32_gt, uint32_gte
 
@@ -495,18 +484,18 @@
 
 
 class InboundStream:
     def __init__(self) -> None:
         self.reassembly: List[DataChunk] = []
         self.sequence_number = 0
         self.has_last = False
-    
-    def check_last(self, flags: int): 
-        if flags & SCTP_DATA_LAST_FRAG: 
-            self.has_last = True 
+
+    def check_last(self, flags: int):
+        if flags & SCTP_DATA_LAST_FRAG:
+            self.has_last = True
 
     def add_chunk(self, chunk: DataChunk) -> None:
         if not self.reassembly or uint32_gt(chunk.tsn, self.reassembly[-1].tsn):
             self.check_last(chunk.flags)
             self.reassembly.append(chunk)
             return
 
@@ -517,16 +506,16 @@
 
             if uint32_gt(rchunk.tsn, chunk.tsn):
                 self.check_last(chunk.flags)
                 self.reassembly.insert(i, chunk)
                 break
 
     def pop_messages(self) -> Iterator[Tuple[int, int, bytes]]:
-        if not self.has_last: 
-            return 
+        if not self.has_last:
+            return
         pos = 0
         start_pos = None
         while pos < len(self.reassembly):
             chunk = self.reassembly[pos]
             if start_pos is None:
                 ordered = not (chunk.flags & SCTP_DATA_UNORDERED)
                 if not (chunk.flags & SCTP_DATA_FIRST_FRAG):
@@ -558,15 +547,15 @@
                     self.sequence_number = uint16_add(self.sequence_number, 1)
                 pos = start_pos
                 yield (chunk.stream_id, chunk.protocol, user_data)
             else:
                 pos += 1
 
             expected_tsn = tsn_plus_one(expected_tsn)
-        
+
         self.has_last = False
 
     def prune_chunks(self, tsn: int) -> int:
         """
         Prune chunks up to the given TSN.
         """
         pos = -1
@@ -965,15 +954,15 @@
         elif (
             isinstance(chunk, ReconfigChunk)
             and self._association_state == self.State.ESTABLISHED
         ):
             for param in chunk.params:
                 cls = RECONFIG_PARAM_TYPES.get(param[0])
                 if cls:
-                    await self._receive_reconfig_param(cls.parse(param[1])) # type: ignore
+                    await self._receive_reconfig_param(cls.parse(param[1]))  # type: ignore
 
         # server
         elif isinstance(chunk, InitChunk) and self.is_server:
             self._last_received_tsn = tsn_minus_one(chunk.initial_tsn)
             self._reconfig_response_seq = tsn_minus_one(chunk.initial_tsn)
             self._remote_verification_tag = chunk.initiate_tag
             self._ssthresh = chunk.advertised_rwnd
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/rtp.py` & `fleece_network-0.2.1/fleece_network/aiortc/rtp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/sdp.py` & `fleece_network-0.2.1/fleece_network/aiortc/sdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 import re
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from . import rtp
 from .rtcdtlstransport import RTCDtlsFingerprint, RTCDtlsParameters
 from .rtcicetransport import RTCIceCandidate, RTCIceParameters
-from .rtcrtpparameters import (
-    ParametersDict,
-    RTCRtcpFeedback,
-    RTCRtpCodecParameters,
-    RTCRtpHeaderExtensionParameters,
-    RTCRtpParameters,
-)
+from .rtcrtpparameters import (ParametersDict, RTCRtcpFeedback,
+                               RTCRtpCodecParameters,
+                               RTCRtpHeaderExtensionParameters,
+                               RTCRtpParameters)
 from .rtcsctptransport import RTCSctpCapabilities
 
 DIRECTIONS = ["inactive", "sendonly", "recvonly", "sendrecv"]
 
 DTLS_ROLE_SETUP = {"auto": "actpass", "client": "active", "server": "passive"}
 DTLS_SETUP_ROLE = dict([(v, k) for (k, v) in DTLS_ROLE_SETUP.items()])
 
@@ -386,15 +383,14 @@
             assert current_media
             return next(filter(lambda x: x.payloadType == pt, current_media.rtp.codecs))
 
         session_lines, media_groups = grouplines(sdp)
 
         # parse session
         session = cls()
-        print(session_lines, media_groups)
         for line in session_lines:
             if line.startswith("v="):
                 session.version = int(line.strip()[2:])
             elif line.startswith("o="):
                 session.origin = line.strip()[2:]
             elif line.startswith("s="):
                 session.name = line.strip()[2:]
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/stats.py` & `fleece_network-0.2.1/fleece_network/aiortc/stats.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/aiortc/utils.py` & `fleece_network-0.2.1/fleece_network/aiortc/utils.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc3/fleece_network/messages.py` & `fleece_network-0.2.1/fleece_network/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import dataclass
 from typing import Generic, Optional, TypeVar
-from .aiortc import RTCSessionDescription
+
 from fastapi import Response
 from pydantic import BaseModel  # type: ignore
 
+from .aiortc import RTCSessionDescription
+
 
 @dataclass
 class RegisterRequest:
     worker_id: str
 
 
 @dataclass
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/peer.py` & `fleece_network-0.2.1/fleece_network/peer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-from abc import ABC, abstractmethod
 import asyncio
 import functools
 import inspect
-import anyio
-from anyio import Event, create_memory_object_stream, to_thread
-from anyio.abc import TaskGroup
-from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 import logging
 import pickle
+from abc import ABC, abstractmethod
 from typing import (
     Any,
     Callable,
     Coroutine,
     Optional,
     Protocol,
     TypeVar,
     Union,
     get_type_hints,
 )
+
+import anyio
+import websockets
+from anyio import Event, create_memory_object_stream, to_thread
+from anyio.abc import TaskGroup
+from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
+from fastapi import HTTPException, Response
+from pydantic import BaseModel
+
 from .aiortc import (  # type: ignore
-    RTCPeerConnection,
     RTCConfiguration,
-    RTCIceServer,
     RTCDataChannel,
+    RTCIceServer,
+    RTCPeerConnection,
     RTCSessionDescription,
 )
-from fastapi import HTTPException, Response
-from pydantic import BaseModel
-import websockets
-
 from .messages import (
     ConnectReply,
     ConnectRequest,
+    RegisterRequest,
     SimpleReply,
     SimpleRequest,
-    RegisterRequest,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Encodable(Protocol):
     @abstractmethod
     def encode(self, charset: str) -> bytes: ...
 
 
-P = TypeVar("P", bound=BaseModel)
+P = TypeVar("P", bound=BaseModel | bytes) 
 E = TypeVar("E", bound=Encodable)
 R = Union[E, str]
 SyncHandler = Callable[[P], R]
 AsyncHandler = Callable[[P], Coroutine[Any, Any, R]]
 
 
 class Outward(ABC):
@@ -542,21 +543,24 @@
         def wrapper(*args: Any) -> Any | Coroutine[Any, Any, Any]:
             signature = inspect.signature(func)
             type_hints = get_type_hints(func)
 
             parsed_args = []
             for param_name, arg in zip(signature.parameters, args):
                 model_cls = type_hints[param_name]
-                if isinstance(arg, (str, bytes)):
-                    parsed_arg = model_cls.model_validate_json(arg)
-                elif isinstance(arg, dict):
-                    parsed_arg = model_cls.model_validate(arg)
+                if issubclass(model_cls, BaseModel):
+                    if isinstance(arg, (str, bytes)):
+                        parsed_arg = model_cls.model_validate_json(arg)
+                    elif isinstance(arg, dict):
+                        parsed_arg = model_cls.model_validate(arg)
+                    else:
+                        parsed_arg = arg
+                    parsed_args.append(parsed_arg)
                 else:
-                    parsed_arg = arg
-                parsed_args.append(parsed_arg)
+                    parsed_args.append(arg)
             return func(*parsed_args)
 
         if asyncio.iscoroutinefunction(func):
 
             @functools.wraps(func)
             async def async_wrapper(*args: Any) -> Any:
                 return await wrapper(*args)
@@ -610,16 +614,14 @@
                             message = pickle.loads(raw)
 
                             # TODO: determine whether use worker thread
                             if isinstance(message, ConnectRequest):
                                 self.tg.start_soon(self._answer, ws, message)
                             elif isinstance(message, ConnectReply):
                                 self.tg.start_soon(self._resolve, message)
-
-                                pass
                             else:
                                 self._logger.error(
                                     "Unknown message type %s",
                                     message.__class__.__name__,
                                 )
             except Exception as e:
                 self._logger.warn("Failed to connect to signaling server due to %s", e)
```

### Comparing `fleece_network-0.2.0rc3/fleece_network/signaling.py` & `fleece_network-0.2.1/fleece_network/signaling.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import asyncio
-import uvicorn
 import logging
 import pickle
 from typing import Dict
+
+import uvicorn
 from fastapi import FastAPI, WebSocket, WebSocketDisconnect
-from .messages import (
-    ConnectReply,
-    ConnectRequest,
-    RegisterReply,
-    RegisterRequest,
-)
+
+from .messages import (ConnectReply, ConnectRequest, RegisterReply,
+                       RegisterRequest)
 
 
 class Signaling:
     workers: Dict[str, WebSocket] = {}
     lock: asyncio.Lock = asyncio.Lock()
```

