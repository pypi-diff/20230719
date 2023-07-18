# Comparing `tmp/iamlistening-1.1.0.tar.gz` & `tmp/iamlistening-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-1.1.0.tar", max compression
+gzip compressed data, was "iamlistening-1.1.1.tar", max compression
```

## Comparing `iamlistening-1.1.0.tar` & `iamlistening-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-16 07:42:51.892565 iamlistening-1.1.0/LICENSE
--rw-r--r--   0        0        0     3035 2023-07-16 07:42:51.892565 iamlistening-1.1.0/README.md
--rw-r--r--   0        0        0       99 2023-07-16 07:42:52.580570 iamlistening-1.1.0/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-16 07:42:51.892565 iamlistening-1.1.0/iamlistening/config.py
--rw-r--r--   0        0        0     1325 2023-07-16 07:42:51.892565 iamlistening-1.1.0/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4164 2023-07-16 07:42:51.892565 iamlistening-1.1.0/iamlistening/main.py
--rw-r--r--   0        0        0     2414 2023-07-16 07:42:52.580570 iamlistening-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 iamlistening-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 22:00:43.761457 iamlistening-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2910 2023-07-18 22:00:43.761457 iamlistening-1.1.1/README.md
+-rw-r--r--   0        0        0       99 2023-07-18 22:00:44.801473 iamlistening-1.1.1/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-18 22:00:43.761457 iamlistening-1.1.1/iamlistening/config.py
+-rw-r--r--   0        0        0     1490 2023-07-18 22:00:43.761457 iamlistening-1.1.1/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4307 2023-07-18 22:00:43.761457 iamlistening-1.1.1/iamlistening/main.py
+-rw-r--r--   0        0        0     3075 2023-07-18 22:00:44.801473 iamlistening-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.1/PKG-INFO
```

### Comparing `iamlistening-1.1.0/LICENSE` & `iamlistening-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.0/README.md` & `iamlistening-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -102,89 +102,81 @@
 00000650: 6b69 2f69 616d 6c69 7374 656e 696e 672f  ki/iamlistening/
 00000660: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
 00000670: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 00000680: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
 00000690: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
 000006a0: 732f 6d72 616e 696b 692f 6961 6d6c 6973  s/mraniki/iamlis
 000006b0: 7465 6e69 6e67 2f25 4630 2539 4625 3931  tening/%F0%9F%91
