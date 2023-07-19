# Comparing `tmp/airavata_mft_sdk-0.0.1a8.tar.gz` & `tmp/airavata_mft_sdk-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airavata_mft_sdk-0.0.1a8.tar", last modified: Mon Apr 11 03:27:20 2022, max compression
+gzip compressed data, was "airavata_mft_sdk-0.0.1a9.tar", last modified: Mon Apr 11 05:47:25 2022, max compression
```

## Comparing `airavata_mft_sdk-0.0.1a8.tar` & `airavata_mft_sdk-0.0.1a9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    11356 2022-04-10 14:49:45.000000 airavata_mft_sdk-0.0.1a8/LICENSE
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      623 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/PKG-INFO
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      353 2022-04-10 18:16:35.000000 airavata_mft_sdk-0.0.1a8/README.md
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      126 2022-04-10 14:49:45.000000 airavata_mft_sdk-0.0.1a8/pyproject.toml
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      792 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/setup.cfg
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.036198 airavata_mft_sdk-0.0.1a8/src/
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.036198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     4675 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/CredCommon_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/CredCommon_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    15403 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/MFTTransferApi_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    14876 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/MFTTransferApi_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:58.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.036198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5725 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureCredential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureCredential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1927 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureSecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     8199 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureSecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2183 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9910 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6875 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.036198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5533 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxCredential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxCredential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1873 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxSecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxSecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2092 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9599 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6508 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.036198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5928 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxCredential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxCredential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1991 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     8451 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2262 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    10219 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7012 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5603 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPCredential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPCredential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1873 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPSecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPSecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2092 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9639 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6718 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5504 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSCredential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSCredential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1864 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSSecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSSecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2083 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9639 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6595 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2174 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9909 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6854 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/__init__.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     3254 2022-04-11 03:26:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/mft_client.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resource/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    11157 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resource/ResourceService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     8510 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resource/ResourceService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resource/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resourcesecretmap/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9648 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    10622 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resourcesecretmap/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5488 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3Credential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3Credential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1824 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3SecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7821 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3SecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2044 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3StorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9444 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3StorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6822 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3Storage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3Storage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.040198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5808 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPCredential_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPCredential_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1864 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPSecretService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPSecretService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2083 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorageService_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9639 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorageService_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6725 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorage_pb2.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorage_pb2_grpc.py
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/__init__.py
-drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 03:27:20.036198 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      623 2022-04-11 03:27:19.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     4205 2022-04-11 03:27:20.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        1 2022-04-11 03:27:19.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)       74 2022-04-11 03:27:19.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/requires.txt
--rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)       17 2022-04-11 03:27:19.000000 airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    11356 2022-04-10 14:49:45.000000 airavata_mft_sdk-0.0.1a9/LICENSE
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      623 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/PKG-INFO
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      353 2022-04-10 18:16:35.000000 airavata_mft_sdk-0.0.1a9/README.md
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      126 2022-04-10 14:49:45.000000 airavata_mft_sdk-0.0.1a9/pyproject.toml
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      792 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/setup.cfg
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     4675 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/CredCommon_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/CredCommon_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    15403 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/MFTTransferApi_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    14876 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/MFTTransferApi_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:58.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5725 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureCredential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureCredential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1927 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureSecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     8199 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureSecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2183 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9910 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6875 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5533 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxCredential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxCredential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1873 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxSecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxSecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2092 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9599 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6508 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5928 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxCredential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxCredential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1991 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     8451 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2262 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    10219 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7012 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5603 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPCredential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPCredential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1873 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPSecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPSecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2092 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9639 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6718 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5504 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSCredential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSCredential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1864 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSSecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSSecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2083 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9639 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6595 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2174 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9909 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6854 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/__init__.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     4022 2022-04-11 05:46:56.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/mft_client.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resource/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    11157 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resource/ResourceService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     8510 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resource/ResourceService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resource/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resourcesecretmap/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9648 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)    10622 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resourcesecretmap/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5488 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3Credential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3Credential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1824 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3SecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7821 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3SecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2044 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3StorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9444 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3StorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6822 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3Storage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3Storage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.047936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     5808 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPCredential_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPCredential_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     1864 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPSecretService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     7947 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPSecretService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     2083 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorageService_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     9639 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorageService_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     6725 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorage_pb2.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      159 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorage_pb2_grpc.py
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 02:42:59.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/__init__.py
+drwxrwxr-x   0 dimuthu   (1000) dimuthu   (1000)        0 2022-04-11 05:47:25.043936 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)      623 2022-04-11 05:47:24.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)     4205 2022-04-11 05:47:25.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)        1 2022-04-11 05:47:24.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)       74 2022-04-11 05:47:24.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/requires.txt
+-rw-rw-r--   0 dimuthu   (1000) dimuthu   (1000)       17 2022-04-11 05:47:24.000000 airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/top_level.txt
```

### Comparing `airavata_mft_sdk-0.0.1a8/LICENSE` & `airavata_mft_sdk-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/PKG-INFO` & `airavata_mft_sdk-0.0.1a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata_mft_sdk
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Python SDK for Apache Airavata Managed File Transfers (MFT)
 Home-page: https://github.com/apache/airavata-mft
 Author: Airavata MFT Developers
 Author-email: dev@airavata.apache.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/apache/airavata-mft/issues
 Platform: UNKNOWN
