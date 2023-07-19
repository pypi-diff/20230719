# Comparing `tmp/thug-5.2.tar.gz` & `tmp/thug-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thug-5.2.tar", last modified: Tue Jun 20 07:50:58 2023, max compression
+gzip compressed data, was "thug-5.3.tar", last modified: Wed Jul 19 08:14:57 2023, max compression
```

## Comparing `thug-5.2.tar` & `thug-5.3.tar`

### file list

```diff
@@ -1,518 +1,518 @@
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.271997 thug-5.2/
--rw-r--r--   0 buffer     (502) staff       (20)    17987 2022-12-28 14:31:40.000000 thug-5.2/LICENSE.txt
--rw-r--r--   0 buffer     (502) staff       (20)      130 2023-01-03 13:39:45.000000 thug-5.2/MANIFEST.in
--rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-06-20 07:50:58.271495 thug-5.2/PKG-INFO
--rw-r--r--   0 buffer     (502) staff       (20)     2676 2023-01-17 09:44:55.000000 thug-5.2/README.rst
--rw-r--r--   0 buffer     (502) staff       (20)     3485 2023-06-20 07:28:22.000000 thug-5.2/pyproject.toml
--rw-r--r--   0 buffer     (502) staff       (20)      339 2023-06-20 07:28:11.000000 thug-5.2/requirements.txt
--rw-r--r--   0 buffer     (502) staff       (20)       38 2023-06-20 07:50:58.272130 thug-5.2/setup.cfg
--rw-r--r--   0 buffer     (502) staff       (20)     1346 2023-01-03 12:33:41.000000 thug-5.2/setup.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.822662 thug-5.2/thug/
--rw-r--r--   0 buffer     (502) staff       (20)     8196 2022-11-04 15:21:57.000000 thug-5.2/thug/.DS_Store
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.832799 thug-5.2/thug/ActiveX/
--rw-r--r--   0 buffer     (502) staff       (20)     7598 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/ActiveX.py
--rw-r--r--   0 buffer     (502) staff       (20)    64018 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/CLSID.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.940343 thug-5.2/thug/ActiveX/modules/
--rw-r--r--   0 buffer     (502) staff       (20)      400 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AOLAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)     1119 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AcroPDF.py
--rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AdodbRecordset.py
--rw-r--r--   0 buffer     (502) staff       (20)     2573 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AdodbStream.py
--rw-r--r--   0 buffer     (502) staff       (20)     1482 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AnswerWorks.py
--rw-r--r--   0 buffer     (502) staff       (20)     1086 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AolAmpX.py
--rw-r--r--   0 buffer     (502) staff       (20)      979 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/AolICQ.py
--rw-r--r--   0 buffer     (502) staff       (20)      801 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/BaiduBar.py
--rw-r--r--   0 buffer     (502) staff       (20)      567 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/BitDefender.py
--rw-r--r--   0 buffer     (502) staff       (20)      421 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/CABrightStor.py
--rw-r--r--   0 buffer     (502) staff       (20)      600 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/CGAgent.py
--rw-r--r--   0 buffer     (502) staff       (20)      726 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Comodo.py
--rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ConnectAndEnterRoom.py
--rw-r--r--   0 buffer     (502) staff       (20)      307 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/CreativeSoftAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/DLinkMPEG.py
--rw-r--r--   0 buffer     (502) staff       (20)      673 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/DPClient.py
--rw-r--r--   0 buffer     (502) staff       (20)      447 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/DVRHOSTWeb.py
--rw-r--r--   0 buffer     (502) staff       (20)      625 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/DirectShow.py
--rw-r--r--   0 buffer     (502) staff       (20)      404 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/DivX.py
--rw-r--r--   0 buffer     (502) staff       (20)     1857 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Domino.py
--rw-r--r--   0 buffer     (502) staff       (20)     1500 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/EnjoySAP.py
--rw-r--r--   0 buffer     (502) staff       (20)      825 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/FacebookPhotoUploader.py
--rw-r--r--   0 buffer     (502) staff       (20)     3049 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/File.py
--rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/FileUploader.py
--rw-r--r--   0 buffer     (502) staff       (20)     2221 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Folder.py
--rw-r--r--   0 buffer     (502) staff       (20)      496 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/GLIEDown2.py
--rw-r--r--   0 buffer     (502) staff       (20)      656 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/GatewayWeblaunch.py
--rw-r--r--   0 buffer     (502) staff       (20)      420 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Gogago.py
--rw-r--r--   0 buffer     (502) staff       (20)      561 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/GomWeb.py
--rw-r--r--   0 buffer     (502) staff       (20)     4119 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/HPInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)      443 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ICQToolbar.py
--rw-r--r--   0 buffer     (502) staff       (20)      945 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/IMWebControl.py
--rw-r--r--   0 buffer     (502) staff       (20)      672 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/InternetCleverSuite.py
--rw-r--r--   0 buffer     (502) staff       (20)     1964 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/JavaDeploymentToolkit.py
--rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
--rw-r--r--   0 buffer     (502) staff       (20)      405 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Kingsoft.py
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/MSRICHTXT.py
--rw-r--r--   0 buffer     (502) staff       (20)      601 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/MSVFP.py
--rw-r--r--   0 buffer     (502) staff       (20)      535 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/MSXML2DOMDocument.py
--rw-r--r--   0 buffer     (502) staff       (20)     4390 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/MacrovisionFlexNet.py
--rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/MicrosoftWorks7Attack.py
--rw-r--r--   0 buffer     (502) staff       (20)     2048 2023-01-13 08:09:32.000000 thug-5.2/thug/ActiveX/modules/MicrosoftXMLDOM.py
--rw-r--r--   0 buffer     (502) staff       (20)     8006 2023-01-06 14:50:41.000000 thug-5.2/thug/ActiveX/modules/MicrosoftXMLHTTP.py
--rw-r--r--   0 buffer     (502) staff       (20)      466 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Move.py
--rw-r--r--   0 buffer     (502) staff       (20)      438 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/MyspaceUploader.py
--rw-r--r--   0 buffer     (502) staff       (20)      589 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/NCTAudioFile2.py
--rw-r--r--   0 buffer     (502) staff       (20)     1259 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/NamoInstaller.py
--rw-r--r--   0 buffer     (502) staff       (20)      616 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/NeoTracePro.py
--rw-r--r--   0 buffer     (502) staff       (20)     3311 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/NessusScanCtrl.py
--rw-r--r--   0 buffer     (502) staff       (20)     1175 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/OfficeOCX.py
--rw-r--r--   0 buffer     (502) staff       (20)     1057 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/OurgameGLWorld.py
--rw-r--r--   0 buffer     (502) staff       (20)     1201 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/PPlayer.py
--rw-r--r--   0 buffer     (502) staff       (20)      498 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/PTZCamPanel.py
--rw-r--r--   0 buffer     (502) staff       (20)      494 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/QuantumStreaming.py
--rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/QvodCtrl.py
--rw-r--r--   0 buffer     (502) staff       (20)      973 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/RDSDataSpace.py
--rw-r--r--   0 buffer     (502) staff       (20)     2335 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/RealPlayer.py
--rw-r--r--   0 buffer     (502) staff       (20)      348 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/RediffBolDownloaderAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)      831 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/RegistryPro.py
--rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/RisingScanner.py
--rw-r--r--   0 buffer     (502) staff       (20)      449 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/RtspVaPgCtrl.py
--rw-r--r--   0 buffer     (502) staff       (20)     1116 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SSReaderPdg2.py
--rw-r--r--   0 buffer     (502) staff       (20)     1027 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ScriptingDictionary.py
--rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ScriptingEncoder.py
--rw-r--r--   0 buffer     (502) staff       (20)     5185 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ScriptingFileSystemObject.py
--rw-r--r--   0 buffer     (502) staff       (20)     1527 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ShellApplication.py
--rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Shockwave.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ShockwaveFlash10.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ShockwaveFlash11.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ShockwaveFlash12.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ShockwaveFlash9.py
--rw-r--r--   0 buffer     (502) staff       (20)      273 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SilverLight.py
--rw-r--r--   0 buffer     (502) staff       (20)      921 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SinaDLoader.py
--rw-r--r--   0 buffer     (502) staff       (20)     1472 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SnapshotViewer.py
--rw-r--r--   0 buffer     (502) staff       (20)      715 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
--rw-r--r--   0 buffer     (502) staff       (20)      906 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Spreadsheet.py
--rw-r--r--   0 buffer     (502) staff       (20)      677 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/StormConfig.py
--rw-r--r--   0 buffer     (502) staff       (20)     2436 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/StormMps.py
--rw-r--r--   0 buffer     (502) staff       (20)      516 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/StreamAudioChainCast.py
--rw-r--r--   0 buffer     (502) staff       (20)     1061 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SymantecAppStream.py
--rw-r--r--   0 buffer     (502) staff       (20)     2224 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/SymantecBackupExec.py
--rw-r--r--   0 buffer     (502) staff       (20)     4772 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/TextStream.py
--rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/Toshiba.py
--rw-r--r--   0 buffer     (502) staff       (20)      391 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/UUSeeUpdate.py
--rw-r--r--   0 buffer     (502) staff       (20)      691 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/UniversalUpload.py
--rw-r--r--   0 buffer     (502) staff       (20)     1763 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/VLC.py
--rw-r--r--   0 buffer     (502) staff       (20)      719 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/VisualStudioDTE80.py
--rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/VsaIDEDTE.py
--rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/VsmIDEDTE.py
--rw-r--r--   0 buffer     (502) staff       (20)      796 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WMEncProfileManager.py
--rw-r--r--   0 buffer     (502) staff       (20)      132 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WMP.py
--rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WScriptCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1280 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WScriptExec.py
--rw-r--r--   0 buffer     (502) staff       (20)     1689 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WScriptNetwork.py
--rw-r--r--   0 buffer     (502) staff       (20)     8980 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WScriptShell.py
--rw-r--r--   0 buffer     (502) staff       (20)      213 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WScriptShortcut.py
--rw-r--r--   0 buffer     (502) staff       (20)      645 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WebViewFolderIcon.py
--rw-r--r--   0 buffer     (502) staff       (20)     1373 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WinNTSystemInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)      599 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WinZip.py
--rw-r--r--   0 buffer     (502) staff       (20)      145 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/WindowsMediaPlayer.py
--rw-r--r--   0 buffer     (502) staff       (20)      942 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/XMLDOMParseError.py
--rw-r--r--   0 buffer     (502) staff       (20)     1026 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/XUpload.py
--rw-r--r--   0 buffer     (502) staff       (20)     1159 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/YahooJukebox.py
--rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/YahooMessengerCyft.py
--rw-r--r--   0 buffer     (502) staff       (20)     1077 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/YahooMessengerYVerInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)     1244 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/YahooMessengerYwcvwr.py
--rw-r--r--   0 buffer     (502) staff       (20)     1932 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)     2870 2022-12-28 14:31:40.000000 thug-5.2/thug/ActiveX/modules/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.941146 thug-5.2/thug/Analysis/
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.942389 thug-5.2/thug/Analysis/awis/
--rw-r--r--   0 buffer     (502) staff       (20)     3224 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/awis/AWIS.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/awis/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.943882 thug-5.2/thug/Analysis/context/
--rw-r--r--   0 buffer     (502) staff       (20)     1554 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/context/ContextAnalyzer.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/context/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.945616 thug-5.2/thug/Analysis/honeyagent/
--rw-r--r--   0 buffer     (502) staff       (20)     4000 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/honeyagent/HoneyAgent.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/honeyagent/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.947343 thug-5.2/thug/Analysis/screenshot/
--rw-r--r--   0 buffer     (502) staff       (20)     1333 2023-03-07 14:57:11.000000 thug-5.2/thug/Analysis/screenshot/Screenshot.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/screenshot/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.949756 thug-5.2/thug/Analysis/shellcode/
--rw-r--r--   0 buffer     (502) staff       (20)     8069 2023-01-13 08:09:32.000000 thug-5.2/thug/Analysis/shellcode/Shellcode.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Analysis/shellcode/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.959863 thug-5.2/thug/Classifier/
--rw-r--r--   0 buffer     (502) staff       (20)     5017 2023-03-28 13:07:55.000000 thug-5.2/thug/Classifier/BaseClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2106 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/CookieClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2159 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/HTMLClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2070 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/ImageClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2008 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/JSClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2243 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/SampleClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2082 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/TextClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2330 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/URLClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2014 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/VBSClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Classifier/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.067747 thug-5.2/thug/DOM/
--rw-r--r--   0 buffer     (502) staff       (20)     2534 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Alexa.py
--rw-r--r--   0 buffer     (502) staff       (20)     2289 2023-03-28 10:08:11.000000 thug-5.2/thug/DOM/AsyncPrefetcher.py
--rw-r--r--   0 buffer     (502) staff       (20)     2254 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/CCInterpreter.py
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Chrome.py
--rw-r--r--   0 buffer     (502) staff       (20)     1304 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/ClipboardData.py
--rw-r--r--   0 buffer     (502) staff       (20)      817 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Components.py
--rw-r--r--   0 buffer     (502) staff       (20)     5901 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Console.py
--rw-r--r--   0 buffer     (502) staff       (20)     1112 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Crypto.py
--rw-r--r--   0 buffer     (502) staff       (20)    54541 2023-03-01 08:10:57.000000 thug-5.2/thug/DOM/DFT.py
--rw-r--r--   0 buffer     (502) staff       (20)     3602 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/External.py
--rw-r--r--   0 buffer     (502) staff       (20)     2776 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/HTMLInspector.py
--rw-r--r--   0 buffer     (502) staff       (20)     9866 2023-03-07 14:57:11.000000 thug-5.2/thug/DOM/HTTPSession.py
--rw-r--r--   0 buffer     (502) staff       (20)      932 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/HTTPSessionException.py
--rw-r--r--   0 buffer     (502) staff       (20)     3593 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/History.py
--rw-r--r--   0 buffer     (502) staff       (20)     3506 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/JSClass.py
--rw-r--r--   0 buffer     (502) staff       (20)     7824 2023-01-06 16:11:13.000000 thug-5.2/thug/DOM/JSEngine.py
--rw-r--r--   0 buffer     (502) staff       (20)     4502 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/JSInspector.py
--rw-r--r--   0 buffer     (502) staff       (20)     5959 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/JScriptEncode.py
--rw-r--r--   0 buffer     (502) staff       (20)      752 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/LocalStorage.py
--rw-r--r--   0 buffer     (502) staff       (20)     4661 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/Location.py
--rw-r--r--   0 buffer     (502) staff       (20)    19549 2023-02-27 08:54:28.000000 thug-5.2/thug/DOM/MIMEHandler.py
--rw-r--r--   0 buffer     (502) staff       (20)      762 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Map.py
--rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/MimeType.py
--rw-r--r--   0 buffer     (502) staff       (20)     5282 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/MimeTypes.py
--rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/MozConnection.py
--rw-r--r--   0 buffer     (502) staff       (20)    13340 2023-03-07 14:57:11.000000 thug-5.2/thug/DOM/Navigator.py
--rw-r--r--   0 buffer     (502) staff       (20)     4056 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Personality.py
--rw-r--r--   0 buffer     (502) staff       (20)     1233 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Plugin.py
--rw-r--r--   0 buffer     (502) staff       (20)     1471 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Plugins.py
--rw-r--r--   0 buffer     (502) staff       (20)     1069 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/SchemeHandler.py
--rw-r--r--   0 buffer     (502) staff       (20)     6150 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Screen.py
--rw-r--r--   0 buffer     (502) staff       (20)      756 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/SessionStorage.py
--rw-r--r--   0 buffer     (502) staff       (20)     1750 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Sidebar.py
--rw-r--r--   0 buffer     (502) staff       (20)     3502 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Storage.py
--rw-r--r--   0 buffer     (502) staff       (20)     3216 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/UserProfile.py
--rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/Utils.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.073409 thug-5.2/thug/DOM/W3C/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.097569 thug-5.2/thug/DOM/W3C/Core/
--rw-r--r--   0 buffer     (502) staff       (20)     2138 2023-01-06 12:37:35.000000 thug-5.2/thug/DOM/W3C/Core/Attr.py
--rw-r--r--   0 buffer     (502) staff       (20)      265 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/CDATASection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1241 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Core/CharacterData.py
--rw-r--r--   0 buffer     (502) staff       (20)     3531 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Core/ClassList.py
--rw-r--r--   0 buffer     (502) staff       (20)      564 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/Comment.py
--rw-r--r--   0 buffer     (502) staff       (20)     1910 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Core/DOMException.py
--rw-r--r--   0 buffer     (502) staff       (20)     5765 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/DOMImplementation.py
--rw-r--r--   0 buffer     (502) staff       (20)     8868 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/Document.py
--rw-r--r--   0 buffer     (502) staff       (20)     2412 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/DocumentFragment.py
--rw-r--r--   0 buffer     (502) staff       (20)     1513 2023-01-06 12:31:24.000000 thug-5.2/thug/DOM/W3C/Core/DocumentType.py
--rw-r--r--   0 buffer     (502) staff       (20)     9544 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/Element.py
--rw-r--r--   0 buffer     (502) staff       (20)      457 2023-01-06 12:38:21.000000 thug-5.2/thug/DOM/W3C/Core/Entity.py
--rw-r--r--   0 buffer     (502) staff       (20)      501 2023-01-06 12:38:52.000000 thug-5.2/thug/DOM/W3C/Core/EntityReference.py
--rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Core/NamedNodeMap.py
--rw-r--r--   0 buffer     (502) staff       (20)    14464 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/Node.py
--rw-r--r--   0 buffer     (502) staff       (20)      569 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/NodeList.py
--rw-r--r--   0 buffer     (502) staff       (20)      474 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/NodeType.py
--rw-r--r--   0 buffer     (502) staff       (20)      485 2023-01-06 12:34:08.000000 thug-5.2/thug/DOM/W3C/Core/Notation.py
--rw-r--r--   0 buffer     (502) staff       (20)      510 2023-01-06 12:34:27.000000 thug-5.2/thug/DOM/W3C/Core/ProcessingInstruction.py
--rw-r--r--   0 buffer     (502) staff       (20)      803 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/Text.py
--rw-r--r--   0 buffer     (502) staff       (20)     1051 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Core/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      337 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Core/abstractmethod.py
--rw-r--r--   0 buffer     (502) staff       (20)      274 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/DOMParser.py
--rw-r--r--   0 buffer     (502) staff       (20)     1454 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/DOMTokenList.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.107910 thug-5.2/thug/DOM/W3C/Events/
--rw-r--r--   0 buffer     (502) staff       (20)      868 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/DocumentEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     4120 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/Event.py
--rw-r--r--   0 buffer     (502) staff       (20)      525 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/EventException.py
--rw-r--r--   0 buffer     (502) staff       (20)      272 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/EventListener.py
--rw-r--r--   0 buffer     (502) staff       (20)     9134 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/EventTarget.py
--rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/HTMLEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     1206 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/MessageEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     2198 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/MouseEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     1575 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/MutationEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/StorageEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)      636 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Events/UIEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)      691 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/Events/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.110181 thug-5.2/thug/DOM/W3C/File/
--rw-r--r--   0 buffer     (502) staff       (20)     2433 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/File/Blob.py
--rw-r--r--   0 buffer     (502) staff       (20)     1381 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/File/File.py
--rw-r--r--   0 buffer     (502) staff       (20)       85 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/File/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.166636 thug-5.2/thug/DOM/W3C/HTML/
--rw-r--r--   0 buffer     (502) staff       (20)      194 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/AudioTrackList.py
--rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/Dataset.py
--rw-r--r--   0 buffer     (502) staff       (20)      374 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLAllCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1922 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLAnchorElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      654 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLAppletElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLAudioElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      252 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLBRElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLBaseElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      331 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1486 2023-04-11 09:54:20.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLBodyElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      582 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLButtonElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1281 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)      265 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLDListElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      263 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLDivElement.py
--rw-r--r--   0 buffer     (502) staff       (20)    15982 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLDocument.py
--rw-r--r--   0 buffer     (502) staff       (20)      955 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)      412 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     4141 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      322 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLFontElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1742 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLFormElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      978 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLFrameElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      289 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      407 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLHRElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLHeadElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLHeadingElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLHtmlElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1300 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLIFrameElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1302 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLImageElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1466 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLInputElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      277 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLLIElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      373 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLLabelElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      376 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLLegendElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      558 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLLinkElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     4216 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLMediaElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      264 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLMenuElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      667 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLMetaElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      296 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLModElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLOListElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     2595 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLObjectElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      343 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLOptionElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      227 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)      259 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLParagraphElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLParamElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLPreElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLQuoteElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      988 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLScriptElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1636 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLSelectElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      177 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLSpanElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      316 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLStyleElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      262 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      917 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTableCellElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTableColElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     4711 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTableElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     2800 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTableRowElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     2091 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1031 2022-12-30 12:26:43.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLTitleElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/HTMLUListElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/TAnimateColor.py
--rw-r--r--   0 buffer     (502) staff       (20)      280 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/TextTrackList.py
--rw-r--r--   0 buffer     (502) staff       (20)      681 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/TimeRanges.py
--rw-r--r--   0 buffer     (502) staff       (20)     5132 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      442 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/attr_property.py
--rw-r--r--   0 buffer     (502) staff       (20)      426 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/bool_property.py
--rw-r--r--   0 buffer     (502) staff       (20)      436 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/HTML/form_property.py
--rw-r--r--   0 buffer     (502) staff       (20)      806 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/HTML/text_property.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.167267 thug-5.2/thug/DOM/W3C/Style/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.169221 thug-5.2/thug/DOM/W3C/Style/CSS/
--rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
--rw-r--r--   0 buffer     (502) staff       (20)      425 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Style/CSS/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Style/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.171204 thug-5.2/thug/DOM/W3C/URL/
--rw-r--r--   0 buffer     (502) staff       (20)     4843 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/URL/URL.py
--rw-r--r--   0 buffer     (502) staff       (20)     2710 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/URL/URLSearchParams.py
--rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/URL/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.173678 thug-5.2/thug/DOM/W3C/Views/
--rw-r--r--   0 buffer     (502) staff       (20)      217 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Views/AbstractView.py
--rw-r--r--   0 buffer     (502) staff       (20)      211 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Views/DocumentView.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/Views/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)       56 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/W3C/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      367 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/W3C/w3c.py
--rw-r--r--   0 buffer     (502) staff       (20)      829 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/WebStore.py
--rw-r--r--   0 buffer     (502) staff       (20)    35015 2023-01-13 08:09:32.000000 thug-5.2/thug/DOM/Window.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)     7624 2022-12-28 14:31:40.000000 thug-5.2/thug/DOM/w3c_bindings.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.174907 thug-5.2/thug/Encoding/
--rw-r--r--   0 buffer     (502) staff       (20)      877 2022-12-28 14:31:40.000000 thug-5.2/thug/Encoding/Encoding.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Encoding/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.177466 thug-5.2/thug/Java/
--rw-r--r--   0 buffer     (502) staff       (20)     1114 2022-12-28 14:31:40.000000 thug-5.2/thug/Java/System.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Java/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      763 2022-12-28 14:31:40.000000 thug-5.2/thug/Java/java.py
--rw-r--r--   0 buffer     (502) staff       (20)      771 2022-12-28 14:31:40.000000 thug-5.2/thug/Java/lang.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.184098 thug-5.2/thug/Logging/
--rw-r--r--   0 buffer     (502) staff       (20)     2454 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/BaseLogging.py
--rw-r--r--   0 buffer     (502) staff       (20)     3893 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/Features.py
--rw-r--r--   0 buffer     (502) staff       (20)      920 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/LoggingModules.py
--rw-r--r--   0 buffer     (502) staff       (20)     5106 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/SampleLogging.py
--rw-r--r--   0 buffer     (502) staff       (20)    14604 2023-01-03 10:16:05.000000 thug-5.2/thug/Logging/ThugLogging.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.189151 thug-5.2/thug/Logging/modules/
--rw-r--r--   0 buffer     (502) staff       (20)     2565 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/modules/ElasticSearch.py
--rw-r--r--   0 buffer     (502) staff       (20)     1301 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/modules/ExploitGraph.py
--rw-r--r--   0 buffer     (502) staff       (20)    14581 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/modules/JSON.py
--rw-r--r--   0 buffer     (502) staff       (20)    10438 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/modules/Mapper.py
--rw-r--r--   0 buffer     (502) staff       (20)    16889 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/modules/MongoDB.py
--rw-r--r--   0 buffer     (502) staff       (20)       83 2022-12-28 14:31:40.000000 thug-5.2/thug/Logging/modules/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.190718 thug-5.2/thug/Magic/
--rw-r--r--   0 buffer     (502) staff       (20)     1593 2022-12-28 14:31:40.000000 thug-5.2/thug/Magic/Magic.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Magic/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.191927 thug-5.2/thug/OS/
--rw-r--r--   0 buffer     (502) staff       (20)     4912 2022-12-28 14:31:40.000000 thug-5.2/thug/OS/Windows.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/OS/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.194448 thug-5.2/thug/Plugins/
--rw-r--r--   0 buffer     (502) staff       (20)      956 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/IPlugin.py
--rw-r--r--   0 buffer     (502) staff       (20)     3401 2023-01-03 10:15:59.000000 thug-5.2/thug/Plugins/ThugPlugins.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.194936 thug-5.2/thug/Plugins/plugins/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.196175 thug-5.2/thug/Plugins/plugins/POST-TestPlugin-999/
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.197662 thug-5.2/thug/Plugins/plugins/PRE-TestPlugin-999/
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/Plugins/plugins/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.204274 thug-5.2/thug/ThugAPI/
--rw-r--r--   0 buffer     (502) staff       (20)    18741 2023-03-07 14:57:11.000000 thug-5.2/thug/ThugAPI/IThugAPI.py
--rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.2/thug/ThugAPI/OpaqueFilter.py
--rw-r--r--   0 buffer     (502) staff       (20)    16007 2023-03-07 14:57:11.000000 thug-5.2/thug/ThugAPI/ThugAPI.py
--rw-r--r--   0 buffer     (502) staff       (20)     9649 2023-03-07 14:57:11.000000 thug-5.2/thug/ThugAPI/ThugOpts.py
--rw-r--r--   0 buffer     (502) staff       (20)     4203 2022-12-28 14:31:40.000000 thug-5.2/thug/ThugAPI/ThugVulnModules.py
--rw-r--r--   0 buffer     (502) staff       (20)     1642 2022-12-28 14:31:40.000000 thug-5.2/thug/ThugAPI/Watchdog.py
--rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.2/thug/ThugAPI/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      317 2022-12-28 14:31:40.000000 thug-5.2/thug/ThugAPI/abstractmethod.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.206389 thug-5.2/thug/WebTracking/
--rw-r--r--   0 buffer     (502) staff       (20)     3206 2022-12-28 14:31:40.000000 thug-5.2/thug/WebTracking/Cookies.py
--rw-r--r--   0 buffer     (502) staff       (20)     1176 2022-12-28 14:31:40.000000 thug-5.2/thug/WebTracking/WebStorage.py
--rw-r--r--   0 buffer     (502) staff       (20)     1596 2022-12-28 14:31:40.000000 thug-5.2/thug/WebTracking/WebTracking.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/WebTracking/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)     2024 2023-06-20 07:40:52.000000 thug-5.2/thug/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.207843 thug-5.2/thug/conf/
--rw-r--r--   0 buffer     (502) staff       (20)     6148 2022-11-04 15:21:57.000000 thug-5.2/thug/conf/.DS_Store
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.208601 thug-5.2/thug/conf/hooks/
--rw-r--r--   0 buffer     (502) staff       (20)       45 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/hooks/README
--rw-r--r--   0 buffer     (502) staff       (20)      174 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/inspector.json
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.232245 thug-5.2/thug/conf/personalities/
--rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/galaxy2chrome18.json
--rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/galaxy2chrome25.json
--rw-r--r--   0 buffer     (502) staff       (20)      743 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/galaxy2chrome29.json
--rw-r--r--   0 buffer     (502) staff       (20)      793 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome33.json
--rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome35.json
--rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome37.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome38.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome39.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome45.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome46.json
--rw-r--r--   0 buffer     (502) staff       (20)      729 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadchrome47.json
--rw-r--r--   0 buffer     (502) staff       (20)      692 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadsafari7.json
--rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadsafari8.json
--rw-r--r--   0 buffer     (502) staff       (20)      680 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/ipadsafari9.json
--rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxchrome26.json
--rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxchrome30.json
--rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxchrome44.json
--rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxchrome54.json
--rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxchrome98.json
--rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxfirefox19.json
--rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/linuxfirefox40.json
--rw-r--r--   0 buffer     (502) staff       (20)      748 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/nexuschrome18.json
--rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/osx10chrome19.json
--rw-r--r--   0 buffer     (502) staff       (20)      690 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/osx10chrome80.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/osx10chrome97.json
--rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/osx10safari5.json
--rw-r--r--   0 buffer     (502) staff       (20)      682 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/osx11safari14.json
--rw-r--r--   0 buffer     (502) staff       (20)      396 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/prefix_allocation.txt
--rw-r--r--   0 buffer     (502) staff       (20)     2851 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win10edge20.json.review
--rw-r--r--   0 buffer     (502) staff       (20)     3826 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win10ie110.json
--rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win2kie60.json
--rw-r--r--   0 buffer     (502) staff       (20)      915 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win2kie80.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7chrome20.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7chrome40.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7chrome45.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7chrome49.json
--rw-r--r--   0 buffer     (502) staff       (20)      579 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7firefox3.json
--rw-r--r--   0 buffer     (502) staff       (20)     3769 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7ie100.json
--rw-r--r--   0 buffer     (502) staff       (20)     3800 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7ie80.json
--rw-r--r--   0 buffer     (502) staff       (20)     3820 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7ie90.json
--rw-r--r--   0 buffer     (502) staff       (20)      678 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/win7safari5.json
--rw-r--r--   0 buffer     (502) staff       (20)      674 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpchrome20.json
--rw-r--r--   0 buffer     (502) staff       (20)      564 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpfirefox12.json
--rw-r--r--   0 buffer     (502) staff       (20)     2876 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpie60.json
--rw-r--r--   0 buffer     (502) staff       (20)     2896 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpie61.json
--rw-r--r--   0 buffer     (502) staff       (20)     2871 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpie70.json
--rw-r--r--   0 buffer     (502) staff       (20)     2968 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpie80.json
--rw-r--r--   0 buffer     (502) staff       (20)      666 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/personalities/winxpsafari5.json
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.232972 thug-5.2/thug/conf/plugins/
--rw-r--r--   0 buffer     (502) staff       (20)       47 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/plugins/README
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.240433 thug-5.2/thug/conf/rules/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.240846 thug-5.2/thug/conf/rules/cookieclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/cookieclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/cookieclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.241888 thug-5.2/thug/conf/rules/cookiefilter/
--rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/cookiefilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/cookiefilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.242661 thug-5.2/thug/conf/rules/htmlclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/htmlclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/htmlclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.243655 thug-5.2/thug/conf/rules/htmlfilter/
--rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/htmlfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/htmlfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.244782 thug-5.2/thug/conf/rules/imageclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/imageclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/imageclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.245665 thug-5.2/thug/conf/rules/imagefilter/
--rw-r--r--   0 buffer     (502) staff       (20)      103 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/imagefilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/imagefilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.246559 thug-5.2/thug/conf/rules/jsclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      245 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/jsclassifier/plugindetect.yar
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/jsclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.247542 thug-5.2/thug/conf/rules/jsfilter/
--rw-r--r--   0 buffer     (502) staff       (20)       97 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/jsfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/jsfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.248470 thug-5.2/thug/conf/rules/sampleclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/sampleclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/sampleclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.249375 thug-5.2/thug/conf/rules/samplefilter/
--rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/samplefilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/samplefilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.250268 thug-5.2/thug/conf/rules/textclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/textclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/textclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.251180 thug-5.2/thug/conf/rules/textfilter/
--rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/textfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/textfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.265497 thug-5.2/thug/conf/rules/urlclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)     3005 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/blackhole.yar
--rw-r--r--   0 buffer     (502) staff       (20)      418 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/cool.yar
--rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/crimeboss.yar
--rw-r--r--   0 buffer     (502) staff       (20)      641 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/critxpack.yar
--rw-r--r--   0 buffer     (502) staff       (20)     1000 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/fiesta.yar
--rw-r--r--   0 buffer     (502) staff       (20)      870 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/g01pack.yar
--rw-r--r--   0 buffer     (502) staff       (20)      387 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/impact.yar
--rw-r--r--   0 buffer     (502) staff       (20)      808 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/neutrino.yar
--rw-r--r--   0 buffer     (502) staff       (20)      612 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/nuclear.yar
--rw-r--r--   0 buffer     (502) staff       (20)      969 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/popads.yar
--rw-r--r--   0 buffer     (502) staff       (20)      765 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/redkit.yar
--rw-r--r--   0 buffer     (502) staff       (20)      427 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/safepack.yar
--rw-r--r--   0 buffer     (502) staff       (20)      176 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/sakura.yar
--rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/sofosfo.yar
--rw-r--r--   0 buffer     (502) staff       (20)     2400 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/styx.yar
--rw-r--r--   0 buffer     (502) staff       (20)      849 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/sweetorange.yar
--rw-r--r--   0 buffer     (502) staff       (20)      340 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier/tds.yar
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.266383 thug-5.2/thug/conf/rules/urlfilter/
--rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/urlfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.266922 thug-5.2/thug/conf/rules/vbsclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/vbsclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/vbsclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.267629 thug-5.2/thug/conf/rules/vbsfilter/
--rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/vbsfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/rules/vbsfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:58.270703 thug-5.2/thug/conf/scripts/
--rw-r--r--   0 buffer     (502) staff       (20)       69 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/scripts/date.js
--rw-r--r--   0 buffer     (502) staff       (20)      197 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/scripts/eval.js
--rw-r--r--   0 buffer     (502) staff       (20)       87 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/scripts/message-event.js
--rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/scripts/storage.js
--rw-r--r--   0 buffer     (502) staff       (20)      753 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/scripts/thug.js
--rw-r--r--   0 buffer     (502) staff       (20)      205 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/scripts/write.js
--rw-r--r--   0 buffer     (502) staff       (20)      325 2022-12-28 14:31:40.000000 thug-5.2/thug/conf/thug.conf
--rw-r--r--   0 buffer     (502) staff       (20)    17085 2023-03-07 14:57:11.000000 thug-5.2/thug/thug.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-06-20 07:50:57.828055 thug-5.2/thug.egg-info/
--rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer     (502) staff       (20)    15813 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer     (502) staff       (20)        1 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer     (502) staff       (20)       40 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer     (502) staff       (20)      507 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/requires.txt
--rw-r--r--   0 buffer     (502) staff       (20)        5 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer     (502) staff       (20)        1 2023-06-20 07:50:57.000000 thug-5.2/thug.egg-info/zip-safe
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.454232 thug-5.3/
+-rw-r--r--   0 buffer     (502) staff       (20)    17987 2022-12-28 14:31:40.000000 thug-5.3/LICENSE.txt
+-rw-r--r--   0 buffer     (502) staff       (20)      130 2023-01-03 13:39:45.000000 thug-5.3/MANIFEST.in
+-rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-07-19 08:14:57.452775 thug-5.3/PKG-INFO
+-rw-r--r--   0 buffer     (502) staff       (20)     2676 2023-01-17 09:44:55.000000 thug-5.3/README.rst
+-rw-r--r--   0 buffer     (502) staff       (20)     3458 2023-07-14 13:36:11.000000 thug-5.3/pyproject.toml
+-rw-r--r--   0 buffer     (502) staff       (20)      339 2023-07-14 13:36:23.000000 thug-5.3/requirements.txt
+-rw-r--r--   0 buffer     (502) staff       (20)       38 2023-07-19 08:14:57.454400 thug-5.3/setup.cfg
+-rw-r--r--   0 buffer     (502) staff       (20)     1346 2023-01-03 12:33:41.000000 thug-5.3/setup.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:56.927108 thug-5.3/thug/
+-rw-r--r--   0 buffer     (502) staff       (20)     8196 2022-11-04 15:21:57.000000 thug-5.3/thug/.DS_Store
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:56.940412 thug-5.3/thug/ActiveX/
+-rw-r--r--   0 buffer     (502) staff       (20)     7598 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/ActiveX.py
+-rw-r--r--   0 buffer     (502) staff       (20)    64018 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/CLSID.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.069227 thug-5.3/thug/ActiveX/modules/
+-rw-r--r--   0 buffer     (502) staff       (20)      400 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AOLAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1119 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AcroPDF.py
+-rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AdodbRecordset.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2573 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AdodbStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1482 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AnswerWorks.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1086 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AolAmpX.py
+-rw-r--r--   0 buffer     (502) staff       (20)      979 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/AolICQ.py
+-rw-r--r--   0 buffer     (502) staff       (20)      801 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/BaiduBar.py
+-rw-r--r--   0 buffer     (502) staff       (20)      567 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/BitDefender.py
+-rw-r--r--   0 buffer     (502) staff       (20)      421 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/CABrightStor.py
+-rw-r--r--   0 buffer     (502) staff       (20)      600 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/CGAgent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      726 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Comodo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ConnectAndEnterRoom.py
+-rw-r--r--   0 buffer     (502) staff       (20)      307 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/CreativeSoftAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/DLinkMPEG.py
+-rw-r--r--   0 buffer     (502) staff       (20)      673 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/DPClient.py
+-rw-r--r--   0 buffer     (502) staff       (20)      447 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/DVRHOSTWeb.py
+-rw-r--r--   0 buffer     (502) staff       (20)      625 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/DirectShow.py
+-rw-r--r--   0 buffer     (502) staff       (20)      404 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/DivX.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1857 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Domino.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1500 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/EnjoySAP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      825 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/FacebookPhotoUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3049 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/File.py
+-rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/FileUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2221 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Folder.py
+-rw-r--r--   0 buffer     (502) staff       (20)      496 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/GLIEDown2.py
+-rw-r--r--   0 buffer     (502) staff       (20)      656 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/GatewayWeblaunch.py
+-rw-r--r--   0 buffer     (502) staff       (20)      420 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Gogago.py
+-rw-r--r--   0 buffer     (502) staff       (20)      561 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/GomWeb.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4119 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/HPInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      443 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ICQToolbar.py
+-rw-r--r--   0 buffer     (502) staff       (20)      945 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/IMWebControl.py
+-rw-r--r--   0 buffer     (502) staff       (20)      672 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/InternetCleverSuite.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1964 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/JavaDeploymentToolkit.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
+-rw-r--r--   0 buffer     (502) staff       (20)      405 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Kingsoft.py
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/MSRICHTXT.py
+-rw-r--r--   0 buffer     (502) staff       (20)      601 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/MSVFP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      535 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/MSXML2DOMDocument.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4390 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/MacrovisionFlexNet.py
+-rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/MicrosoftWorks7Attack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2048 2023-01-13 08:09:32.000000 thug-5.3/thug/ActiveX/modules/MicrosoftXMLDOM.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8006 2023-01-06 14:50:41.000000 thug-5.3/thug/ActiveX/modules/MicrosoftXMLHTTP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      466 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Move.py
+-rw-r--r--   0 buffer     (502) staff       (20)      438 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/MyspaceUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)      589 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/NCTAudioFile2.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1259 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/NamoInstaller.py
+-rw-r--r--   0 buffer     (502) staff       (20)      616 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/NeoTracePro.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3311 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/NessusScanCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1175 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/OfficeOCX.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1057 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/OurgameGLWorld.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1201 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/PPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      498 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/PTZCamPanel.py
+-rw-r--r--   0 buffer     (502) staff       (20)      494 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/QuantumStreaming.py
+-rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/QvodCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)      973 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/RDSDataSpace.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2335 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/RealPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      348 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/RediffBolDownloaderAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)      831 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/RegistryPro.py
+-rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/RisingScanner.py
+-rw-r--r--   0 buffer     (502) staff       (20)      449 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/RtspVaPgCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1116 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SSReaderPdg2.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1027 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ScriptingDictionary.py
+-rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ScriptingEncoder.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5185 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ScriptingFileSystemObject.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1527 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ShellApplication.py
+-rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Shockwave.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ShockwaveFlash10.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ShockwaveFlash11.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ShockwaveFlash12.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ShockwaveFlash9.py
+-rw-r--r--   0 buffer     (502) staff       (20)      273 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SilverLight.py
+-rw-r--r--   0 buffer     (502) staff       (20)      921 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SinaDLoader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1472 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SnapshotViewer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      715 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
+-rw-r--r--   0 buffer     (502) staff       (20)      906 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Spreadsheet.py
+-rw-r--r--   0 buffer     (502) staff       (20)      677 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/StormConfig.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2436 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/StormMps.py
+-rw-r--r--   0 buffer     (502) staff       (20)      516 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/StreamAudioChainCast.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1061 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SymantecAppStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2224 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/SymantecBackupExec.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4772 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/TextStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/Toshiba.py
+-rw-r--r--   0 buffer     (502) staff       (20)      391 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/UUSeeUpdate.py
+-rw-r--r--   0 buffer     (502) staff       (20)      691 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/UniversalUpload.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1763 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/VLC.py
+-rw-r--r--   0 buffer     (502) staff       (20)      719 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/VisualStudioDTE80.py
+-rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/VsaIDEDTE.py
+-rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/VsmIDEDTE.py
+-rw-r--r--   0 buffer     (502) staff       (20)      796 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WMEncProfileManager.py
+-rw-r--r--   0 buffer     (502) staff       (20)      132 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WMP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WScriptCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1280 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WScriptExec.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1689 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WScriptNetwork.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8980 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WScriptShell.py
+-rw-r--r--   0 buffer     (502) staff       (20)      213 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WScriptShortcut.py
+-rw-r--r--   0 buffer     (502) staff       (20)      645 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WebViewFolderIcon.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1373 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WinNTSystemInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      599 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WinZip.py
+-rw-r--r--   0 buffer     (502) staff       (20)      145 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/WindowsMediaPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      942 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/XMLDOMParseError.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1026 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/XUpload.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1159 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/YahooJukebox.py
+-rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/YahooMessengerCyft.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1077 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/YahooMessengerYVerInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1244 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/YahooMessengerYwcvwr.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1932 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2870 2022-12-28 14:31:40.000000 thug-5.3/thug/ActiveX/modules/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.070174 thug-5.3/thug/Analysis/
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.071930 thug-5.3/thug/Analysis/awis/
+-rw-r--r--   0 buffer     (502) staff       (20)     3224 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/awis/AWIS.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/awis/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.073801 thug-5.3/thug/Analysis/context/
+-rw-r--r--   0 buffer     (502) staff       (20)     1554 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/context/ContextAnalyzer.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/context/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.075597 thug-5.3/thug/Analysis/honeyagent/
+-rw-r--r--   0 buffer     (502) staff       (20)     4000 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/honeyagent/HoneyAgent.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/honeyagent/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.077228 thug-5.3/thug/Analysis/screenshot/
+-rw-r--r--   0 buffer     (502) staff       (20)     1333 2023-03-07 14:57:11.000000 thug-5.3/thug/Analysis/screenshot/Screenshot.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/screenshot/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.079063 thug-5.3/thug/Analysis/shellcode/
+-rw-r--r--   0 buffer     (502) staff       (20)     8069 2023-01-13 08:09:32.000000 thug-5.3/thug/Analysis/shellcode/Shellcode.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Analysis/shellcode/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.089746 thug-5.3/thug/Classifier/
+-rw-r--r--   0 buffer     (502) staff       (20)     5017 2023-03-28 13:07:55.000000 thug-5.3/thug/Classifier/BaseClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2106 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/CookieClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2159 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/HTMLClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2070 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/ImageClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2008 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/JSClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2243 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/SampleClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2082 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/TextClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2331 2023-07-19 07:06:40.000000 thug-5.3/thug/Classifier/URLClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2014 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/VBSClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Classifier/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.165609 thug-5.3/thug/DOM/
+-rw-r--r--   0 buffer     (502) staff       (20)     2534 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Alexa.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2289 2023-03-28 10:08:11.000000 thug-5.3/thug/DOM/AsyncPrefetcher.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2254 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/CCInterpreter.py
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Chrome.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1304 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/ClipboardData.py
+-rw-r--r--   0 buffer     (502) staff       (20)      817 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Components.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5901 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Console.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1112 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Crypto.py
+-rw-r--r--   0 buffer     (502) staff       (20)    54552 2023-07-19 07:06:40.000000 thug-5.3/thug/DOM/DFT.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3602 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/External.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2776 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/HTMLInspector.py
+-rw-r--r--   0 buffer     (502) staff       (20)    10112 2023-07-19 07:06:40.000000 thug-5.3/thug/DOM/HTTPSession.py
+-rw-r--r--   0 buffer     (502) staff       (20)      932 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/HTTPSessionException.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3593 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/History.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3506 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/JSClass.py
+-rw-r--r--   0 buffer     (502) staff       (20)     7824 2023-01-06 16:11:13.000000 thug-5.3/thug/DOM/JSEngine.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4502 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/JSInspector.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5959 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/JScriptEncode.py
+-rw-r--r--   0 buffer     (502) staff       (20)      752 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/LocalStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4670 2023-07-19 07:06:40.000000 thug-5.3/thug/DOM/Location.py
+-rw-r--r--   0 buffer     (502) staff       (20)    19549 2023-02-27 08:54:28.000000 thug-5.3/thug/DOM/MIMEHandler.py
+-rw-r--r--   0 buffer     (502) staff       (20)      762 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Map.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/MimeType.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5282 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/MimeTypes.py
+-rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/MozConnection.py
+-rw-r--r--   0 buffer     (502) staff       (20)    13340 2023-03-07 14:57:11.000000 thug-5.3/thug/DOM/Navigator.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4056 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Personality.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1233 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Plugin.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1471 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Plugins.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1069 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/SchemeHandler.py
+-rw-r--r--   0 buffer     (502) staff       (20)     6150 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Screen.py
+-rw-r--r--   0 buffer     (502) staff       (20)      756 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/SessionStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1750 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Sidebar.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3502 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Storage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3216 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/UserProfile.py
+-rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/Utils.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.180417 thug-5.3/thug/DOM/W3C/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.218917 thug-5.3/thug/DOM/W3C/Core/
+-rw-r--r--   0 buffer     (502) staff       (20)     2138 2023-01-06 12:37:35.000000 thug-5.3/thug/DOM/W3C/Core/Attr.py
+-rw-r--r--   0 buffer     (502) staff       (20)      265 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/CDATASection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1241 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Core/CharacterData.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3531 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Core/ClassList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      564 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/Comment.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1910 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Core/DOMException.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5765 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/DOMImplementation.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8868 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/Document.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2412 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/DocumentFragment.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1513 2023-01-06 12:31:24.000000 thug-5.3/thug/DOM/W3C/Core/DocumentType.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9544 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/Element.py
+-rw-r--r--   0 buffer     (502) staff       (20)      457 2023-01-06 12:38:21.000000 thug-5.3/thug/DOM/W3C/Core/Entity.py
+-rw-r--r--   0 buffer     (502) staff       (20)      501 2023-01-06 12:38:52.000000 thug-5.3/thug/DOM/W3C/Core/EntityReference.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Core/NamedNodeMap.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14464 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/Node.py
+-rw-r--r--   0 buffer     (502) staff       (20)      569 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/NodeList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      474 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/NodeType.py
+-rw-r--r--   0 buffer     (502) staff       (20)      485 2023-01-06 12:34:08.000000 thug-5.3/thug/DOM/W3C/Core/Notation.py
+-rw-r--r--   0 buffer     (502) staff       (20)      510 2023-01-06 12:34:27.000000 thug-5.3/thug/DOM/W3C/Core/ProcessingInstruction.py
+-rw-r--r--   0 buffer     (502) staff       (20)      803 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/Text.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1051 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Core/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      337 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Core/abstractmethod.py
+-rw-r--r--   0 buffer     (502) staff       (20)      274 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/DOMParser.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1454 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/DOMTokenList.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.236754 thug-5.3/thug/DOM/W3C/Events/
+-rw-r--r--   0 buffer     (502) staff       (20)      868 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/DocumentEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4120 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/Event.py
+-rw-r--r--   0 buffer     (502) staff       (20)      525 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/EventException.py
+-rw-r--r--   0 buffer     (502) staff       (20)      272 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/EventListener.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9134 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/EventTarget.py
+-rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/HTMLEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1206 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/MessageEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2198 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/MouseEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1575 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/MutationEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/StorageEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      636 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Events/UIEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      691 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/Events/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.241845 thug-5.3/thug/DOM/W3C/File/
+-rw-r--r--   0 buffer     (502) staff       (20)     2433 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/File/Blob.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1381 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/File/File.py
+-rw-r--r--   0 buffer     (502) staff       (20)       85 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/File/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.309200 thug-5.3/thug/DOM/W3C/HTML/
+-rw-r--r--   0 buffer     (502) staff       (20)      194 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/AudioTrackList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/Dataset.py
+-rw-r--r--   0 buffer     (502) staff       (20)      374 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLAllCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1922 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLAnchorElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      654 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLAppletElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLAudioElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      252 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLBRElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLBaseElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      331 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1486 2023-04-11 09:54:20.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLBodyElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      582 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLButtonElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1281 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)      265 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLDListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      263 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLDivElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)    15982 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLDocument.py
+-rw-r--r--   0 buffer     (502) staff       (20)      955 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      412 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4141 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      322 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLFontElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1742 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLFormElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      978 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLFrameElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      289 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      407 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLHRElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLHeadElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLHeadingElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLHtmlElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1300 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLIFrameElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1302 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLImageElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1466 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLInputElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      277 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLLIElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      373 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLLabelElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      376 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLLegendElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      558 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLLinkElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4216 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLMediaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      264 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLMenuElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      667 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLMetaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      296 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLModElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLOListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2595 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLObjectElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      343 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLOptionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      227 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)      259 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLParagraphElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLParamElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLPreElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLQuoteElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      988 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLScriptElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1636 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLSelectElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      177 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLSpanElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      316 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLStyleElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      262 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      917 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTableCellElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTableColElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4711 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTableElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2800 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTableRowElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2091 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1031 2022-12-30 12:26:43.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLTitleElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/HTMLUListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/TAnimateColor.py
+-rw-r--r--   0 buffer     (502) staff       (20)      280 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/TextTrackList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      681 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/TimeRanges.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5132 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      442 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/attr_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      426 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/bool_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      436 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/HTML/form_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      806 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/HTML/text_property.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.309678 thug-5.3/thug/DOM/W3C/Style/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.311027 thug-5.3/thug/DOM/W3C/Style/CSS/
+-rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
+-rw-r--r--   0 buffer     (502) staff       (20)      425 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Style/CSS/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Style/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.312662 thug-5.3/thug/DOM/W3C/URL/
+-rw-r--r--   0 buffer     (502) staff       (20)     4843 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/URL/URL.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2710 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/URL/URLSearchParams.py
+-rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/URL/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.314423 thug-5.3/thug/DOM/W3C/Views/
+-rw-r--r--   0 buffer     (502) staff       (20)      217 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Views/AbstractView.py
+-rw-r--r--   0 buffer     (502) staff       (20)      211 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Views/DocumentView.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/Views/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)       56 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/W3C/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      367 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/W3C/w3c.py
+-rw-r--r--   0 buffer     (502) staff       (20)      829 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/WebStore.py
+-rw-r--r--   0 buffer     (502) staff       (20)    35015 2023-01-13 08:09:32.000000 thug-5.3/thug/DOM/Window.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)     7624 2022-12-28 14:31:40.000000 thug-5.3/thug/DOM/w3c_bindings.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.316496 thug-5.3/thug/Encoding/
+-rw-r--r--   0 buffer     (502) staff       (20)      877 2022-12-28 14:31:40.000000 thug-5.3/thug/Encoding/Encoding.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Encoding/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.319750 thug-5.3/thug/Java/
+-rw-r--r--   0 buffer     (502) staff       (20)     1114 2022-12-28 14:31:40.000000 thug-5.3/thug/Java/System.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Java/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      763 2022-12-28 14:31:40.000000 thug-5.3/thug/Java/java.py
+-rw-r--r--   0 buffer     (502) staff       (20)      771 2022-12-28 14:31:40.000000 thug-5.3/thug/Java/lang.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.325706 thug-5.3/thug/Logging/
+-rw-r--r--   0 buffer     (502) staff       (20)     2454 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/BaseLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3893 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/Features.py
+-rw-r--r--   0 buffer     (502) staff       (20)      920 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/LoggingModules.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5106 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/SampleLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14604 2023-01-03 10:16:05.000000 thug-5.3/thug/Logging/ThugLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.331051 thug-5.3/thug/Logging/modules/
+-rw-r--r--   0 buffer     (502) staff       (20)     2758 2023-06-21 16:13:14.000000 thug-5.3/thug/Logging/modules/ElasticSearch.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1301 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/modules/ExploitGraph.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14581 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/modules/JSON.py
+-rw-r--r--   0 buffer     (502) staff       (20)    10438 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/modules/Mapper.py
+-rw-r--r--   0 buffer     (502) staff       (20)    16889 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/modules/MongoDB.py
+-rw-r--r--   0 buffer     (502) staff       (20)       83 2022-12-28 14:31:40.000000 thug-5.3/thug/Logging/modules/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.333704 thug-5.3/thug/Magic/
+-rw-r--r--   0 buffer     (502) staff       (20)     1593 2022-12-28 14:31:40.000000 thug-5.3/thug/Magic/Magic.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Magic/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.335219 thug-5.3/thug/OS/
+-rw-r--r--   0 buffer     (502) staff       (20)     4912 2022-12-28 14:31:40.000000 thug-5.3/thug/OS/Windows.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/OS/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.338624 thug-5.3/thug/Plugins/
+-rw-r--r--   0 buffer     (502) staff       (20)      956 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/IPlugin.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3401 2023-01-03 10:15:59.000000 thug-5.3/thug/Plugins/ThugPlugins.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.339211 thug-5.3/thug/Plugins/plugins/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.340864 thug-5.3/thug/Plugins/plugins/POST-TestPlugin-999/
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.342398 thug-5.3/thug/Plugins/plugins/PRE-TestPlugin-999/
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/Plugins/plugins/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.349807 thug-5.3/thug/ThugAPI/
+-rw-r--r--   0 buffer     (502) staff       (20)    18741 2023-03-07 14:57:11.000000 thug-5.3/thug/ThugAPI/IThugAPI.py
+-rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.3/thug/ThugAPI/OpaqueFilter.py
+-rw-r--r--   0 buffer     (502) staff       (20)    16007 2023-03-07 14:57:11.000000 thug-5.3/thug/ThugAPI/ThugAPI.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9649 2023-03-07 14:57:11.000000 thug-5.3/thug/ThugAPI/ThugOpts.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4203 2022-12-28 14:31:40.000000 thug-5.3/thug/ThugAPI/ThugVulnModules.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1642 2022-12-28 14:31:40.000000 thug-5.3/thug/ThugAPI/Watchdog.py
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.3/thug/ThugAPI/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      317 2022-12-28 14:31:40.000000 thug-5.3/thug/ThugAPI/abstractmethod.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.352483 thug-5.3/thug/WebTracking/
+-rw-r--r--   0 buffer     (502) staff       (20)     3206 2022-12-28 14:31:40.000000 thug-5.3/thug/WebTracking/Cookies.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1176 2022-12-28 14:31:40.000000 thug-5.3/thug/WebTracking/WebStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1596 2022-12-28 14:31:40.000000 thug-5.3/thug/WebTracking/WebTracking.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/WebTracking/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2024 2023-07-19 07:57:36.000000 thug-5.3/thug/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.354719 thug-5.3/thug/conf/
+-rw-r--r--   0 buffer     (502) staff       (20)     6148 2022-11-04 15:21:57.000000 thug-5.3/thug/conf/.DS_Store
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.355553 thug-5.3/thug/conf/hooks/
+-rw-r--r--   0 buffer     (502) staff       (20)       45 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/hooks/README
+-rw-r--r--   0 buffer     (502) staff       (20)      174 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/inspector.json
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.401623 thug-5.3/thug/conf/personalities/
+-rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/galaxy2chrome18.json
+-rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/galaxy2chrome25.json
+-rw-r--r--   0 buffer     (502) staff       (20)      743 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/galaxy2chrome29.json
+-rw-r--r--   0 buffer     (502) staff       (20)      793 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome33.json
+-rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome35.json
+-rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome37.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome38.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome39.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome45.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome46.json
+-rw-r--r--   0 buffer     (502) staff       (20)      729 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadchrome47.json
+-rw-r--r--   0 buffer     (502) staff       (20)      692 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadsafari7.json
+-rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadsafari8.json
+-rw-r--r--   0 buffer     (502) staff       (20)      680 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/ipadsafari9.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxchrome26.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxchrome30.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxchrome44.json
+-rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxchrome54.json
+-rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxchrome98.json
+-rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxfirefox19.json
+-rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/linuxfirefox40.json
+-rw-r--r--   0 buffer     (502) staff       (20)      748 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/nexuschrome18.json
+-rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/osx10chrome19.json
+-rw-r--r--   0 buffer     (502) staff       (20)      690 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/osx10chrome80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/osx10chrome97.json
+-rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/osx10safari5.json
+-rw-r--r--   0 buffer     (502) staff       (20)      682 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/osx11safari14.json
+-rw-r--r--   0 buffer     (502) staff       (20)      396 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/prefix_allocation.txt
+-rw-r--r--   0 buffer     (502) staff       (20)     2851 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win10edge20.json.review
+-rw-r--r--   0 buffer     (502) staff       (20)     3826 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win10ie110.json
+-rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win2kie60.json
+-rw-r--r--   0 buffer     (502) staff       (20)      915 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win2kie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7chrome20.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7chrome40.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7chrome45.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7chrome49.json
+-rw-r--r--   0 buffer     (502) staff       (20)      579 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7firefox3.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3769 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7ie100.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3800 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7ie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3820 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7ie90.json
+-rw-r--r--   0 buffer     (502) staff       (20)      678 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/win7safari5.json
+-rw-r--r--   0 buffer     (502) staff       (20)      674 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpchrome20.json
+-rw-r--r--   0 buffer     (502) staff       (20)      564 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpfirefox12.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2876 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpie60.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2896 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpie61.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2871 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpie70.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2968 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      666 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/personalities/winxpsafari5.json
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.402285 thug-5.3/thug/conf/plugins/
+-rw-r--r--   0 buffer     (502) staff       (20)       47 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/plugins/README
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.410397 thug-5.3/thug/conf/rules/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.410779 thug-5.3/thug/conf/rules/cookieclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/cookieclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/cookieclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.411859 thug-5.3/thug/conf/rules/cookiefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/cookiefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/cookiefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.412605 thug-5.3/thug/conf/rules/htmlclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/htmlclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/htmlclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.413713 thug-5.3/thug/conf/rules/htmlfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/htmlfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/htmlfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.414436 thug-5.3/thug/conf/rules/imageclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/imageclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/imageclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.415655 thug-5.3/thug/conf/rules/imagefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      103 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/imagefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/imagefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.416679 thug-5.3/thug/conf/rules/jsclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      245 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/jsclassifier/plugindetect.yar
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/jsclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.417622 thug-5.3/thug/conf/rules/jsfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       97 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/jsfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/jsfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.418597 thug-5.3/thug/conf/rules/sampleclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/sampleclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/sampleclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.419457 thug-5.3/thug/conf/rules/samplefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/samplefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/samplefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.420410 thug-5.3/thug/conf/rules/textclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/textclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/textclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.421399 thug-5.3/thug/conf/rules/textfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/textfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/textfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.442582 thug-5.3/thug/conf/rules/urlclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)     3005 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/blackhole.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      418 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/cool.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/crimeboss.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      641 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/critxpack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)     1000 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/fiesta.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      870 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/g01pack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      387 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/impact.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      808 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/neutrino.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      612 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/nuclear.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      969 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/popads.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      765 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/redkit.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      427 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/safepack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      176 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/sakura.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/sofosfo.yar
+-rw-r--r--   0 buffer     (502) staff       (20)     2400 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/styx.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      849 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/sweetorange.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      340 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier/tds.yar
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.443669 thug-5.3/thug/conf/rules/urlfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/urlfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.444673 thug-5.3/thug/conf/rules/vbsclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/vbsclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/vbsclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.445620 thug-5.3/thug/conf/rules/vbsfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/vbsfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/rules/vbsfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:57.451881 thug-5.3/thug/conf/scripts/
+-rw-r--r--   0 buffer     (502) staff       (20)       69 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/scripts/date.js
+-rw-r--r--   0 buffer     (502) staff       (20)      197 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/scripts/eval.js
+-rw-r--r--   0 buffer     (502) staff       (20)       87 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/scripts/message-event.js
+-rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/scripts/storage.js
+-rw-r--r--   0 buffer     (502) staff       (20)      753 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/scripts/thug.js
+-rw-r--r--   0 buffer     (502) staff       (20)      205 2022-12-28 14:31:40.000000 thug-5.3/thug/conf/scripts/write.js
+-rw-r--r--   0 buffer     (502) staff       (20)      325 2023-06-21 15:23:50.000000 thug-5.3/thug/conf/thug.conf
+-rw-r--r--   0 buffer     (502) staff       (20)    17085 2023-03-07 14:57:11.000000 thug-5.3/thug/thug.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-07-19 08:14:56.935622 thug-5.3/thug.egg-info/
+-rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/PKG-INFO
+-rw-r--r--   0 buffer     (502) staff       (20)    15813 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        1 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 buffer     (502) staff       (20)       40 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/entry_points.txt
+-rw-r--r--   0 buffer     (502) staff       (20)      487 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/requires.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        5 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/top_level.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        1 2023-07-19 08:14:56.000000 thug-5.3/thug.egg-info/zip-safe
```

### Comparing `thug-5.2/LICENSE.txt` & `thug-5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thug-5.2/PKG-INFO` & `thug-5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 5.2
+Version: 5.3
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
```

### Comparing `thug-5.2/README.rst` & `thug-5.3/README.rst`

 * *Files identical despite different names*

### Comparing `thug-5.2/pyproject.toml` & `thug-5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
 ]
 dependencies = [
     "appdirs==1.4.4",
     "beautifulsoup4==4.12.2",
-    "charset-normalizer==3.1.0",
+    "charset-normalizer==3.2.0",
     "cssutils==2.7.1",
     "html5lib==1.1",
-    "lxml==4.9.2",
+    "lxml==4.9.3",
     "networkx==3.1",
     "pefile==2023.2.7",
     "promise==2.3",
     "pylibemu==0.8",
-    "pymongo==4.3.3",
+    "pymongo==4.4.1",
     "pysocks==1.7.1",
     "python-magic==0.4.27",
     "rarfile==4.0",
     "requests==2.31.0",
     "requests-futures==1.0.1",
     "setuptools>=65.5.1",
     "ssdeep==3.4",
@@ -62,16 +62,15 @@
     "low-interaction",
     "client-honeypot",
     "security-tools",
 ]
 
 [project.optional-dependencies]
 test = [
-    "elasticmock",
-    "elasticsearch==7.17.9",
+    "elasticsearch",
     "imgkit==1.1.0",
     "mock",
     "mongomock",
     "pre-commit",
     "pygraphviz",
     "pytesseract",
     "pytest",
```

### Comparing `thug-5.2/setup.py` & `thug-5.3/setup.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/.DS_Store` & `thug-5.3/thug/.DS_Store`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/ActiveX.py` & `thug-5.3/thug/ActiveX/ActiveX.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/CLSID.py` & `thug-5.3/thug/ActiveX/CLSID.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/AcroPDF.py` & `thug-5.3/thug/ActiveX/modules/AcroPDF.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/AdodbRecordset.py` & `thug-5.3/thug/ActiveX/modules/AdodbRecordset.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/AdodbStream.py` & `thug-5.3/thug/ActiveX/modules/AdodbStream.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/AnswerWorks.py` & `thug-5.3/thug/ActiveX/modules/AnswerWorks.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/AolAmpX.py` & `thug-5.3/thug/ActiveX/modules/AolAmpX.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/AolICQ.py` & `thug-5.3/thug/ActiveX/modules/AolICQ.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/BaiduBar.py` & `thug-5.3/thug/ActiveX/modules/BaiduBar.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/BitDefender.py` & `thug-5.3/thug/ActiveX/modules/BitDefender.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/CGAgent.py` & `thug-5.3/thug/ActiveX/modules/CGAgent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/Comodo.py` & `thug-5.3/thug/ActiveX/modules/Comodo.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/ConnectAndEnterRoom.py` & `thug-5.3/thug/ActiveX/modules/ConnectAndEnterRoom.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/DPClient.py` & `thug-5.3/thug/ActiveX/modules/DPClient.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/DirectShow.py` & `thug-5.3/thug/ActiveX/modules/DirectShow.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/Domino.py` & `thug-5.3/thug/ActiveX/modules/Domino.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/EnjoySAP.py` & `thug-5.3/thug/ActiveX/modules/EnjoySAP.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/FacebookPhotoUploader.py` & `thug-5.3/thug/ActiveX/modules/FacebookPhotoUploader.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/File.py` & `thug-5.3/thug/ActiveX/modules/File.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/Folder.py` & `thug-5.3/thug/ActiveX/modules/Folder.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/GatewayWeblaunch.py` & `thug-5.3/thug/ActiveX/modules/GatewayWeblaunch.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/GomWeb.py` & `thug-5.3/thug/ActiveX/modules/GomWeb.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/HPInfo.py` & `thug-5.3/thug/ActiveX/modules/HPInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/IMWebControl.py` & `thug-5.3/thug/ActiveX/modules/IMWebControl.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/InternetCleverSuite.py` & `thug-5.3/thug/ActiveX/modules/InternetCleverSuite.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/JavaDeploymentToolkit.py` & `thug-5.3/thug/ActiveX/modules/JavaDeploymentToolkit.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py` & `thug-5.3/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/MSRICHTXT.py` & `thug-5.3/thug/ActiveX/modules/MSRICHTXT.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/MSVFP.py` & `thug-5.3/thug/ActiveX/modules/MSVFP.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/MSXML2DOMDocument.py` & `thug-5.3/thug/ActiveX/modules/MSXML2DOMDocument.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/MacrovisionFlexNet.py` & `thug-5.3/thug/ActiveX/modules/MacrovisionFlexNet.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/MicrosoftXMLDOM.py` & `thug-5.3/thug/ActiveX/modules/MicrosoftXMLDOM.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/MicrosoftXMLHTTP.py` & `thug-5.3/thug/ActiveX/modules/MicrosoftXMLHTTP.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/NCTAudioFile2.py` & `thug-5.3/thug/ActiveX/modules/NCTAudioFile2.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/NamoInstaller.py` & `thug-5.3/thug/ActiveX/modules/NamoInstaller.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/NeoTracePro.py` & `thug-5.3/thug/ActiveX/modules/NeoTracePro.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/NessusScanCtrl.py` & `thug-5.3/thug/ActiveX/modules/NessusScanCtrl.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/OfficeOCX.py` & `thug-5.3/thug/ActiveX/modules/OfficeOCX.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/OurgameGLWorld.py` & `thug-5.3/thug/ActiveX/modules/OurgameGLWorld.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/PPlayer.py` & `thug-5.3/thug/ActiveX/modules/PPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/RDSDataSpace.py` & `thug-5.3/thug/ActiveX/modules/RDSDataSpace.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/RealPlayer.py` & `thug-5.3/thug/ActiveX/modules/RealPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/RegistryPro.py` & `thug-5.3/thug/ActiveX/modules/RegistryPro.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/SSReaderPdg2.py` & `thug-5.3/thug/ActiveX/modules/SSReaderPdg2.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/ScriptingDictionary.py` & `thug-5.3/thug/ActiveX/modules/ScriptingDictionary.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/ScriptingFileSystemObject.py` & `thug-5.3/thug/ActiveX/modules/ScriptingFileSystemObject.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/ShellApplication.py` & `thug-5.3/thug/ActiveX/modules/ShellApplication.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/SinaDLoader.py` & `thug-5.3/thug/ActiveX/modules/SinaDLoader.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/SnapshotViewer.py` & `thug-5.3/thug/ActiveX/modules/SnapshotViewer.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py` & `thug-5.3/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/Spreadsheet.py` & `thug-5.3/thug/ActiveX/modules/Spreadsheet.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/StormConfig.py` & `thug-5.3/thug/ActiveX/modules/StormConfig.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/StormMps.py` & `thug-5.3/thug/ActiveX/modules/StormMps.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/StreamAudioChainCast.py` & `thug-5.3/thug/ActiveX/modules/StreamAudioChainCast.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/SymantecAppStream.py` & `thug-5.3/thug/ActiveX/modules/SymantecAppStream.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/SymantecBackupExec.py` & `thug-5.3/thug/ActiveX/modules/SymantecBackupExec.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/TextStream.py` & `thug-5.3/thug/ActiveX/modules/TextStream.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/Toshiba.py` & `thug-5.3/thug/ActiveX/modules/Toshiba.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/UniversalUpload.py` & `thug-5.3/thug/ActiveX/modules/UniversalUpload.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/VLC.py` & `thug-5.3/thug/ActiveX/modules/VLC.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/VisualStudioDTE80.py` & `thug-5.3/thug/ActiveX/modules/VisualStudioDTE80.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/VsaIDEDTE.py` & `thug-5.3/thug/ActiveX/modules/VsaIDEDTE.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/VsmIDEDTE.py` & `thug-5.3/thug/ActiveX/modules/VsmIDEDTE.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WMEncProfileManager.py` & `thug-5.3/thug/ActiveX/modules/WMEncProfileManager.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WScriptExec.py` & `thug-5.3/thug/ActiveX/modules/WScriptExec.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WScriptNetwork.py` & `thug-5.3/thug/ActiveX/modules/WScriptNetwork.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WScriptShell.py` & `thug-5.3/thug/ActiveX/modules/WScriptShell.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WebViewFolderIcon.py` & `thug-5.3/thug/ActiveX/modules/WebViewFolderIcon.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WinNTSystemInfo.py` & `thug-5.3/thug/ActiveX/modules/WinNTSystemInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/WinZip.py` & `thug-5.3/thug/ActiveX/modules/WinZip.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/XMLDOMParseError.py` & `thug-5.3/thug/ActiveX/modules/XMLDOMParseError.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/XUpload.py` & `thug-5.3/thug/ActiveX/modules/XUpload.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/YahooJukebox.py` & `thug-5.3/thug/ActiveX/modules/YahooJukebox.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/YahooMessengerCyft.py` & `thug-5.3/thug/ActiveX/modules/YahooMessengerCyft.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/YahooMessengerYVerInfo.py` & `thug-5.3/thug/ActiveX/modules/YahooMessengerYVerInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/YahooMessengerYwcvwr.py` & `thug-5.3/thug/ActiveX/modules/YahooMessengerYwcvwr.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py` & `thug-5.3/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ActiveX/modules/__init__.py` & `thug-5.3/thug/ActiveX/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Analysis/awis/AWIS.py` & `thug-5.3/thug/Analysis/awis/AWIS.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Analysis/context/ContextAnalyzer.py` & `thug-5.3/thug/Analysis/context/ContextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Analysis/honeyagent/HoneyAgent.py` & `thug-5.3/thug/Analysis/honeyagent/HoneyAgent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Analysis/screenshot/Screenshot.py` & `thug-5.3/thug/Analysis/screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Analysis/shellcode/Shellcode.py` & `thug-5.3/thug/Analysis/shellcode/Shellcode.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/BaseClassifier.py` & `thug-5.3/thug/Classifier/BaseClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/CookieClassifier.py` & `thug-5.3/thug/Classifier/CookieClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/HTMLClassifier.py` & `thug-5.3/thug/Classifier/HTMLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/ImageClassifier.py` & `thug-5.3/thug/Classifier/ImageClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/JSClassifier.py` & `thug-5.3/thug/Classifier/JSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/SampleClassifier.py` & `thug-5.3/thug/Classifier/SampleClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/TextClassifier.py` & `thug-5.3/thug/Classifier/TextClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Classifier/URLClassifier.py` & `thug-5.3/thug/Classifier/URLClassifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     default_filter_file = "rules/urlfilter.yar"
     _classifier         = "URL Classifier"
 
     def __init__(self):
         BaseClassifier.__init__(self)
 
     def classify(self, url):
-        if url.lower().startswith("data:"):
+        if log.HTTPSession.is_data_uri(url):
             return
 
         for match in self.rules.match(data = url):
             self.matches.append((url, match))
 
             if self.discard_url_match(url, match):
                 continue
```

### Comparing `thug-5.2/thug/Classifier/VBSClassifier.py` & `thug-5.3/thug/Classifier/VBSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Alexa.py` & `thug-5.3/thug/DOM/Alexa.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/AsyncPrefetcher.py` & `thug-5.3/thug/DOM/AsyncPrefetcher.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/CCInterpreter.py` & `thug-5.3/thug/DOM/CCInterpreter.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Chrome.py` & `thug-5.3/thug/DOM/Chrome.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/ClipboardData.py` & `thug-5.3/thug/DOM/ClipboardData.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Components.py` & `thug-5.3/thug/DOM/Components.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Console.py` & `thug-5.3/thug/DOM/Console.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Crypto.py` & `thug-5.3/thug/DOM/Crypto.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/DFT.py` & `thug-5.3/thug/DOM/DFT.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
             try:
                 self.window._navigator.fetch(codebase,
                                              redirect_type = "object codebase",
                                              params = params)
             except Exception as e: # pragma: no cover,pylint:disable=broad-except
                 log.info("[ERROR][handle_object] %s", str(e))
 
-        if data and not data.startswith('data:'):
+        if data and not log.HTTPSession.is_data_uri(data):
             if log.ThugOpts.features_logging:
                 log.ThugLogging.Features.increase_url_count()
 
             try:
                 self.window._navigator.fetch(data,
                                              redirect_type = "object data",
                                              params = params)
@@ -717,15 +717,15 @@
         src = script.get('src', None)
         if src is None:
             return
 
         if log.ThugOpts.features_logging:
             log.ThugLogging.Features.increase_url_count()
 
-        if src.lower().startswith("data:"):
+        if log.HTTPSession.is_data_uri(src):
             self.handle_data_javascript(script, src)
             return
 
         try:
             response = self.window._navigator.fetch(src, redirect_type = "script src")
         except Exception as e: # pylint:disable=broad-except
             log.info("[ERROR][handle_external_javascript] %s", str(e))
@@ -1232,15 +1232,15 @@
 
         Some browsers (Chrome, Opera, Safari, Firefox) accept a non-standard
         ordering if both ;base64 and ;charset are supplied, while Internet
         Explorer requires that the charset's specification must precede the
         base64 token.
         """
         uri = uri if isinstance(uri, str) else str(uri)
-        if not uri.lower().startswith("data:"):
+        if not log.HTTPSession.is_data_uri(uri):
             return None
 
         if log.ThugOpts.features_logging:
             log.ThugLogging.Features.increase_data_uri_count()
 
         h = uri.split(",")
         if len(h) < 2 or not h[1]:
```

### Comparing `thug-5.2/thug/DOM/External.py` & `thug-5.3/thug/DOM/External.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/HTMLInspector.py` & `thug-5.3/thug/DOM/HTMLInspector.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/HTTPSession.py` & `thug-5.3/thug/DOM/HTTPSession.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,19 +126,29 @@
 
     def is_download_prevented(self, mimetype = None):
         if mimetype and mimetype.startswith(self.download_prevented_mimetypes):
             return True
 
         return False
 
+    @staticmethod
+    def is_data_uri(url):
+        if url.lower().startswith("data:"):
+            return True
+
+        if url.startswith(("'", '"')) and url[1:].lower().startswith("data:"):
+            return True # pragma: no cover
+
+        return False
+
     def normalize_url(self, window, url):
         url = url.strip()
 
         # Do not normalize Data URI scheme
-        if url.lower().startswith('url=') or url.lower().startswith('data:'):
+        if url.lower().startswith('url=') or self.is_data_uri(url):
             return url
 
         if url.startswith('#'):
             log.warning("[INFO] Ignoring anchor: %s", url)
             return None
 
         # Check the URL is not broken (i.e. http:/www.google.com) and
@@ -230,15 +240,15 @@
         except Exception as e: # pragma: no cover,pylint:disable=broad-except
             log.warning("[SSL ERROR] %s", str(e))
 
     def fetch(self, url, method = "GET", window = None, personality = None, headers = None, body = None):
         if log.URLClassifier.filter(url):
             return None
 
-        if url.startswith("data:"):
+        if self.is_data_uri(url):
             log.DFT._handle_data_uri(url)
             return None
 
         fetcher = getattr(self.session, method.lower(), None)
         if fetcher is None: # pragma: no cover
             log.warning("Not supported method: %s", method)
             return None
```

### Comparing `thug-5.2/thug/DOM/HTTPSessionException.py` & `thug-5.3/thug/DOM/HTTPSessionException.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/History.py` & `thug-5.3/thug/DOM/History.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/JSClass.py` & `thug-5.3/thug/DOM/JSClass.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/JSEngine.py` & `thug-5.3/thug/DOM/JSEngine.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/JSInspector.py` & `thug-5.3/thug/DOM/JSInspector.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/JScriptEncode.py` & `thug-5.3/thug/DOM/JScriptEncode.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/LocalStorage.py` & `thug-5.3/thug/DOM/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Location.py` & `thug-5.3/thug/DOM/Location.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def parts(self):
         return urlparse(self._window.url)
 
     def get_href(self):
         return self._window.url
 
     def set_href(self, url):
-        if url.startswith("data:"): # pragma: no cover
+        if log.HTTPSession.is_data_uri(url): # pragma: no cover
             log.DFT._handle_data_uri(url)
             return
 
         referer = self._window.url
         if log.HTTPSession.check_equal_urls(url, referer):
             log.warning("Skipping location redirection from %s to %s", referer, url)
             return
```

### Comparing `thug-5.2/thug/DOM/MIMEHandler.py` & `thug-5.3/thug/DOM/MIMEHandler.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Map.py` & `thug-5.3/thug/DOM/Map.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/MimeType.py` & `thug-5.3/thug/DOM/MimeType.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/MimeTypes.py` & `thug-5.3/thug/DOM/MimeTypes.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/MozConnection.py` & `thug-5.3/thug/DOM/MozConnection.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Navigator.py` & `thug-5.3/thug/DOM/Navigator.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Personality.py` & `thug-5.3/thug/DOM/Personality.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Plugin.py` & `thug-5.3/thug/DOM/Plugin.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Plugins.py` & `thug-5.3/thug/DOM/Plugins.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/SchemeHandler.py` & `thug-5.3/thug/DOM/SchemeHandler.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Screen.py` & `thug-5.3/thug/DOM/Screen.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/SessionStorage.py` & `thug-5.3/thug/DOM/SessionStorage.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Sidebar.py` & `thug-5.3/thug/DOM/Sidebar.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Storage.py` & `thug-5.3/thug/DOM/Storage.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/UserProfile.py` & `thug-5.3/thug/DOM/UserProfile.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Utils.py` & `thug-5.3/thug/DOM/Utils.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/Attr.py` & `thug-5.3/thug/DOM/W3C/Core/Attr.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/CharacterData.py` & `thug-5.3/thug/DOM/W3C/Core/CharacterData.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/ClassList.py` & `thug-5.3/thug/DOM/W3C/Core/ClassList.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/Comment.py` & `thug-5.3/thug/DOM/W3C/Core/Comment.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/DOMException.py` & `thug-5.3/thug/DOM/W3C/Core/DOMException.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/DOMImplementation.py` & `thug-5.3/thug/DOM/W3C/Core/DOMImplementation.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/Document.py` & `thug-5.3/thug/DOM/W3C/Core/Document.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/DocumentFragment.py` & `thug-5.3/thug/DOM/W3C/Core/DocumentFragment.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/DocumentType.py` & `thug-5.3/thug/DOM/W3C/Core/DocumentType.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/Element.py` & `thug-5.3/thug/DOM/W3C/Core/Element.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/NamedNodeMap.py` & `thug-5.3/thug/DOM/W3C/Core/NamedNodeMap.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/Node.py` & `thug-5.3/thug/DOM/W3C/Core/Node.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/NodeList.py` & `thug-5.3/thug/DOM/W3C/Core/NodeList.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/Text.py` & `thug-5.3/thug/DOM/W3C/Core/Text.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Core/__init__.py` & `thug-5.3/thug/DOM/W3C/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/DOMTokenList.py` & `thug-5.3/thug/DOM/W3C/DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/DocumentEvent.py` & `thug-5.3/thug/DOM/W3C/Events/DocumentEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/Event.py` & `thug-5.3/thug/DOM/W3C/Events/Event.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/EventException.py` & `thug-5.3/thug/DOM/W3C/Events/EventException.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/EventTarget.py` & `thug-5.3/thug/DOM/W3C/Events/EventTarget.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/MessageEvent.py` & `thug-5.3/thug/DOM/W3C/Events/MessageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/MouseEvent.py` & `thug-5.3/thug/DOM/W3C/Events/MouseEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/MutationEvent.py` & `thug-5.3/thug/DOM/W3C/Events/MutationEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/StorageEvent.py` & `thug-5.3/thug/DOM/W3C/Events/StorageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/UIEvent.py` & `thug-5.3/thug/DOM/W3C/Events/UIEvent.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Events/__init__.py` & `thug-5.3/thug/DOM/W3C/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/File/Blob.py` & `thug-5.3/thug/DOM/W3C/File/Blob.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/File/File.py` & `thug-5.3/thug/DOM/W3C/File/File.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/Dataset.py` & `thug-5.3/thug/DOM/W3C/HTML/Dataset.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLAnchorElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLAnchorElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLAppletElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLAppletElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLBodyElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLBodyElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLButtonElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLButtonElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLCollection.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLCollection.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLDocument.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLFormElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLFormElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLFrameElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLIFrameElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLIFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLImageElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLImageElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLInputElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLInputElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLLinkElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLLinkElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLMediaElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLMediaElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLMetaElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLMetaElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLObjectElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLObjectElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLOptionElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLOptionElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLScriptElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLScriptElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLSelectElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLSelectElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLTableCellElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLTableCellElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLTableElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLTableElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLTableRowElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLTableRowElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLTableSectionElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLTableSectionElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/HTMLTextAreaElement.py` & `thug-5.3/thug/DOM/W3C/HTML/HTMLTextAreaElement.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/TAnimateColor.py` & `thug-5.3/thug/DOM/W3C/HTML/TAnimateColor.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/TimeRanges.py` & `thug-5.3/thug/DOM/W3C/HTML/TimeRanges.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/__init__.py` & `thug-5.3/thug/DOM/W3C/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/HTML/text_property.py` & `thug-5.3/thug/DOM/W3C/HTML/text_property.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py` & `thug-5.3/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/URL/URL.py` & `thug-5.3/thug/DOM/W3C/URL/URL.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/W3C/URL/URLSearchParams.py` & `thug-5.3/thug/DOM/W3C/URL/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/WebStore.py` & `thug-5.3/thug/DOM/WebStore.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/Window.py` & `thug-5.3/thug/DOM/Window.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/DOM/w3c_bindings.py` & `thug-5.3/thug/DOM/w3c_bindings.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Encoding/Encoding.py` & `thug-5.3/thug/Encoding/Encoding.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Java/System.py` & `thug-5.3/thug/Java/System.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Java/java.py` & `thug-5.3/thug/Java/java.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Java/lang.py` & `thug-5.3/thug/Java/lang.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/BaseLogging.py` & `thug-5.3/thug/Logging/BaseLogging.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/Features.py` & `thug-5.3/thug/Logging/Features.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/LoggingModules.py` & `thug-5.3/thug/Logging/LoggingModules.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/SampleLogging.py` & `thug-5.3/thug/Logging/SampleLogging.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/ThugLogging.py` & `thug-5.3/thug/Logging/ThugLogging.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/modules/ElasticSearch.py` & `thug-5.3/thug/Logging/modules/ElasticSearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,20 @@
 
         return True
 
     def __init_elasticsearch(self):
         if not self.__init_config():
             return False
 
-        self.es = elasticsearch.Elasticsearch(self.opts['url'], connection_class = elasticsearch.RequestsHttpConnection)
+        if elasticsearch._major < 8:
+            self.es = elasticsearch.Elasticsearch(self.opts['url'],
+                                                  connection_class = elasticsearch.RequestsHttpConnection) # pragma: no cover
+        else:
+            self.es = elasticsearch.Elasticsearch(self.opts['url'])
+
         if not self.es.ping():
             log.warning("[WARNING] ElasticSearch instance not properly initialized")
             return False
 
         self.es.indices.create(index = self.opts['index'], ignore = 400)  # pylint:disable=unexpected-keyword-arg
         return True
```

### Comparing `thug-5.2/thug/Logging/modules/ExploitGraph.py` & `thug-5.3/thug/Logging/modules/ExploitGraph.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/modules/JSON.py` & `thug-5.3/thug/Logging/modules/JSON.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/modules/Mapper.py` & `thug-5.3/thug/Logging/modules/Mapper.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Logging/modules/MongoDB.py` & `thug-5.3/thug/Logging/modules/MongoDB.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Magic/Magic.py` & `thug-5.3/thug/Magic/Magic.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/OS/Windows.py` & `thug-5.3/thug/OS/Windows.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Plugins/IPlugin.py` & `thug-5.3/thug/Plugins/IPlugin.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Plugins/ThugPlugins.py` & `thug-5.3/thug/Plugins/ThugPlugins.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py` & `thug-5.3/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py` & `thug-5.3/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ThugAPI/IThugAPI.py` & `thug-5.3/thug/ThugAPI/IThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ThugAPI/OpaqueFilter.py` & `thug-5.3/thug/ThugAPI/OpaqueFilter.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ThugAPI/ThugAPI.py` & `thug-5.3/thug/ThugAPI/ThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ThugAPI/ThugOpts.py` & `thug-5.3/thug/ThugAPI/ThugOpts.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ThugAPI/ThugVulnModules.py` & `thug-5.3/thug/ThugAPI/ThugVulnModules.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/ThugAPI/Watchdog.py` & `thug-5.3/thug/ThugAPI/Watchdog.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/WebTracking/Cookies.py` & `thug-5.3/thug/WebTracking/Cookies.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/WebTracking/WebStorage.py` & `thug-5.3/thug/WebTracking/WebStorage.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/WebTracking/WebTracking.py` & `thug-5.3/thug/WebTracking/WebTracking.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/__init__.py` & `thug-5.3/thug/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import appdirs
 
-__version__            = "5.2"
+__version__            = "5.3"
 __jsengine__           = ""
 __jsengine_version__   = ""
 
 __global_configuration_path__ = "/etc/thug"
 if os.path.exists(__global_configuration_path__):
     __configuration_path__ = __global_configuration_path__
 else:
```

### Comparing `thug-5.2/thug/conf/.DS_Store` & `thug-5.3/thug/conf/.DS_Store`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/galaxy2chrome18.json` & `thug-5.3/thug/conf/personalities/galaxy2chrome18.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/galaxy2chrome25.json` & `thug-5.3/thug/conf/personalities/galaxy2chrome25.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/galaxy2chrome29.json` & `thug-5.3/thug/conf/personalities/galaxy2chrome29.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome33.json` & `thug-5.3/thug/conf/personalities/ipadchrome33.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome35.json` & `thug-5.3/thug/conf/personalities/ipadchrome35.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome37.json` & `thug-5.3/thug/conf/personalities/ipadchrome37.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome38.json` & `thug-5.3/thug/conf/personalities/ipadchrome38.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome39.json` & `thug-5.3/thug/conf/personalities/ipadchrome39.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome45.json` & `thug-5.3/thug/conf/personalities/ipadchrome45.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome46.json` & `thug-5.3/thug/conf/personalities/ipadchrome46.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadchrome47.json` & `thug-5.3/thug/conf/personalities/ipadchrome47.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadsafari7.json` & `thug-5.3/thug/conf/personalities/ipadsafari7.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadsafari8.json` & `thug-5.3/thug/conf/personalities/ipadsafari8.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/ipadsafari9.json` & `thug-5.3/thug/conf/personalities/ipadsafari9.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxchrome26.json` & `thug-5.3/thug/conf/personalities/linuxchrome26.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxchrome30.json` & `thug-5.3/thug/conf/personalities/linuxchrome30.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxchrome44.json` & `thug-5.3/thug/conf/personalities/linuxchrome44.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxchrome54.json` & `thug-5.3/thug/conf/personalities/linuxchrome54.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxchrome98.json` & `thug-5.3/thug/conf/personalities/linuxchrome98.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxfirefox19.json` & `thug-5.3/thug/conf/personalities/linuxfirefox19.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/linuxfirefox40.json` & `thug-5.3/thug/conf/personalities/linuxfirefox40.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/nexuschrome18.json` & `thug-5.3/thug/conf/personalities/nexuschrome18.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/osx10chrome19.json` & `thug-5.3/thug/conf/personalities/osx10chrome19.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/osx10chrome80.json` & `thug-5.3/thug/conf/personalities/osx10chrome80.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/osx10chrome97.json` & `thug-5.3/thug/conf/personalities/osx10chrome97.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/osx10safari5.json` & `thug-5.3/thug/conf/personalities/osx10safari5.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/osx11safari14.json` & `thug-5.3/thug/conf/personalities/osx11safari14.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win10edge20.json.review` & `thug-5.3/thug/conf/personalities/win10edge20.json.review`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win10ie110.json` & `thug-5.3/thug/conf/personalities/win10ie110.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win2kie60.json` & `thug-5.3/thug/conf/personalities/win2kie60.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win2kie80.json` & `thug-5.3/thug/conf/personalities/win2kie80.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7chrome20.json` & `thug-5.3/thug/conf/personalities/win7chrome20.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7chrome40.json` & `thug-5.3/thug/conf/personalities/win7chrome40.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7chrome45.json` & `thug-5.3/thug/conf/personalities/win7chrome45.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7chrome49.json` & `thug-5.3/thug/conf/personalities/win7chrome49.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7firefox3.json` & `thug-5.3/thug/conf/personalities/win7firefox3.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7ie100.json` & `thug-5.3/thug/conf/personalities/win7ie100.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7ie80.json` & `thug-5.3/thug/conf/personalities/win7ie80.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7ie90.json` & `thug-5.3/thug/conf/personalities/win7ie90.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/win7safari5.json` & `thug-5.3/thug/conf/personalities/win7safari5.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpchrome20.json` & `thug-5.3/thug/conf/personalities/winxpchrome20.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpfirefox12.json` & `thug-5.3/thug/conf/personalities/winxpfirefox12.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpie60.json` & `thug-5.3/thug/conf/personalities/winxpie60.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpie61.json` & `thug-5.3/thug/conf/personalities/winxpie61.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpie70.json` & `thug-5.3/thug/conf/personalities/winxpie70.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpie80.json` & `thug-5.3/thug/conf/personalities/winxpie80.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/personalities/winxpsafari5.json` & `thug-5.3/thug/conf/personalities/winxpsafari5.json`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/blackhole.yar` & `thug-5.3/thug/conf/rules/urlclassifier/blackhole.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/crimeboss.yar` & `thug-5.3/thug/conf/rules/urlclassifier/crimeboss.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/critxpack.yar` & `thug-5.3/thug/conf/rules/urlclassifier/critxpack.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/fiesta.yar` & `thug-5.3/thug/conf/rules/urlclassifier/fiesta.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/g01pack.yar` & `thug-5.3/thug/conf/rules/urlclassifier/g01pack.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/neutrino.yar` & `thug-5.3/thug/conf/rules/urlclassifier/neutrino.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/nuclear.yar` & `thug-5.3/thug/conf/rules/urlclassifier/nuclear.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/popads.yar` & `thug-5.3/thug/conf/rules/urlclassifier/popads.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/redkit.yar` & `thug-5.3/thug/conf/rules/urlclassifier/redkit.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/styx.yar` & `thug-5.3/thug/conf/rules/urlclassifier/styx.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/rules/urlclassifier/sweetorange.yar` & `thug-5.3/thug/conf/rules/urlclassifier/sweetorange.yar`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/conf/scripts/thug.js` & `thug-5.3/thug/conf/scripts/thug.js`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug/thug.py` & `thug-5.3/thug/thug.py`

 * *Files identical despite different names*

### Comparing `thug-5.2/thug.egg-info/PKG-INFO` & `thug-5.3/thug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 5.2
+Version: 5.3
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
```

### Comparing `thug-5.2/thug.egg-info/SOURCES.txt` & `thug-5.3/thug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