-000006c0: 2542 3725 4532 2538 3025 3844 2545 3225  %B7%E2%80%8D%E2%
-000006d0: 3939 2538 3225 4546 2542 3825 3846 466c  99%82%EF%B8%8FFl
-000006e0: 6f77 2e79 6d6c 3f73 7479 6c65 3d66 6f72  ow.yml?style=for
-000006f0: 2d74 6865 2d62 6164 6765 266c 6f67 6f3d  -the-badge&logo=
-00000700: 4769 7448 7562 266c 6f67 6f43 6f6c 6f72  GitHub&logoColor
-00000710: 3d77 6869 7465 223e 3c2f 613e 3c62 723e  =white"></a><br>
-00000720: 0a20 2020 3c61 2068 7265 663d 2268 7474  .   <a href="htt
-00000730: 7073 3a2f 2f74 616c 6b79 2e72 6561 6474  ps://talky.readt
-00000740: 6865 646f 6373 2e69 6f2f 223e 3c69 6d67  hedocs.io/"><img
-00000750: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
-00000760: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
-00000770: 6f6a 6563 7473 2f69 616d 6c69 7374 656e  ojects/iamlisten
-00000780: 696e 672f 6261 6467 652f 3f76 6572 7369  ing/badge/?versi
-00000790: 6f6e 3d6c 6174 6573 7426 7374 796c 653d  on=latest&style=
-000007a0: 666f 722d 7468 652d 6261 6467 6522 3e3c  for-the-badge"><
-000007b0: 2f61 3e3c 6272 3e0a 2020 203c 6120 6872  /a><br>.   <a hr
-000007c0: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
-000007d0: 6265 6174 2e63 6f2f 7072 6f6a 6563 7473  beat.co/projects
-000007e0: 2f67 6974 6875 622d 636f 6d2d 6d72 616e  /github-com-mran
-000007f0: 696b 692d 6961 6d6c 6973 7465 6e69 6e67  iki-iamlistening
-00000800: 2d6d 6169 6e22 3e3c 696d 6720 7372 633d  -main"><img src=
-00000810: 2268 7474 7073 3a2f 2f63 6f64 6562 6561  "https://codebea
-00000820: 742e 636f 2f62 6164 6765 732f 3430 3835  t.co/badges/4085
-00000830: 3333 3465 2d34 3539 302d 3431 6636 2d61  334e-4590-41f6-a
-00000840: 3730 632d 3639 6539 6132 3634 3163 3739  70c-69e9a2641c79
-00000850: 222f 3e3c 2f61 3e3c 6272 3e0a 2020 203c  "/></a><br>.   <
-00000860: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000870: 636f 6465 636f 762e 696f 2f67 682f 6d72  codecov.io/gh/mr
-00000880: 616e 696b 692f 6961 6d6c 6973 7465 6e69  aniki/iamlisteni
-00000890: 6e67 223e 203c 696d 6720 7372 633d 2268  ng"> <img src="h
-000008a0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-000008b0: 6f2f 6768 2f6d 7261 6e69 6b69 2f69 616d  o/gh/mraniki/iam
-000008c0: 6c69 7374 656e 696e 672f 6272 616e 6368  listening/branch
-000008d0: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
-000008e0: 652e 7376 673f 746f 6b65 6e3d 515a 3535  e.svg?token=QZ55
-000008f0: 5536 4b51 464e 222f 3e3c 2f61 3e3c 6272  U6KQFN"/></a><br
-00000900: 3e0a 2020 2020 3c2f 7464 3e0a 2020 2020  >.    </td>.    
-00000910: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
-00000920: 3e20 0a20 2020 2020 2020 4120 7079 7468  > .       A pyth
-00000930: 6f6e 2070 6163 6b61 6765 2074 6f20 6c69  on package to li
-00000940: 7374 656e 2074 6f20 6d65 7373 6167 696e  sten to messagin
-00000950: 6720 706c 6174 666f 726d 732c 3c62 723e  g platforms,<br>
-00000960: 0a20 2020 2020 2020 7375 6368 2061 7320  .       such as 
-00000970: 6469 7363 6f72 642c 2074 656c 6567 7261  discord, telegra
-00000980: 6d20 616e 6420 6d61 7472 6978 200a 2020  m and matrix .  
-00000990: 2020 3c2f 7464 3e0a 2020 2020 200a 2020    </td>.     .  
-000009a0: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a0a  </tr>.</table>..
-000009b0: 3c68 353e 486f 7720 746f 2075 7365 2069  <h5>How to use i
-000009c0: 743c 2f68 353e 0a3c 7072 653e 0a3c 636f  t</h5>.<pre>.<co
-000009d0: 6465 3e0a 2020 2020 2020 6672 6f6d 2069  de>.      from i
-000009e0: 616d 6c69 7374 656e 696e 6720 696d 706f  amlistening impo
-000009f0: 7274 204c 6973 7465 6e65 720a 2020 2020  rt Listener.    
-00000a00: 2020 2020 6c69 7374 656e 6572 203d 204c      listener = L
-00000a10: 6973 7465 6e65 7228 290a 2020 2020 2020  istener().      
-00000a20: 2020 7461 736b 203d 2061 7379 6e63 696f    task = asyncio
-00000a30: 2e63 7265 6174 655f 7461 736b 286c 6973  .create_task(lis
-00000a40: 7465 6e65 722e 7275 6e5f 666f 7265 7665  tener.run_foreve
-00000a50: 7228 2929 0a20 2020 2020 2020 2077 6869  r()).        whi
-00000a60: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
-00000a70: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00000a80: 2020 2020 2020 6d73 6720 3d20 6177 6169        msg = awai
-00000a90: 7420 6c69 7374 656e 6572 2e67 6574 5f6c  t listener.get_l
-00000aa0: 6174 6573 745f 6d65 7373 6167 6528 290a  atest_message().
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000ac0: 206d 7367 3a0a 2020 2020 2020 2020 2020   msg:.          
-00000ad0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-00000ae0: 4672 6173 6965 72f0 9f91 823a 207b 6d73  Frasier....: {ms
-00000af0: 677d 220a 2020 2020 2020 2020 2020 6578  g}".          ex
-00000b00: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00000b10: 7320 6572 726f 723a 0a20 2020 2020 2020  s error:.       
-00000b20: 2020 2020 2020 2070 7269 6e74 2865 7272         print(err
-00000b30: 6f72 290a 2020 2020 2020 2020 6177 6169  or).        awai
-00000b40: 7420 7461 736b 0a3c 2f63 6f64 653e 0a3c  t task.</code>.<
-00000b50: 2f70 7265 3e0a 0a3c 6835 3e45 7861 6d70  /pre>..<h5>Examp
-00000b60: 6c65 3c2f 6835 3e0a 0a68 7474 7073 3a2f  le</h5>..https:/
-00000b70: 2f67 6974 6875 622e 636f 6d2f 6d72 616e  /github.com/mran
-00000b80: 696b 692f 6961 6d6c 6973 7465 6e69 6e67  iki/iamlistening
-00000b90: 2f62 6c6f 622f 3532 6462 3066 3463 3139  /blob/52db0f4c19
-00000ba0: 3466 6539 6564 6431 3266 3438 3139 3937  4fe9edd12f481997
-00000bb0: 3337 6234 6531 6337 3366 3731 3934 2f65  37b4e1c73f7194/e
-00000bc0: 7861 6d70 6c65 732f 6578 616d 706c 652e  xamples/example.
-00000bd0: 7079 234c 312d 4c35 340a 0a              py#L1-L54..
+000006c0: 2542 3746 6c6f 772e 796d 6c3f 7374 796c  %B7Flow.yml?styl
+000006d0: 653d 666f 722d 7468 652d 6261 6467 6526  e=for-the-badge&
+000006e0: 6c6f 676f 3d47 6974 4875 6226 6c6f 676f  logo=GitHub&logo
+000006f0: 436f 6c6f 723d 7768 6974 6522 3e3c 2f61  Color=white"></a
+00000700: 3e3c 6272 3e0a 2020 203c 6120 6872 6566  ><br>.   <a href
+00000710: 3d22 6874 7470 733a 2f2f 7461 6c6b 792e  ="https://talky.
+00000720: 7265 6164 7468 6564 6f63 732e 696f 2f22  readthedocs.io/"
+00000730: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000740: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
+00000750: 7267 2f70 726f 6a65 6374 732f 6961 6d6c  rg/projects/iaml
+00000760: 6973 7465 6e69 6e67 2f62 6164 6765 2f3f  istening/badge/?
+00000770: 7665 7273 696f 6e3d 6c61 7465 7374 2673  version=latest&s
+00000780: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+00000790: 6765 223e 3c2f 613e 3c62 723e 0a20 2020  ge"></a><br>.   
+000007a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000007b0: 2f63 6f64 6562 6561 742e 636f 2f70 726f  /codebeat.co/pro
+000007c0: 6a65 6374 732f 6769 7468 7562 2d63 6f6d  jects/github-com
+000007d0: 2d6d 7261 6e69 6b69 2d69 616d 6c69 7374  -mraniki-iamlist
+000007e0: 656e 696e 672d 6d61 696e 223e 3c69 6d67  ening-main"><img
+000007f0: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
+00000800: 6465 6265 6174 2e63 6f2f 6261 6467 6573  debeat.co/badges
+00000810: 2f34 3038 3533 3334 652d 3435 3930 2d34  /4085334e-4590-4
+00000820: 3166 362d 6137 3063 2d36 3965 3961 3236  1f6-a70c-69e9a26
+00000830: 3431 6337 3922 2f3e 3c2f 613e 3c62 723e  41c79"/></a><br>
+00000840: 0a20 2020 3c61 2068 7265 663d 2268 7474  .   <a href="htt
+00000850: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+00000860: 6768 2f6d 7261 6e69 6b69 2f69 616d 6c69  gh/mraniki/iamli
+00000870: 7374 656e 696e 6722 3e20 3c69 6d67 2073  stening"> <img s
+00000880: 7263 3d22 6874 7470 733a 2f2f 636f 6465  rc="https://code
+00000890: 636f 762e 696f 2f67 682f 6d72 616e 696b  cov.io/gh/mranik
+000008a0: 692f 6961 6d6c 6973 7465 6e69 6e67 2f62  i/iamlistening/b
+000008b0: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+000008c0: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+000008d0: 3d51 5a35 3555 364b 5146 4e22 2f3e 3c2f  =QZ55U6KQFN"/></
+000008e0: 613e 3c62 723e 0a20 2020 203c 2f74 643e  a><br>.    </td>
+000008f0: 0a20 2020 203c 7464 2061 6c69 676e 3d22  .    <td align="
+00000900: 6c65 6674 223e 200a 2020 2020 2020 2041  left"> .       A
+00000910: 2070 7974 686f 6e20 7061 636b 6167 6520   python package 
+00000920: 746f 206c 6973 7465 6e20 746f 206d 6573  to listen to mes
+00000930: 7361 6769 6e67 2070 6c61 7466 6f72 6d73  saging platforms
+00000940: 2c3c 6272 3e0a 2020 2020 2020 2073 7563  ,<br>.       suc
+00000950: 6820 6173 2064 6973 636f 7264 2c20 7465  h as discord, te
+00000960: 6c65 6772 616d 2061 6e64 206d 6174 7269  legram and matri
+00000970: 782e 0a20 2020 203c 2f74 643e 0a20 2020  x..    </td>.   
+00000980: 2020 0a20 203c 2f74 723e 0a3c 2f74 6162    .  </tr>.</tab
+00000990: 6c65 3e0a 0a3c 6835 3e48 6f77 2074 6f20  le>..<h5>How to 
+000009a0: 7573 6520 6974 3c2f 6835 3e0a 3c70 7265  use it</h5>.<pre
+000009b0: 3e0a 3c63 6f64 653e 0a20 2020 2020 2066  >.<code>.      f
+000009c0: 726f 6d20 6961 6d6c 6973 7465 6e69 6e67  rom iamlistening
+000009d0: 2069 6d70 6f72 7420 4c69 7374 656e 6572   import Listener
+000009e0: 0a20 2020 2020 2020 206c 6973 7465 6e65  .        listene
+000009f0: 7220 3d20 4c69 7374 656e 6572 2829 0a20  r = Listener(). 
+00000a00: 2020 2020 2020 2074 6173 6b20 3d20 6173         task = as
+00000a10: 796e 6369 6f2e 6372 6561 7465 5f74 6173  yncio.create_tas
+00000a20: 6b28 6c69 7374 656e 6572 2e72 756e 5f66  k(listener.run_f
+00000a30: 6f72 6576 6572 2829 290a 2020 2020 2020  orever()).      
+00000a40: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+00000a50: 2020 2020 2020 2020 6d73 6720 3d20 6177          msg = aw
+00000a60: 6169 7420 6c69 7374 656e 6572 2e67 6574  ait listener.get
+00000a70: 5f6c 6174 6573 745f 6d65 7373 6167 6528  _latest_message(
+00000a80: 290a 2020 2020 2020 2020 2020 6966 206d  ).          if m
+00000a90: 7367 3a0a 2020 2020 2020 2020 2020 2020  sg:.            
+00000aa0: 7072 696e 7428 6622 4672 6173 6965 72f0  print(f"Frasier.
+00000ab0: 9f91 823a 207b 6d73 677d 220a 2020 2020  ...: {msg}".    
+00000ac0: 2020 2020 6177 6169 7420 7461 736b 0a3c      await task.<
+00000ad0: 2f63 6f64 653e 0a3c 2f70 7265 3e0a 0a3c  /code>.</pre>..<
+00000ae0: 6835 3e45 7861 6d70 6c65 3c2f 6835 3e0a  h5>Example</h5>.
+00000af0: 0a68 7474 7073 3a2f 2f67 6974 6875 622e  .https://github.
+00000b00: 636f 6d2f 6d72 616e 696b 692f 6961 6d6c  com/mraniki/iaml
+00000b10: 6973 7465 6e69 6e67 2f62 6c6f 622f 6463  istening/blob/dc
+00000b20: 6335 6461 6438 3838 3733 3030 6533 3464  c5dad8887300e34d
+00000b30: 3636 6431 6533 3636 3335 3437 3961 6433  66d1e36635479ad3
+00000b40: 6235 3436 3835 2f65 7861 6d70 6c65 732f  b54685/examples/
+00000b50: 6578 616d 706c 652e 7079 234c 310a       example.py#L1.
```

### Comparing `iamlistening-1.1.0/iamlistening/config.py` & `iamlistening-1.1.1/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.0/iamlistening/default_settings.toml` & `iamlistening-1.1.1/iamlistening/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,49 @@
-#########################################################
-###                  DEFAULT SETTINGS                 ###
-#########################################################
-# Any of those settings can be overwritten by the user.
-# To overwrite a setting, create a settings.toml
-# or load the settings from .env file or vars.
-# As an example, to disable the iamlistening object:
+########################################
+###          DEFAULT SETTINGS        ###
+########################################
+
+# Any of those settings can be changed
+# by the user. To overwrite a setting, 
+# create a settings.toml or load the 
+# settings from .env file or vars.
+# As an example, to disable the 
+# iamlistening object:
 # settings.toml
 # [default]
 # iamlistening_enabled = false
 
+
 [default]
 VALUE = "On Default"
 iamlistening_enabled = true
 bot_token = ""
 bot_channel_id = ""
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = ""
 matrix_user = ""
 matrix_pass = ""
 
 
+
+
+
+
+
+
+
+
+########################################
+###         TESTING SETTINGS         ###
+########################################
+# Any of those settings are used 
+# for testing purpose.
+# It can be ignored. 
+
 [testing]
 VALUE = "On Testing"
 iamlistening_enabled = true
 bot_token = "1234556"
 bot_channel_id = "1234556"
 telethon_api_id = "1234556"
 telethon_api_hash = "1234556"
```

### Comparing `iamlistening-1.1.0/iamlistening/main.py` & `iamlistening-1.1.1/iamlistening/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 """
 
 import asyncio
 import logging
 import threading
 
 import discord
-from telethon import TelegramClient, events
 import simplematrixbotlib as botlib
+from telethon import TelegramClient, events
 
-from .config import settings
 from iamlistening import __version__
 
+from .config import settings
+
+
 class Listener:
     """ 👂 Listener class """
 
     def __init__(self):
         self.logger = logging.getLogger("Listener")
         self.latest_message = None
         self.loop = asyncio.get_event_loop()
@@ -24,14 +26,15 @@
         self.stopped = False
 
     async def start(self):
         """start"""
 
         if settings.telethon_api_id:
             # TELEGRAM
+            self.logger.debug("Telegram setup")
             bot = await TelegramClient(
                         None,
                         settings.telethon_api_id,
                         settings.telethon_api_hash
                         ).start(bot_token=settings.bot_token)
             await self.post_init()
 
@@ -39,14 +42,15 @@
             async def telethon(event):
                 await self.handle_message(event.message.message)
 
             await bot.run_until_disconnected()
 
         elif settings.matrix_hostname:
             # MATRIX
+            self.logger.debug("Matrix setup")
             config = botlib.Config()
             config.emoji_verify = True
             config.ignore_unverified_devices = True
             config.store_path = './config/matrix/'
             creds = botlib.Creds(
                         settings.matrix_hostname,
                         settings.matrix_user,
@@ -71,14 +75,15 @@
                     await action(room_id)
             await bot.api.async_client.sync_forever(
                                                     timeout=3000,
                                                     full_state=True
                                                 )
         elif settings.bot_token:
             # DISCORD
+            self.logger.debug("Discord setup")
             intents = discord.Intents.default()
             intents.message_content = True
             bot = discord.Bot(intents=intents)
 
             @bot.event
             async def on_ready():
                 await self.post_init()
```

### Comparing `iamlistening-1.1.0/pyproject.toml` & `iamlistening-1.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "1.1.0"
+version = "1.1.1"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
@@ -25,17 +25,36 @@
 python = "^3.10"
 dynaconf = "^3.1.12"
 telethon= "^1.28.5"
 py-cord= "^2.4.1"
 simplematrixbotlib= "^2.9.0"
 
 
-[tool.poetry.dev-dependencies]
-python-semantic-release = "^7.34.3"
+[tool.poetry.group.dev.dependencies]
+python-semantic-release = "^8.0.1"
+ruff = "^0.0.278"
+
+[tool.ruff]
+select = [
+  "E",  # pycodestyle
+  "F",  # pyflakes
+  "I",  # isort
+]
+exclude = [
+  ".github/*",
+]
+ignore = ["E401","F401","F811"]
+format = "github"
 
+[tool.pylint.exceptions]
+overgeneral-exceptions = [
+    "builtins.BaseException",
+    "builtins.Exception",
+    "builtins.RuntimeError",
+]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 
@@ -56,27 +75,65 @@
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
+filterwarnings = [
+    " ignore:.*U.*mode is deprecated:DeprecationWarning",
+    "ignore::DeprecationWarning",
+]
 
 [tool.coverage.run]
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
+
 [tool.semantic_release]
-version_variable = ["pyproject.toml:version","iamlistening/__init__.py:__version__"]
-branch = "main"
-upload_to_pypi = true
-upload_to_release = true
+upload_to_vcs_release = true
+version_variables = ["pyproject.toml:version","iamlistening/__init__.py:__version__"]
 build_command = "pip install poetry && poetry build"
-commit_parser = "semantic_release.history.emoji_parser"
-use_textual_changelog_sections = true
-major_emoji = "BREAKING,💥,:boom:"
-minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
-patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
+commit_parser = "emoji"
+
+[tool.semantic_release.commit_parser_options]
+major_tags = [
+    "BREAKING",
+    "💥",
+    ":boom:",
+  ]
+minor_tags = ["feat",
+    "🥚",":egg:",
+    "🚀",":rocket:",
+    "💄",":lipstick:",
+    "✨",":sparkles:",
+]
+
+patch_tags = ["fix","bump","Update",
+    "🎨",":art:",
+    "🐛",":bug:",
+    "🚑",":ambulance:",
+    "⚡",":zap:",
+    "🔥",":fire:",
+    "🚨",":rotating_light:",
+    "♻️",":recycle:",
+    "🔧",":wrench:",
+    "⬆️",":arrow_up:",
+    "🩹",":adhesive_bandage:",
+    "👷",":construction_worker:",
+    "📝",":memo:",
+    "🔒",":lock:",
+    "👽",":alien:",
+    "💬",":speech_balloon:",
+    "🥅",":goal_net:",
+    "✅",":white_check_mark:",
+    "🐳",":whale:",
+    "🙈",":see_no_evil:",
+    "⚗️",":alembic:",
+    "🧐",":monocle_face:",
+    "🔇",":mute:",
+    "🔊",":volume:",
+]
```

### Comparing `iamlistening-1.1.0/PKG-INFO` & `iamlistening-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6961 6d6c  : 2.1.Name: iaml
 00000020: 6973 7465 6e69 6e67 0a56 6572 7369 6f6e  istening.Version
-00000030: 3a20 312e 312e 300a 5375 6d6d 6172 793a  : 1.1.0.Summary:
+00000030: 3a20 312e 312e 310a 5375 6d6d 6172 793a  : 1.1.1.Summary:
 00000040: 2041 2070 7974 686f 6e20 7061 636b 6167   A python packag
 00000050: 6520 746f 2069 6e74 6572 6163 7420 7769  e to interact wi
 00000060: 7468 206d 6573 7361 6769 6e67 2070 6c61  th messaging pla
 00000070: 7466 6f72 6d2e 0a4c 6963 656e 7365 3a20  tform..License: 
 00000080: 4d49 540a 4b65 7977 6f72 6473 3a20 6469  MIT.Keywords: di
 00000090: 7363 6f72 642c 7465 6c65 6772 616d 2c62  scord,telegram,b
 000000a0: 6f74 2c6d 6573 7361 6769 6e67 2c6d 6174  ot,messaging,mat
@@ -160,89 +160,81 @@
 000009f0: 2f69 616d 6c69 7374 656e 696e 672f 223e  /iamlistening/">
 00000a00: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
 00000a10: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
 00000a20: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
 00000a30: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
 00000a40: 6d72 616e 696b 692f 6961 6d6c 6973 7465  mraniki/iamliste
 00000a50: 6e69 6e67 2f25 4630 2539 4625 3931 2542  ning/%F0%9F%91%B
-00000a60: 3725 4532 2538 3025 3844 2545 3225 3939  7%E2%80%8D%E2%99
-00000a70: 2538 3225 4546 2542 3825 3846 466c 6f77  %82%EF%B8%8FFlow
-00000a80: 2e79 6d6c 3f73 7479 6c65 3d66 6f72 2d74  .yml?style=for-t
-00000a90: 6865 2d62 6164 6765 266c 6f67 6f3d 4769  he-badge&logo=Gi
-00000aa0: 7448 7562 266c 6f67 6f43 6f6c 6f72 3d77  tHub&logoColor=w
-00000ab0: 6869 7465 223e 3c2f 613e 3c62 723e 0a20  hite"></a><br>. 
-00000ac0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000ad0: 3a2f 2f74 616c 6b79 2e72 6561 6474 6865  ://talky.readthe
-00000ae0: 646f 6373 2e69 6f2f 223e 3c69 6d67 2073  docs.io/"><img s
-00000af0: 7263 3d22 6874 7470 733a 2f2f 7265 6164  rc="https://read
-00000b00: 7468 6564 6f63 732e 6f72 672f 7072 6f6a  thedocs.org/proj
-00000b10: 6563 7473 2f69 616d 6c69 7374 656e 696e  ects/iamlistenin
-00000b20: 672f 6261 6467 652f 3f76 6572 7369 6f6e  g/badge/?version
-00000b30: 3d6c 6174 6573 7426 7374 796c 653d 666f  =latest&style=fo
-00000b40: 722d 7468 652d 6261 6467 6522 3e3c 2f61  r-the-badge"></a
-00000b50: 3e3c 6272 3e0a 2020 203c 6120 6872 6566  ><br>.   <a href
-00000b60: 3d22 6874 7470 733a 2f2f 636f 6465 6265  ="https://codebe
-00000b70: 6174 2e63 6f2f 7072 6f6a 6563 7473 2f67  at.co/projects/g
-00000b80: 6974 6875 622d 636f 6d2d 6d72 616e 696b  ithub-com-mranik
-00000b90: 692d 6961 6d6c 6973 7465 6e69 6e67 2d6d  i-iamlistening-m
-00000ba0: 6169 6e22 3e3c 696d 6720 7372 633d 2268  ain"><img src="h
-00000bb0: 7474 7073 3a2f 2f63 6f64 6562 6561 742e  ttps://codebeat.
-00000bc0: 636f 2f62 6164 6765 732f 3430 3835 3333  co/badges/408533
-00000bd0: 3465 2d34 3539 302d 3431 6636 2d61 3730  4e-4590-41f6-a70
-00000be0: 632d 3639 6539 6132 3634 3163 3739 222f  c-69e9a2641c79"/
-00000bf0: 3e3c 2f61 3e3c 6272 3e0a 2020 203c 6120  ></a><br>.   <a 
-00000c00: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
-00000c10: 6465 636f 762e 696f 2f67 682f 6d72 616e  decov.io/gh/mran
-00000c20: 696b 692f 6961 6d6c 6973 7465 6e69 6e67  iki/iamlistening
-00000c30: 223e 203c 696d 6720 7372 633d 2268 7474  "> <img src="htt
-00000c40: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-00000c50: 6768 2f6d 7261 6e69 6b69 2f69 616d 6c69  gh/mraniki/iamli
-00000c60: 7374 656e 696e 672f 6272 616e 6368 2f6d  stening/branch/m
-00000c70: 6169 6e2f 6772 6170 682f 6261 6467 652e  ain/graph/badge.
-00000c80: 7376 673f 746f 6b65 6e3d 515a 3535 5536  svg?token=QZ55U6
-00000c90: 4b51 464e 222f 3e3c 2f61 3e3c 6272 3e0a  KQFN"/></a><br>.
-00000ca0: 2020 2020 3c2f 7464 3e0a 2020 2020 3c74      </td>.    <t
-00000cb0: 6420 616c 6967 6e3d 226c 6566 7422 3e20  d align="left"> 
-00000cc0: 0a20 2020 2020 2020 4120 7079 7468 6f6e  .       A python
-00000cd0: 2070 6163 6b61 6765 2074 6f20 6c69 7374   package to list
-00000ce0: 656e 2074 6f20 6d65 7373 6167 696e 6720  en to messaging 
-00000cf0: 706c 6174 666f 726d 732c 3c62 723e 0a20  platforms,<br>. 
-00000d00: 2020 2020 2020 7375 6368 2061 7320 6469        such as di
-00000d10: 7363 6f72 642c 2074 656c 6567 7261 6d20  scord, telegram 
-00000d20: 616e 6420 6d61 7472 6978 200a 2020 2020  and matrix .    
-00000d30: 3c2f 7464 3e0a 2020 2020 200a 2020 3c2f  </td>.     .  </
-00000d40: 7472 3e0a 3c2f 7461 626c 653e 0a0a 3c68  tr>.</table>..<h
-00000d50: 353e 486f 7720 746f 2075 7365 2069 743c  5>How to use it<
-00000d60: 2f68 353e 0a3c 7072 653e 0a3c 636f 6465  /h5>.<pre>.<code
-00000d70: 3e0a 2020 2020 2020 6672 6f6d 2069 616d  >.      from iam
-00000d80: 6c69 7374 656e 696e 6720 696d 706f 7274  listening import
-00000d90: 204c 6973 7465 6e65 720a 2020 2020 2020   Listener.      
-00000da0: 2020 6c69 7374 656e 6572 203d 204c 6973    listener = Lis
-00000db0: 7465 6e65 7228 290a 2020 2020 2020 2020  tener().        
-00000dc0: 7461 736b 203d 2061 7379 6e63 696f 2e63  task = asyncio.c
-00000dd0: 7265 6174 655f 7461 736b 286c 6973 7465  reate_task(liste
-00000de0: 6e65 722e 7275 6e5f 666f 7265 7665 7228  ner.run_forever(
-00000df0: 2929 0a20 2020 2020 2020 2077 6869 6c65  )).        while
-00000e00: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
-00000e10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00000e20: 2020 2020 6d73 6720 3d20 6177 6169 7420      msg = await 
-00000e30: 6c69 7374 656e 6572 2e67 6574 5f6c 6174  listener.get_lat
-00000e40: 6573 745f 6d65 7373 6167 6528 290a 2020  est_message().  
-00000e50: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00000e60: 7367 3a0a 2020 2020 2020 2020 2020 2020  sg:.            
-00000e70: 2020 2020 2020 7072 696e 7428 6622 4672        print(f"Fr
-00000e80: 6173 6965 72f0 9f91 823a 207b 6d73 677d  asier....: {msg}
-00000e90: 220a 2020 2020 2020 2020 2020 6578 6365  ".          exce
-00000ea0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00000eb0: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
-00000ec0: 2020 2020 2070 7269 6e74 2865 7272 6f72       print(error
-00000ed0: 290a 2020 2020 2020 2020 6177 6169 7420  ).        await 
-00000ee0: 7461 736b 0a3c 2f63 6f64 653e 0a3c 2f70  task.</code>.</p
-00000ef0: 7265 3e0a 0a3c 6835 3e45 7861 6d70 6c65  re>..<h5>Example
-00000f00: 3c2f 6835 3e0a 0a68 7474 7073 3a2f 2f67  </h5>..https://g
-00000f10: 6974 6875 622e 636f 6d2f 6d72 616e 696b  ithub.com/mranik
-00000f20: 692f 6961 6d6c 6973 7465 6e69 6e67 2f62  i/iamlistening/b
-00000f30: 6c6f 622f 3532 6462 3066 3463 3139 3466  lob/52db0f4c194f
-00000f40: 6539 6564 6431 3266 3438 3139 3937 3337  e9edd12f48199737
-00000f50: 6234 6531 6337 3366 3731 3934 2f65 7861  b4e1c73f7194/exa
-00000f60: 6d70 6c65 732f 6578 616d 706c 652e 7079  mples/example.py
-00000f70: 234c 312d 4c35 340a 0a0a                 #L1-L54...
+00000a60: 3746 6c6f 772e 796d 6c3f 7374 796c 653d  7Flow.yml?style=
+00000a70: 666f 722d 7468 652d 6261 6467 6526 6c6f  for-the-badge&lo
+00000a80: 676f 3d47 6974 4875 6226 6c6f 676f 436f  go=GitHub&logoCo
+00000a90: 6c6f 723d 7768 6974 6522 3e3c 2f61 3e3c  lor=white"></a><
+00000aa0: 6272 3e0a 2020 203c 6120 6872 6566 3d22  br>.   <a href="
+00000ab0: 6874 7470 733a 2f2f 7461 6c6b 792e 7265  https://talky.re
+00000ac0: 6164 7468 6564 6f63 732e 696f 2f22 3e3c  adthedocs.io/"><
+00000ad0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000ae0: 2f72 6561 6474 6865 646f 6373 2e6f 7267  /readthedocs.org
+00000af0: 2f70 726f 6a65 6374 732f 6961 6d6c 6973  /projects/iamlis
+00000b00: 7465 6e69 6e67 2f62 6164 6765 2f3f 7665  tening/badge/?ve
+00000b10: 7273 696f 6e3d 6c61 7465 7374 2673 7479  rsion=latest&sty
+00000b20: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00000b30: 223e 3c2f 613e 3c62 723e 0a20 2020 3c61  "></a><br>.   <a
+00000b40: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00000b50: 6f64 6562 6561 742e 636f 2f70 726f 6a65  odebeat.co/proje
+00000b60: 6374 732f 6769 7468 7562 2d63 6f6d 2d6d  cts/github-com-m
+00000b70: 7261 6e69 6b69 2d69 616d 6c69 7374 656e  raniki-iamlisten
+00000b80: 696e 672d 6d61 696e 223e 3c69 6d67 2073  ing-main"><img s
+00000b90: 7263 3d22 6874 7470 733a 2f2f 636f 6465  rc="https://code
+00000ba0: 6265 6174 2e63 6f2f 6261 6467 6573 2f34  beat.co/badges/4
+00000bb0: 3038 3533 3334 652d 3435 3930 2d34 3166  085334e-4590-41f
+00000bc0: 362d 6137 3063 2d36 3965 3961 3236 3431  6-a70c-69e9a2641
+00000bd0: 6337 3922 2f3e 3c2f 613e 3c62 723e 0a20  c79"/></a><br>. 
+00000be0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000bf0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000c00: 2f6d 7261 6e69 6b69 2f69 616d 6c69 7374  /mraniki/iamlist
+00000c10: 656e 696e 6722 3e20 3c69 6d67 2073 7263  ening"> <img src
+00000c20: 3d22 6874 7470 733a 2f2f 636f 6465 636f  ="https://codeco
+00000c30: 762e 696f 2f67 682f 6d72 616e 696b 692f  v.io/gh/mraniki/
+00000c40: 6961 6d6c 6973 7465 6e69 6e67 2f62 7261  iamlistening/bra
+00000c50: 6e63 682f 6d61 696e 2f67 7261 7068 2f62  nch/main/graph/b
+00000c60: 6164 6765 2e73 7667 3f74 6f6b 656e 3d51  adge.svg?token=Q
+00000c70: 5a35 3555 364b 5146 4e22 2f3e 3c2f 613e  Z55U6KQFN"/></a>
+00000c80: 3c62 723e 0a20 2020 203c 2f74 643e 0a20  <br>.    </td>. 
+00000c90: 2020 203c 7464 2061 6c69 676e 3d22 6c65     <td align="le
+00000ca0: 6674 223e 200a 2020 2020 2020 2041 2070  ft"> .       A p
+00000cb0: 7974 686f 6e20 7061 636b 6167 6520 746f  ython package to
+00000cc0: 206c 6973 7465 6e20 746f 206d 6573 7361   listen to messa
+00000cd0: 6769 6e67 2070 6c61 7466 6f72 6d73 2c3c  ging platforms,<
+00000ce0: 6272 3e0a 2020 2020 2020 2073 7563 6820  br>.       such 
+00000cf0: 6173 2064 6973 636f 7264 2c20 7465 6c65  as discord, tele
+00000d00: 6772 616d 2061 6e64 206d 6174 7269 782e  gram and matrix.
+00000d10: 0a20 2020 203c 2f74 643e 0a20 2020 2020  .    </td>.     
+00000d20: 0a20 203c 2f74 723e 0a3c 2f74 6162 6c65  .  </tr>.</table
+00000d30: 3e0a 0a3c 6835 3e48 6f77 2074 6f20 7573  >..<h5>How to us
+00000d40: 6520 6974 3c2f 6835 3e0a 3c70 7265 3e0a  e it</h5>.<pre>.
+00000d50: 3c63 6f64 653e 0a20 2020 2020 2066 726f  <code>.      fro
+00000d60: 6d20 6961 6d6c 6973 7465 6e69 6e67 2069  m iamlistening i
+00000d70: 6d70 6f72 7420 4c69 7374 656e 6572 0a20  mport Listener. 
+00000d80: 2020 2020 2020 206c 6973 7465 6e65 7220         listener 
+00000d90: 3d20 4c69 7374 656e 6572 2829 0a20 2020  = Listener().   
+00000da0: 2020 2020 2074 6173 6b20 3d20 6173 796e       task = asyn
+00000db0: 6369 6f2e 6372 6561 7465 5f74 6173 6b28  cio.create_task(
+00000dc0: 6c69 7374 656e 6572 2e72 756e 5f66 6f72  listener.run_for
+00000dd0: 6576 6572 2829 290a 2020 2020 2020 2020  ever()).        
+00000de0: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+00000df0: 2020 2020 2020 6d73 6720 3d20 6177 6169        msg = awai
+00000e00: 7420 6c69 7374 656e 6572 2e67 6574 5f6c  t listener.get_l
+00000e10: 6174 6573 745f 6d65 7373 6167 6528 290a  atest_message().
+00000e20: 2020 2020 2020 2020 2020 6966 206d 7367            if msg
+00000e30: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00000e40: 696e 7428 6622 4672 6173 6965 72f0 9f91  int(f"Frasier...
+00000e50: 823a 207b 6d73 677d 220a 2020 2020 2020  .: {msg}".      
+00000e60: 2020 6177 6169 7420 7461 736b 0a3c 2f63    await task.</c
+00000e70: 6f64 653e 0a3c 2f70 7265 3e0a 0a3c 6835  ode>.</pre>..<h5
+00000e80: 3e45 7861 6d70 6c65 3c2f 6835 3e0a 0a68  >Example</h5>..h
+00000e90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ea0: 6d2f 6d72 616e 696b 692f 6961 6d6c 6973  m/mraniki/iamlis
+00000eb0: 7465 6e69 6e67 2f62 6c6f 622f 6463 6335  tening/blob/dcc5
+00000ec0: 6461 6438 3838 3733 3030 6533 3464 3636  dad8887300e34d66
+00000ed0: 6431 6533 3636 3335 3437 3961 6433 6235  d1e36635479ad3b5
+00000ee0: 3436 3835 2f65 7861 6d70 6c65 732f 6578  4685/examples/ex
+00000ef0: 616d 706c 652e 7079 234c 310a 0a         ample.py#L1..
```