```

### Comparing `airavata_mft_sdk-0.0.1a8/setup.cfg` & `airavata_mft_sdk-0.0.1a9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airavata_mft_sdk
-version = 0.0.1-alpha8
+version = 0.0.1-alpha9
 author = Airavata MFT Developers
 author_email = dev@airavata.apache.org
 description = Python SDK for Apache Airavata Managed File Transfers (MFT)
 long_description = Python SDK for Apache Airavata Managed File Transfers (MFT)
 url = https://github.com/apache/airavata-mft
 project_urls = 
 	Bug Tracker = https://github.com/apache/airavata-mft/issues
```

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/CredCommon_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/CredCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/MFTTransferApi_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/MFTTransferApi_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/MFTTransferApi_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/MFTTransferApi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureCredential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureCredential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureSecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureSecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureSecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureSecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/azure/AzureStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/azure/AzureStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxCredential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxCredential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxSecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxSecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxSecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxSecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/box/BoxStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/box/BoxStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxCredential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxCredential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxSecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/dropbox/DropboxStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/dropbox/DropboxStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPCredential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPCredential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPSecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPSecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPSecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPSecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/ftp/FTPStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/ftp/FTPStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSCredential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSCredential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSSecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSSecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSSecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSSecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/gcs/GCSStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/gcs/GCSStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/local/LocalStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/local/LocalStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resource/ResourceService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resource/ResourceService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resource/ResourceService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resource/ResourceService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/resourcesecretmap/StorageSecretMap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3Credential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3Credential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3SecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3SecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3SecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3SecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3StorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3StorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3StorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3StorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/s3/S3Storage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/s3/S3Storage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPCredential_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPCredential_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPSecretService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPSecretService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPSecretService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPSecretService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorageService_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorageService_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorageService_pb2_grpc.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorageService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk/scp/SCPStorage_pb2.py` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk/scp/SCPStorage_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/PKG-INFO` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-mft-sdk
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Python SDK for Apache Airavata Managed File Transfers (MFT)
 Home-page: https://github.com/apache/airavata-mft
 Author: Airavata MFT Developers
 Author-email: dev@airavata.apache.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/apache/airavata-mft/issues
 Platform: UNKNOWN
```

### Comparing `airavata_mft_sdk-0.0.1a8/src/airavata_mft_sdk.egg-info/SOURCES.txt` & `airavata_mft_sdk-0.0.1a9/src/airavata_mft_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

