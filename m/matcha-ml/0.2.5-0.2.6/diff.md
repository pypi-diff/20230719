# Comparing `tmp/matcha_ml-0.2.5.tar.gz` & `tmp/matcha_ml-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matcha_ml-0.2.5.tar", max compression
+gzip compressed data, was "matcha_ml-0.2.6.tar", max compression
```

## Comparing `matcha_ml-0.2.5.tar` & `matcha_ml-0.2.6.tar`

### file list

```diff
@@ -1,117 +1,118 @@
--rw-r--r--   0        0        0    11357 2023-05-31 07:24:38.008574 matcha_ml-0.2.5/LICENSE
--rw-r--r--   0        0        0     4289 2023-05-19 10:23:10.003833 matcha_ml-0.2.5/README.md
--rw-r--r--   0        0        0     3706 2023-06-06 14:47:51.925733 matcha_ml-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        6 2023-06-06 14:47:51.925990 matcha_ml-0.2.5/src/matcha_ml/VERSION
--rw-r--r--   0        0        0      220 2023-05-16 13:30:52.737917 matcha_ml-0.2.5/src/matcha_ml/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 13:30:52.738233 matcha_ml-0.2.5/src/matcha_ml/cli/__init__.py
--rw-r--r--   0        0        0     7712 2023-06-06 14:40:41.482127 matcha_ml-0.2.5/src/matcha_ml/cli/_validation.py
--rw-r--r--   0        0        0     5473 2023-06-06 14:40:41.482478 matcha_ml-0.2.5/src/matcha_ml/cli/cli.py
--rw-r--r--   0        0        0      769 2023-06-06 14:40:41.483120 matcha_ml-0.2.5/src/matcha_ml/cli/constants.py
--rw-r--r--   0        0        0     2038 2023-06-06 14:40:41.483427 matcha_ml-0.2.5/src/matcha_ml/cli/destroy.py
--rw-r--r--   0        0        0     4668 2023-06-06 14:40:41.483729 matcha_ml-0.2.5/src/matcha_ml/cli/provision.py
--rw-r--r--   0        0        0      278 2023-05-16 13:30:52.739662 matcha_ml-0.2.5/src/matcha_ml/cli/ui/emojis.py
--rw-r--r--   0        0        0     1173 2023-05-16 13:30:52.739975 matcha_ml-0.2.5/src/matcha_ml/cli/ui/print_messages.py
--rw-r--r--   0        0        0     2549 2023-05-16 13:30:52.740225 matcha_ml-0.2.5/src/matcha_ml/cli/ui/resource_message_builders.py
--rw-r--r--   0        0        0     1249 2023-05-16 13:30:52.740423 matcha_ml-0.2.5/src/matcha_ml/cli/ui/spinner.py
--rw-r--r--   0        0        0     1961 2023-06-06 14:40:41.484003 matcha_ml-0.2.5/src/matcha_ml/cli/ui/status_message_builders.py
--rw-r--r--   0        0        0       61 2023-06-06 14:40:41.484582 matcha_ml-0.2.5/src/matcha_ml/constants.py
--rw-r--r--   0        0        0        0 2023-06-06 14:40:41.484744 matcha_ml-0.2.5/src/matcha_ml/core/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-06 14:40:41.485190 matcha_ml-0.2.5/src/matcha_ml/core/core.py
--rw-r--r--   0        0        0     2535 2023-05-16 13:30:52.741158 matcha_ml-0.2.5/src/matcha_ml/errors.py
--rw-r--r--   0        0        0      882 2023-06-06 14:40:41.485449 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.gitignore
--rw-r--r--   0        0        0     1156 2023-06-06 14:40:41.485898 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl
--rw-r--r--   0        0        0      440 2023-06-06 14:40:41.486078 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/main.tf
--rw-r--r--   0        0        0      762 2023-06-06 14:40:41.486477 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/output.tf
--rw-r--r--   0        0        0      110 2023-06-06 14:40:41.486807 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/resource_group/main.tf
--rw-r--r--   0        0        0      106 2023-06-06 14:40:41.486990 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/resource_group/output.tf
--rw-r--r--   0        0        0      235 2023-06-06 14:40:41.487228 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/resource_group/variables.tf
--rw-r--r--   0        0        0      776 2023-06-06 14:40:41.487495 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf
--rw-r--r--   0        0        0     1819 2023-06-06 14:40:41.487697 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf
--rw-r--r--   0        0        0      457 2023-06-06 14:40:41.487864 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/variables.tf
--rw-r--r--   0        0        0      256 2023-06-06 14:40:41.488045 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/variables.tf
--rw-r--r--   0        0        0      882 2023-06-06 14:40:41.488497 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.gitignore
--rw-r--r--   0        0        0     9245 2023-06-06 14:40:41.488748 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl
--rw-r--r--   0        0        0     4696 2023-06-06 14:40:41.488954 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/README.md
--rw-r--r--   0        0        0     2213 2023-06-06 14:40:41.489267 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/README.md
--rw-r--r--   0        0        0      439 2023-06-06 14:40:41.489453 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/main.tf
--rw-r--r--   0        0        0     1437 2023-06-06 14:40:41.489761 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/output.tf
--rw-r--r--   0        0        0      386 2023-06-06 14:40:41.489995 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/variables.tf
--rw-r--r--   0        0        0     1605 2023-06-06 14:40:41.490242 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md
--rw-r--r--   0        0        0      484 2023-06-06 14:40:41.490406 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/main.tf
--rw-r--r--   0        0        0      327 2023-06-06 14:40:41.490543 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/output.tf
--rw-r--r--   0        0        0      462 2023-06-06 14:40:41.490689 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/variables.tf
--rw-r--r--   0        0        0      625 2023-06-06 14:40:41.490863 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/configure_kubectl.tf
--rw-r--r--   0        0        0      337 2023-06-06 14:40:41.491218 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/helm.tf
--rw-r--r--   0        0        0     1107 2023-06-06 14:40:41.491487 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/kubernetes.tf
--rw-r--r--   0        0        0     1886 2023-06-06 14:40:41.491920 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/main.tf
--rw-r--r--   0        0        0     2208 2023-06-06 14:40:41.492315 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/README.md
--rw-r--r--   0        0        0      308 2023-06-06 14:40:41.492557 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/getURI.tf
--rw-r--r--   0        0        0     1314 2023-06-06 14:40:41.492749 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf
--rw-r--r--   0        0        0      251 2023-06-06 14:40:41.493013 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/output.tf
--rw-r--r--   0        0        0      383 2023-06-06 14:40:41.493196 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/providers.tf
--rw-r--r--   0        0        0      803 2023-06-06 14:40:41.493371 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf
--rw-r--r--   0        0        0       81 2023-06-06 14:40:41.493536 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/zenml_namespace.tf
--rw-r--r--   0        0        0     2238 2023-06-06 14:40:41.493726 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/output.tf
--rw-r--r--   0        0        0       33 2023-06-06 14:40:41.493980 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/printf.cmd
--rw-r--r--   0        0        0      782 2023-06-06 14:40:41.494229 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/providers.tf
--rw-r--r--   0        0        0      892 2023-06-06 14:40:41.494515 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/README.md
--rw-r--r--   0        0        0       80 2023-06-06 14:40:41.494699 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/main.tf
--rw-r--r--   0        0        0      111 2023-06-06 14:40:41.494857 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/output.tf
--rw-r--r--   0        0        0       95 2023-06-06 14:40:41.494999 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/variables.tf
--rw-r--r--   0        0        0     3010 2023-06-06 14:40:41.495268 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/README.md
--rw-r--r--   0        0        0     1894 2023-06-06 14:40:41.495454 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/istio.tf
--rw-r--r--   0        0        0     1158 2023-06-06 14:40:41.495616 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/main.tf
--rw-r--r--   0        0        0      663 2023-06-06 14:40:41.495788 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/outputs.tf
--rw-r--r--   0        0        0      925 2023-06-06 14:40:41.495982 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/permissions.tf
--rw-r--r--   0        0        0      380 2023-06-06 14:40:41.496142 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/providers.tf
--rw-r--r--   0        0        0      453 2023-06-06 14:40:41.496307 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/variables.tf
--rw-r--r--   0        0        0     2914 2023-06-06 14:40:41.496622 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/README.md
--rw-r--r--   0        0        0      866 2023-06-06 14:40:41.496785 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/main.tf
--rw-r--r--   0        0        0     1779 2023-06-06 14:40:41.497058 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/output.tf
--rw-r--r--   0        0        0      124 2023-06-06 14:40:41.497317 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/providers.tf
--rw-r--r--   0        0        0      454 2023-06-06 14:40:41.497501 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/variables.tf
--rw-r--r--   0        0        0      754 2023-06-06 14:40:41.497715 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/variables.tf
--rw-r--r--   0        0        0     6080 2023-06-06 14:40:41.497973 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/README.md
--rw-r--r--   0        0        0      216 2023-06-06 14:40:41.498149 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/getURL.tf
--rw-r--r--   0        0        0      979 2023-06-06 14:40:41.498297 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf
--rw-r--r--   0        0        0     3026 2023-06-06 14:40:41.498465 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/main.tf
--rw-r--r--   0        0        0      704 2023-06-06 14:40:41.498642 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf
--rw-r--r--   0        0        0      292 2023-06-06 14:40:41.498805 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/providers.tf
--rw-r--r--   0        0        0     1943 2023-06-06 14:40:41.498971 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/sql.tf
--rw-r--r--   0        0        0     4701 2023-06-06 14:40:41.499130 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/variables.tf
--rw-r--r--   0        0        0      342 2023-06-06 14:40:41.499392 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/Chart.yaml
--rw-r--r--   0        0        0     1987 2023-06-06 14:40:41.499652 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt
--rw-r--r--   0        0        0     2054 2023-06-06 14:40:41.499882 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl
--rw-r--r--   0        0        0     1565 2023-06-06 14:40:41.500086 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml
--rw-r--r--   0        0        0      910 2023-06-06 14:40:41.500241 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml
--rw-r--r--   0        0        0    10774 2023-06-06 14:40:41.500516 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml
--rw-r--r--   0        0        0     2225 2023-06-06 14:40:41.500698 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml
--rw-r--r--   0        0        0     3584 2023-06-06 14:40:41.500854 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml
--rw-r--r--   0        0        0      367 2023-06-06 14:40:41.500996 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-service.yaml
--rw-r--r--   0        0        0      316 2023-06-06 14:40:41.501165 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      379 2023-06-06 14:40:41.501430 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0    11587 2023-06-06 14:40:41.501640 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml
--rw-r--r--   0        0        0     3453 2023-06-06 14:40:41.501870 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/README.md
--rw-r--r--   0        0        0     1102 2023-06-06 14:40:41.502010 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf
--rw-r--r--   0        0        0     1926 2023-06-06 14:40:41.502178 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf
--rw-r--r--   0        0        0      468 2023-06-06 14:40:41.502319 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/variables.tf
--rw-r--r--   0        0        0      170 2023-06-06 14:40:41.502514 matcha_ml-0.2.5/src/matcha_ml/runners/__init__.py
--rw-r--r--   0        0        0     5732 2023-06-06 14:40:41.502828 matcha_ml-0.2.5/src/matcha_ml/runners/azure_runner.py
--rw-r--r--   0        0        0     6611 2023-06-06 14:40:41.503191 matcha_ml-0.2.5/src/matcha_ml/runners/base_runner.py
--rw-r--r--   0        0        0     2825 2023-06-06 14:40:41.503498 matcha_ml-0.2.5/src/matcha_ml/runners/remote_state_runner.py
--rw-r--r--   0        0        0      103 2023-05-16 13:30:52.757540 matcha_ml-0.2.5/src/matcha_ml/services/__init__.py
--rw-r--r--   0        0        0      646 2023-06-06 14:40:41.504545 matcha_ml-0.2.5/src/matcha_ml/services/_validation.py
--rw-r--r--   0        0        0     3409 2023-06-06 14:40:41.505438 matcha_ml-0.2.5/src/matcha_ml/services/analytics_service.py
--rw-r--r--   0        0        0    10848 2023-06-06 14:40:41.505839 matcha_ml-0.2.5/src/matcha_ml/services/azure_service.py
--rw-r--r--   0        0        0     4542 2023-06-06 14:40:41.506364 matcha_ml-0.2.5/src/matcha_ml/services/global_parameters_service.py
--rw-r--r--   0        0        0     5796 2023-06-06 14:40:41.507481 matcha_ml-0.2.5/src/matcha_ml/services/terraform_service.py
--rw-r--r--   0        0        0      185 2023-05-19 10:43:53.173299 matcha_ml-0.2.5/src/matcha_ml/state/__init__.py
--rw-r--r--   0        0        0     3028 2023-06-06 14:40:41.507988 matcha_ml-0.2.5/src/matcha_ml/state/matcha_state.py
--rw-r--r--   0        0        0    11303 2023-06-06 14:40:41.508573 matcha_ml-0.2.5/src/matcha_ml/state/remote_state_manager.py
--rw-r--r--   0        0        0       94 2023-05-19 10:43:53.174430 matcha_ml-0.2.5/src/matcha_ml/storage/__init__.py
--rw-r--r--   0        0        0     9692 2023-06-06 14:40:41.508964 matcha_ml-0.2.5/src/matcha_ml/storage/azure_storage.py
--rw-r--r--   0        0        0      184 2023-06-06 14:40:41.509200 matcha_ml-0.2.5/src/matcha_ml/templates/__init__.py
--rw-r--r--   0        0        0     1952 2023-06-06 14:40:41.509416 matcha_ml-0.2.5/src/matcha_ml/templates/azure_template.py
--rw-r--r--   0        0        0     7255 2023-06-06 14:40:41.509594 matcha_ml-0.2.5/src/matcha_ml/templates/base_template.py
--rw-r--r--   0        0        0      635 2023-06-06 14:40:41.509704 matcha_ml-0.2.5/src/matcha_ml/templates/remote_state_template.py
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 matcha_ml-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-19 13:57:24.538459 matcha_ml-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4289 2023-07-19 13:57:24.538616 matcha_ml-0.2.6/README.md
+-rw-r--r--   0        0        0     3811 2023-07-19 14:29:44.899515 matcha_ml-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-07-19 14:29:44.908241 matcha_ml-0.2.6/src/matcha_ml/VERSION
+-rw-r--r--   0        0        0      220 2023-07-19 13:57:24.567863 matcha_ml-0.2.6/src/matcha_ml/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-19 13:57:24.568088 matcha_ml-0.2.6/src/matcha_ml/cli/__init__.py
+-rw-r--r--   0        0        0     3893 2023-07-19 14:28:18.772178 matcha_ml-0.2.6/src/matcha_ml/cli/_validation.py
+-rw-r--r--   0        0        0     8030 2023-07-19 14:28:18.772524 matcha_ml-0.2.6/src/matcha_ml/cli/cli.py
+-rw-r--r--   0        0        0      769 2023-07-19 13:57:24.568737 matcha_ml-0.2.6/src/matcha_ml/cli/constants.py
+-rw-r--r--   0        0        0     1817 2023-07-19 14:28:18.772911 matcha_ml-0.2.6/src/matcha_ml/cli/destroy.py
+-rw-r--r--   0        0        0      278 2023-07-19 13:57:24.569287 matcha_ml-0.2.6/src/matcha_ml/cli/ui/emojis.py
+-rw-r--r--   0        0        0     1173 2023-07-19 13:57:24.569546 matcha_ml-0.2.6/src/matcha_ml/cli/ui/print_messages.py
+-rw-r--r--   0        0        0     2639 2023-07-19 14:28:18.773546 matcha_ml-0.2.6/src/matcha_ml/cli/ui/resource_message_builders.py
+-rw-r--r--   0        0        0     1249 2023-07-19 14:28:18.773904 matcha_ml-0.2.6/src/matcha_ml/cli/ui/spinner.py
+-rw-r--r--   0        0        0     1957 2023-07-19 14:28:18.774143 matcha_ml-0.2.6/src/matcha_ml/cli/ui/status_message_builders.py
+-rw-r--r--   0        0        0     1063 2023-07-19 14:28:18.774485 matcha_ml-0.2.6/src/matcha_ml/cli/ui/user_approval_functions.py
+-rw-r--r--   0        0        0      150 2023-07-19 14:28:18.774716 matcha_ml-0.2.6/src/matcha_ml/constants.py
+-rw-r--r--   0        0        0      299 2023-07-19 14:28:18.775004 matcha_ml-0.2.6/src/matcha_ml/core/__init__.py
+-rw-r--r--   0        0        0     2755 2023-07-19 14:28:18.775245 matcha_ml-0.2.6/src/matcha_ml/core/_validation.py
+-rw-r--r--   0        0        0     9203 2023-07-19 14:28:18.775480 matcha_ml-0.2.6/src/matcha_ml/core/core.py
+-rw-r--r--   0        0        0     2559 2023-07-19 14:28:18.775936 matcha_ml-0.2.6/src/matcha_ml/errors.py
+-rw-r--r--   0        0        0      882 2023-07-19 13:57:24.572006 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.gitignore
+-rw-r--r--   0        0        0     1156 2023-07-19 13:57:24.572219 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl
+-rw-r--r--   0        0        0      440 2023-07-19 14:28:18.776357 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/main.tf
+-rw-r--r--   0        0        0      762 2023-07-19 13:57:24.572721 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/output.tf
+-rw-r--r--   0        0        0      110 2023-07-19 13:57:24.573124 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/resource_group/main.tf
+-rw-r--r--   0        0        0      106 2023-07-19 13:57:24.573253 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/resource_group/output.tf
+-rw-r--r--   0        0        0      235 2023-07-19 13:57:24.573443 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/resource_group/variables.tf
+-rw-r--r--   0        0        0      776 2023-07-19 13:57:24.573629 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf
+-rw-r--r--   0        0        0     1819 2023-07-19 13:57:24.573797 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf
+-rw-r--r--   0        0        0      457 2023-07-19 13:57:24.573951 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/variables.tf
+-rw-r--r--   0        0        0      256 2023-07-19 13:57:24.574201 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/variables.tf
+-rw-r--r--   0        0        0      882 2023-07-19 13:57:24.574564 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.gitignore
+-rw-r--r--   0        0        0     9245 2023-07-19 13:57:24.574918 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl
+-rw-r--r--   0        0        0     4696 2023-07-19 13:57:24.575155 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/README.md
+-rw-r--r--   0        0        0     2213 2023-07-19 13:57:24.575467 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/README.md
+-rw-r--r--   0        0        0      439 2023-07-19 13:57:24.575822 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/main.tf
+-rw-r--r--   0        0        0     1437 2023-07-19 13:57:24.576087 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/output.tf
+-rw-r--r--   0        0        0      386 2023-07-19 13:57:24.576296 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/variables.tf
+-rw-r--r--   0        0        0     1605 2023-07-19 13:57:24.576606 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md
+-rw-r--r--   0        0        0      484 2023-07-19 13:57:24.576809 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/main.tf
+-rw-r--r--   0        0        0      327 2023-07-19 13:57:24.577295 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/output.tf
+-rw-r--r--   0        0        0      462 2023-07-19 13:57:24.577469 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/variables.tf
+-rw-r--r--   0        0        0      625 2023-07-19 13:57:24.577696 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/configure_kubectl.tf
+-rw-r--r--   0        0        0      337 2023-07-19 13:57:24.577990 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/helm.tf
+-rw-r--r--   0        0        0     1107 2023-07-19 13:57:24.578189 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/kubernetes.tf
+-rw-r--r--   0        0        0     1885 2023-07-19 14:28:18.776812 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/main.tf
+-rw-r--r--   0        0        0     2208 2023-07-19 13:57:24.578733 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/README.md
+-rw-r--r--   0        0        0      308 2023-07-19 13:57:24.578903 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/getURI.tf
+-rw-r--r--   0        0        0     1314 2023-07-19 13:57:24.579123 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf
+-rw-r--r--   0        0        0      251 2023-07-19 13:57:24.579295 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/output.tf
+-rw-r--r--   0        0        0      383 2023-07-19 13:57:24.579479 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/providers.tf
+-rw-r--r--   0        0        0      803 2023-07-19 13:57:24.579662 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf
+-rw-r--r--   0        0        0       81 2023-07-19 13:57:24.579872 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/zenml_namespace.tf
+-rw-r--r--   0        0        0     2458 2023-07-19 14:28:18.777114 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/output.tf
+-rw-r--r--   0        0        0       33 2023-07-19 13:57:24.580447 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/printf.cmd
+-rw-r--r--   0        0        0      782 2023-07-19 13:57:24.580721 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/providers.tf
+-rw-r--r--   0        0        0      892 2023-07-19 13:57:24.581143 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/README.md
+-rw-r--r--   0        0        0       80 2023-07-19 13:57:24.581384 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/main.tf
+-rw-r--r--   0        0        0      111 2023-07-19 13:57:24.581545 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/output.tf
+-rw-r--r--   0        0        0       95 2023-07-19 13:57:24.581725 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/variables.tf
+-rw-r--r--   0        0        0     3010 2023-07-19 13:57:24.582085 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/README.md
+-rw-r--r--   0        0        0     1894 2023-07-19 13:57:24.582500 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/istio.tf
+-rw-r--r--   0        0        0     1158 2023-07-19 13:57:24.582689 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/main.tf
+-rw-r--r--   0        0        0      663 2023-07-19 13:57:24.582873 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/outputs.tf
+-rw-r--r--   0        0        0      925 2023-07-19 13:57:24.583130 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/permissions.tf
+-rw-r--r--   0        0        0      380 2023-07-19 13:57:24.583582 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/providers.tf
+-rw-r--r--   0        0        0      453 2023-07-19 13:57:24.583789 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/variables.tf
+-rw-r--r--   0        0        0     2914 2023-07-19 13:57:24.584086 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/README.md
+-rw-r--r--   0        0        0      866 2023-07-19 13:57:24.584274 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/main.tf
+-rw-r--r--   0        0        0     1779 2023-07-19 13:57:24.584465 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/output.tf
+-rw-r--r--   0        0        0      124 2023-07-19 13:57:24.584675 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/providers.tf
+-rw-r--r--   0        0        0      454 2023-07-19 13:57:24.584870 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/variables.tf
+-rw-r--r--   0        0        0      754 2023-07-19 13:57:24.585157 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/variables.tf
+-rw-r--r--   0        0        0     6080 2023-07-19 13:57:24.585488 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/README.md
+-rw-r--r--   0        0        0      216 2023-07-19 13:57:24.585708 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/getURL.tf
+-rw-r--r--   0        0        0      979 2023-07-19 13:57:24.586089 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf
+-rw-r--r--   0        0        0     3026 2023-07-19 13:57:24.586498 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/main.tf
+-rw-r--r--   0        0        0      704 2023-07-19 13:57:24.586731 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf
+-rw-r--r--   0        0        0      292 2023-07-19 13:57:24.586936 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/providers.tf
+-rw-r--r--   0        0        0     1943 2023-07-19 13:57:24.587532 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/sql.tf
+-rw-r--r--   0        0        0     4701 2023-07-19 13:57:24.587990 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/variables.tf
+-rw-r--r--   0        0        0      342 2023-07-19 13:57:24.588336 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/Chart.yaml
+-rw-r--r--   0        0        0     1987 2023-07-19 13:57:24.588770 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt
+-rw-r--r--   0        0        0     2054 2023-07-19 13:57:24.589254 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1565 2023-07-19 13:57:24.589472 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml
+-rw-r--r--   0        0        0      910 2023-07-19 13:57:24.589702 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml
+-rw-r--r--   0        0        0    10774 2023-07-19 13:57:24.589953 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml
+-rw-r--r--   0        0        0     2225 2023-07-19 13:57:24.590184 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml
+-rw-r--r--   0        0        0     3584 2023-07-19 13:57:24.590439 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml
+-rw-r--r--   0        0        0      367 2023-07-19 13:57:24.590616 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-service.yaml
+-rw-r--r--   0        0        0      316 2023-07-19 13:57:24.590824 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      379 2023-07-19 13:57:24.591193 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0    11587 2023-07-19 13:57:24.591487 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml
+-rw-r--r--   0        0        0     3453 2023-07-19 13:57:24.591783 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/README.md
+-rw-r--r--   0        0        0     1102 2023-07-19 13:57:24.592009 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf
+-rw-r--r--   0        0        0     1926 2023-07-19 13:57:24.592187 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf
+-rw-r--r--   0        0        0      468 2023-07-19 13:57:24.592418 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/variables.tf
+-rw-r--r--   0        0        0      170 2023-07-19 14:28:18.777464 matcha_ml-0.2.6/src/matcha_ml/runners/__init__.py
+-rw-r--r--   0        0        0     2478 2023-07-19 14:28:18.777841 matcha_ml-0.2.6/src/matcha_ml/runners/azure_runner.py
+-rw-r--r--   0        0        0     6546 2023-07-19 14:28:18.778250 matcha_ml-0.2.6/src/matcha_ml/runners/base_runner.py
+-rw-r--r--   0        0        0     2847 2023-07-19 14:28:18.778557 matcha_ml-0.2.6/src/matcha_ml/runners/remote_state_runner.py
+-rw-r--r--   0        0        0      103 2023-07-19 13:57:24.593553 matcha_ml-0.2.6/src/matcha_ml/services/__init__.py
+-rw-r--r--   0        0        0      646 2023-07-19 13:57:24.593744 matcha_ml-0.2.6/src/matcha_ml/services/_validation.py
+-rw-r--r--   0        0        0     4711 2023-07-19 14:28:18.778966 matcha_ml-0.2.6/src/matcha_ml/services/analytics_service.py
+-rw-r--r--   0        0        0    10848 2023-07-19 14:28:18.779487 matcha_ml-0.2.6/src/matcha_ml/services/azure_service.py
+-rw-r--r--   0        0        0     4542 2023-07-19 14:28:18.780112 matcha_ml-0.2.6/src/matcha_ml/services/global_parameters_service.py
+-rw-r--r--   0        0        0     5609 2023-07-19 14:28:18.780501 matcha_ml-0.2.6/src/matcha_ml/services/terraform_service.py
+-rw-r--r--   0        0        0      213 2023-07-19 14:28:18.780856 matcha_ml-0.2.6/src/matcha_ml/state/__init__.py
+-rw-r--r--   0        0        0    12364 2023-07-19 14:28:18.781389 matcha_ml-0.2.6/src/matcha_ml/state/matcha_state.py
+-rw-r--r--   0        0        0    11275 2023-07-19 14:28:18.782017 matcha_ml-0.2.6/src/matcha_ml/state/remote_state_manager.py
+-rw-r--r--   0        0        0       94 2023-07-19 13:57:24.595939 matcha_ml-0.2.6/src/matcha_ml/storage/__init__.py
+-rw-r--r--   0        0        0     9883 2023-07-19 14:28:18.782566 matcha_ml-0.2.6/src/matcha_ml/storage/azure_storage.py
+-rw-r--r--   0        0        0      184 2023-07-19 13:57:24.596527 matcha_ml-0.2.6/src/matcha_ml/templates/__init__.py
+-rw-r--r--   0        0        0     1923 2023-07-19 14:28:18.783143 matcha_ml-0.2.6/src/matcha_ml/templates/azure_template.py
+-rw-r--r--   0        0        0     7255 2023-07-19 13:57:24.597046 matcha_ml-0.2.6/src/matcha_ml/templates/base_template.py
+-rw-r--r--   0        0        0      635 2023-07-19 13:57:24.597267 matcha_ml-0.2.6/src/matcha_ml/templates/remote_state_template.py
+-rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 matcha_ml-0.2.6/PKG-INFO
```

### Comparing `matcha_ml-0.2.5/LICENSE` & `matcha_ml-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/README.md` & `matcha_ml-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/pyproject.toml` & `matcha_ml-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matcha-ml"
-version = "0.2.5"
+version = "0.2.6"
 description = "Matcha: An open source tool for provisioning MLOps environments to the cloud."
 authors = ["FuzzyLabs <info@fuzzylabs.ai>"]
 license = "Apache-2.0"
 homepage = "http://fuzzylabs.github.io/matcha"
 documentation = "http://fuzzylabs.github.io/matcha"
 repository = "https://github.com/fuzzylabs/matcha"
 readme = "README.md"
@@ -46,15 +46,15 @@
 typer = {extras = ["all"], version = "^0.7.0"}
 python-terraform = "^0.10.1"
 azure-identity = "^1.12.0"
 azure-mgmt-resource = "^23.0.0"
 azure-mgmt-subscription = "^3.1.1"
 azure-mgmt-authorization = "^3.0.0"
 azure-mgmt-confluent = "^1.0.0"
-pyyaml = "^5.4.1"
+pyyaml = "^6.0.1"
 types-pyyaml = "^6.0.12.9"
 segment-analytics-python = "^2.2.2"
 azure-mgmt-storage = "^21.0.0"
 dataclasses-json = "^0.5.7"
 azure-storage-blob = "^12.16.0"
 urllib3 = "1.26.6"
 types-urllib3 = "^1.26.25.13"
@@ -67,14 +67,16 @@
 pytest-cov = "^4.0.0"
 mypy = "^1.1.1"
 
 [tool.poetry.group.doc.dependencies]
 mkdocs-glightbox = "^0.3.4"
 pymdown-extensions = "10.0"
 mkdocs-material = "^9.1.12"
+mkdocstrings = "0.22.0"
+mkdocstrings-python = "1.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 show_error_codes = true
@@ -147,7 +149,11 @@
 
 [[tool.mypy.overrides]]
 module = [
     "python_terraform.*",
     "segment.*"
 ]
 ignore_missing_imports = true
+
+[tool.ruff.pylint]
+max-branches = 13
+max-args = 6
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/cli/cli.py` & `matcha_ml-0.2.6/src/matcha_ml/cli/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,82 @@
 """Matcha CLI."""
-from typing import Optional
+from typing import Optional, Tuple
 
 import typer
 
-from matcha_ml import __version__
+from matcha_ml import __version__, core
 from matcha_ml.cli._validation import (
     prefix_typer_callback,
     region_typer_callback,
 )
 from matcha_ml.cli.constants import RESOURCE_MSG, STATE_RESOURCE_MSG
-from matcha_ml.cli.destroy import destroy_resources
-from matcha_ml.cli.provision import provision_resources
 from matcha_ml.cli.ui.print_messages import (
     print_error,
     print_resource_output,
     print_status,
 )
 from matcha_ml.cli.ui.resource_message_builders import (
     build_resource_output,
     hide_sensitive_in_output,
 )
-from matcha_ml.core import core
+from matcha_ml.cli.ui.status_message_builders import (
+    build_status,
+    build_step_success_status,
+)
+from matcha_ml.cli.ui.user_approval_functions import is_user_approved
 from matcha_ml.errors import MatchaError, MatchaInputError
-from matcha_ml.services.analytics_service import AnalyticsEvent, track
-from matcha_ml.state import RemoteStateManager
 
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
 analytics_app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
 app.add_typer(
     analytics_app,
     name="analytics",
     help="Enable or disable the collection of anonymous usage data (enabled by default).",
 )
 
 
-@app.command()
-@track(event_name=AnalyticsEvent.PROVISION)
+def fill_provision_variables(
+    location: str,
+    prefix: str,
+    password: str,
+) -> Tuple[str, str, str]:
+    """Prompt for the provision variables if they were not provided.
+
+    Args:
+        location (str): Azure location in which all resources will be provisioned, or empty string to fill in.
+        prefix (str): Prefix used for all resources, or empty string to fill in.
+        password (str): Password for ZenServer, or empty string to fill in.
+
+    Returns:
+        Tuple[str, str, str]: A tuple of location, prefix and password which were filled in
+    """
+    if not location:
+        location = typer.prompt(
+            default=None,
+            text="What region should your resources be provisioned in (e.g., 'ukwest')?",
+            value_proc=region_typer_callback,
+        )
+    if not prefix:
+        prefix = typer.prompt(
+            text="Your resources need a name (an alphanumerical prefix; 3-11 character limit), what should matcha call them?",
+            default="matcha",
+            value_proc=prefix_typer_callback,
+        )
+    if not password:
+        password = typer.prompt(
+            default=None,
+            text="Set a password for your deployment server",
+            confirmation_prompt=True,
+            hide_input=True,
+        )
+
+    return location, prefix, password
+
+
+@app.command(help="Provision cloud resources.")
 def provision(
     location: str = typer.Option(
         callback=region_typer_callback,
         default="",
         help="The region where your resources will be provisioned, e.g., 'ukwest'",
     ),
     prefix: str = typer.Option(
@@ -51,20 +88,43 @@
         default="",
         help="A password for the deployment server",
     ),
     verbose: Optional[bool] = typer.Option(
         False, help="Get more detailed information from matcha provision!"
     ),
 ) -> None:
-    """Provision cloud resources with a template."""
-    provision_resources(location, prefix, password, verbose)
+    """Provision cloud resources.
+
+    Args:
+        location (Optional[str]): Azure location in which all resources will be provisioned.
+        prefix (Optional[str]): Prefix used for all resources.
+        password (Optional[str]): Password for ZenServer.
+        verbose (Optional[bool]): additional output is show when True. Defaults to False.
+
+    Raises:
+        Exit: Exit if resources are already provisioned.
+    """
+    location, prefix, password = fill_provision_variables(location, prefix, password)
+    if is_user_approved(verb="provision", resources=RESOURCE_MSG):
+        try:
+            _ = core.provision(location, prefix, password, verbose)
+        except MatchaError as e:
+            print_error(str(e))
+            raise typer.Exit()
+        print_status(build_step_success_status("Provisioning is complete!"))
+    else:
+        print_status(
+            build_status(
+                "You decided to cancel - if you change your mind, then run 'matcha provision' again."
+            )
+        )
+        raise typer.Exit()
 
 
 @app.command(help="Get information for the provisioned resources.")
-@track(event_name=AnalyticsEvent.GET)
 def get(
     resource_name: Optional[str] = typer.Argument(None),
     property_name: Optional[str] = typer.Argument(None),
     output: Optional[str] = typer.Option(
         default=None,
         help="The format of your output, e.g., 'json', 'yaml'.",
     ),
@@ -83,36 +143,51 @@
 
     Raises:
         Exit: Exit if matcha remote state has not been provisioned.
         Exit: Exit if matcha.state file does not exist.
         Exit: Exit if resource type or property does not exist in matcha.state.
     """
     try:
-        resources = core.get(resource_name, property_name)
+        resources = core.get(resource_name, property_name).to_dict()
     except MatchaInputError as e:
         print_error(str(e))
         raise typer.Exit()
     except MatchaError as e:
         print_error(str(e))
         raise typer.Exit()
 
     if not show_sensitive:
         resources = hide_sensitive_in_output(resources)
 
-    resource_output = build_resource_output(resources=resources, output_format=output)
+    resource_output = build_resource_output(
+        matcha_state=resources, output_format=output
+    )
     print_resource_output(resource_output=resource_output, output_format=output)
 
 
 @app.command()
-@track(event_name=AnalyticsEvent.DESTROY)
 def destroy() -> None:
-    """Destroy the provisioned cloud resources."""
-    remote_state_manager = RemoteStateManager()
-    destroy_resources(resources=STATE_RESOURCE_MSG + RESOURCE_MSG)
-    remote_state_manager.deprovision_remote_state()
+    """Destroy the provisioned cloud resources.
+
+    Raises:
+        Exit: Exit if core.destroy throws a MatchaError.
+    """
+    if is_user_approved(verb="destroy", resources=RESOURCE_MSG + STATE_RESOURCE_MSG):
+        try:
+            core.destroy()
+            print_status(build_step_success_status("Destroying resources is complete!"))
+        except MatchaError as e:
+            print_error(str(e))
+            raise typer.Exit()
+    else:
+        print_status(
+            build_status(
+                "You decided to cancel - your resources will remain active! If you change your mind, then run 'matcha destroy' again."
+            )
+        )
 
 
 @app.command()
 def force_unlock() -> None:
     """Force unlock remote matcha state on Azure."""
     delete = typer.confirm("Are you sure you want to remove the lock forcefully?")
     if not delete:
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/cli/constants.py` & `matcha_ml-0.2.6/src/matcha_ml/cli/constants.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/cli/destroy.py` & `matcha_ml-0.2.6/src/matcha_ml/cli/destroy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Destroy CLI."""
 from typing import List, Tuple
 
 import typer
 
-from matcha_ml.cli._validation import check_current_deployment_exists
 from matcha_ml.cli.ui.print_messages import print_error, print_status
 from matcha_ml.cli.ui.status_message_builders import (
     build_status,
     build_step_success_status,
 )
+from matcha_ml.cli.ui.user_approval_functions import is_user_approved
 from matcha_ml.runners import AzureRunner
 from matcha_ml.state import RemoteStateManager
 
 
 def destroy_resources(resources: List[Tuple[str, str]]) -> None:
     """Destroy resources.
 
@@ -23,29 +23,23 @@
         typer.Exit: Exit if matcha remote state has not been provisioned.
         typer.Exit: if an existing deployment does not exist.
         typer.Exit: if approval is not given by user.
     """
     remote_state = RemoteStateManager()
     if not remote_state.is_state_provisioned():
         print_error(
-            "Error - resources that have not been provisioned cannot be destroy. Run 'matcha provision' to get started!"
+            "Error - resources that have not been provisioned cannot be destroyed. Run 'matcha provision' to get started!"
         )
         raise typer.Exit()
 
     with remote_state.use_lock(), remote_state.use_remote_state():
         # create a runner for deprovisioning resource with Terraform service.
         template_runner = AzureRunner()
 
-        if not check_current_deployment_exists():
-            print_error(
-                "Error - you cannot destroy resources that have not been provisioned yet."
-            )
-            raise typer.Exit()
-
-        if template_runner.is_approved(verb="destroy", resources=resources):
+        if is_user_approved(verb="destroy", resources=resources):
             # deprovision the resources
             template_runner.deprovision()
             print_status(build_step_success_status("Destroying resources is complete!"))
         else:
             print_status(
                 build_status(
                     "You decided to cancel - your resources will remain active! If you change your mind, then run 'matcha destroy' again."
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/cli/ui/print_messages.py` & `matcha_ml-0.2.6/src/matcha_ml/cli/ui/print_messages.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/cli/ui/spinner.py` & `matcha_ml-0.2.6/src/matcha_ml/cli/ui/spinner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Implements a context manager interface using the __enter__() and __exit__() methods.
     """
 
     status: str
     progress: Progress
 
     def __init__(self, status: str):
-        """Initialise a spinner using Progress.
+        """Initialize a spinner using Progress.
 
         Args:
             status (str): task description
         """
         self.status = status
         self.progress = Progress(
             SpinnerColumn(spinner_name=SPINNER),
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/cli/ui/status_message_builders.py` & `matcha_ml-0.2.6/src/matcha_ml/cli/ui/status_message_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,57 +28,57 @@
 
     return message
 
 
 def build_status(status: str) -> str:
     """Build information status message.
 
-    Use white colour for formatting
+    Use white color for formatting
 
     Args:
         status: status message
 
     Returns:
         str: formatted message
     """
     return f"[bright_white]{status}[/bright_white]"
 
 
 def build_step_success_status(status: str) -> str:
     """Build step success status message.
 
-    Use green colour and bold font for formatting
+    Use green color and bold font for formatting
 
     Args:
         status: status message
 
     Returns:
         str: formatted message
     """
     return f"[green bold]{status}[/green bold]"
 
 
 def build_substep_success_status(status: str) -> str:
     """Build sub-step success status message.
 
-    Use green colour for formatting
+    Use green color for formatting
 
     Args:
         status: status message
 
     Returns:
         str: formatted message
     """
     return f"[green]{status}[/green]"
 
 
 def build_warning_status(status: str) -> str:
     """Build warning status message.
 
-    Use yellow colour for formatting
+    Use yellow color for formatting
 
     Args:
         status: status message
 
     Returns:
         str: formatted message
     """
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/errors.py` & `matcha_ml-0.2.6/src/matcha_ml/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any
 
 
 class MatchaError(Exception):
     """Matcha generic Error."""
 
     def __init__(self, message: str, *args: Any, **kwargs: Any):
-        """Initialise Matcha Error.
+        """Initialize Matcha Error.
 
         Args:
             message: the error message to propagate to the user
             *args: args
             **kwargs: kwargs
         """
         super().__init__(message, *args, **kwargs)
@@ -19,15 +19,15 @@
 class MatchaPermissionError(MatchaError):
     """Matcha Permission Error.
 
     Raised when the user does not have the appropriate permissions.
     """
 
     def __init__(self, message: str, *args: Any, **kwargs: Any):
-        """Initialise Matcha Permission Error.
+        """Initialize Matcha Permission Error.
 
         Args:
             message: the error message to propagate to the user
             *args: args
             **kwargs: kwargs
         """
         super().__init__(message, *args, **kwargs)
@@ -36,15 +36,15 @@
 class MatchaAuthenticationError(MatchaError):
     """Matcha Authentication Error.
 
     Raised when the user is not authenticated with an external service.
     """
 
     def __init__(self, auth_error: str, *args: Any, **kwargs: Any):
-        """The initialiser for the Authentication error.
+        """The initializer for the Authentication error.
 
         Args:
             auth_error (str): the error to propagate to the user.
             *args: additional arguments to pass to the Exception base class.
             **kwargs: additional key word arguments to pass to the Exception base class.
         """
         message = f"Error - Matcha couldn't authenticate you with Azure: {auth_error}, make sure you've run 'az login'!"
@@ -54,15 +54,15 @@
 class MatchaInputError(MatchaError):
     """Matcha Input Error.
 
     Raised when the user inputs a bad value.
     """
 
     def __init__(self, *args: Any, **kwargs: Any):
-        """The initialiser for Input error.
+        """The initializer for Input error.
 
         Args:
             *args: additional arguments to pass to the Exception base class.
             **kwargs: additional key word arguments to pass to the Exception base class.
         """
         super().__init__(*args, **kwargs)
 
@@ -70,16 +70,18 @@
 class MatchaTerraformError(MatchaError):
     """Matcha Terraform Error.
 
     Raised when terraform fails to run.
     """
 
     def __init__(self, tf_error: str, *args: Any, **kwargs: Any):
-        """Initialise Matcha Terraform Error.
+        """Initialize Matcha Terraform Error.
 
         Args:
             tf_error: terraform error
             *args: args
             **kwargs: kwargs
         """
-        message = f"Terraform failed because of the following error: '{tf_error}'."
+        message = (
+            f"Terraform failed because of the following error: '{tf_error}'."
+        )
         super().__init__(message, *args, **kwargs)
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.gitignore` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/output.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.gitignore` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/output.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/configure_kubectl.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/configure_kubectl.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/kubernetes.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/kubernetes.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/main.tf`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
   depends_on = [null_resource.configure_local_kubectl]
 
   # storage variables
   storage_account_name      = module.storage.storage_account_name
   storage_container_name    = module.storage.storage_container_name
   artifact_azure_access_key = module.storage.primary_access_key
-
 }
 
 
 module "zenserver" {
   source = "./zen_server"
 
   depends_on = [null_resource.configure_local_kubectl]
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/output.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/output.tf`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 output "experiment_tracker_mlflow_tracking_url" {
   description = "The URL for the MLflow tracking server"
   value       = module.mlflow.mlflow_tracking_url
 }
 
+output "experiment_tracker_mlflow_azure_connection_string" {
+  description = "The Azure connection string for the MLflow artifact storage"
+  value       = module.storage.primary_connection_string
+  sensitive   = true
+}
+
 output "pipeline_zenml_storage_path" {
   description = "The Azure Blob Storage Container path for storing ZenML artifacts"
   value       = module.zenml_storage.zenml_blobstorage_container_path
 }
 
 output "pipeline_zenml_connection_string" {
   description = "The primary connection string for the ZenML Azure Storage Account"
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/providers.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/providers.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/istio.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/istio.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/outputs.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/permissions.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/permissions.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/output.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/variables.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/sql.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/sql.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/variables.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/README.md` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf` & `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/runners/azure_runner.py` & `matcha_ml-0.2.6/src/matcha_ml/runners/base_runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,170 @@
 """Run terraform templates to provision and deprovision resources."""
-import json
-import uuid
-from collections import defaultdict
-from typing import Dict, List, Tuple
+import os
+from typing import Optional, Tuple
 
 import typer
 
 from matcha_ml.cli.ui.emojis import Emojis
-from matcha_ml.cli.ui.print_messages import (
-    print_error,
-    print_json,
-    print_status,
-)
-from matcha_ml.cli.ui.resource_message_builders import (
-    dict_to_json,
-    hide_sensitive_in_output,
-)
+from matcha_ml.cli.ui.print_messages import print_error, print_status
+from matcha_ml.cli.ui.spinner import Spinner
 from matcha_ml.cli.ui.status_message_builders import (
-    build_resource_confirmation,
     build_status,
+    build_substep_success_status,
 )
-from matcha_ml.errors import MatchaInputError
-from matcha_ml.runners.base_runner import BaseRunner
+from matcha_ml.errors import MatchaTerraformError
+from matcha_ml.services.terraform_service import TerraformConfig, TerraformService
+
+SPINNER = "dots"
+
 
-RESOURCE_NAMES = [
-    "experiment_tracker",
-    "pipeline",
-    "orchestrator",
-    "cloud",
-    "container_registry",
-    "model_deployer",
-]
-
-
-class AzureRunner(BaseRunner):
-    """A Runner class provides methods that interface with the Terraform service to facilitate the provisioning and deprovisioning of resources."""
-
-    def __init__(self) -> None:
-        """Initialize AzureRunner class."""
-        super().__init__()
+class BaseRunner:
+    """A BaseRunner class provides methods that interface with the Terraform service to facilitate the provisioning and deprovisioning of resources."""
 
-    def is_approved(self, verb: str, resources: List[Tuple[str, str]]) -> bool:
-        """Get approval from user to modify resources on cloud.
+    def __init__(self, working_dir: Optional[str] = None) -> None:
+        """Initialize BaseRunner class.
 
         Args:
-            verb (str): the verb to use in the approval message.
-            resources(list): the list of resources to be actioned by the verb to be provided to the user as a status message
+            working_dir (Optional[str]): Working directory for terraform. Defaults to None.
+        """
+        if working_dir is not None:
+            working_dir = working_dir
+        else:
+            working_dir = TerraformConfig().working_dir
+        self.terraform_config = TerraformConfig(working_dir=working_dir)
+        self.tfs = TerraformService(self.terraform_config)
+        self.tf_state_dir = self.tfs.get_tf_state_dir()
+
+    def _check_terraform_installation(self) -> None:
+        """Checks if terraform is installed on the host system.
 
-        Returns:
-            bool: True if user approves, False otherwise.
+        Raises:
+            typer.Exit: if terraform is not installed.
         """
-        summary_message = build_resource_confirmation(
-            header=f"The following resources will be {verb}ed",
-            resources=resources,
-            footer=f"{verb.capitalize()}ing the resources may take approximately 20 minutes. May we suggest you grab a cup of {Emojis.MATCHA.value}?",
-        )
+        if not self.tfs.check_installation():
+            print_error(f"{Emojis.CROSS.value} Terraform is not installed")
+            print_error(
+                "Terraform is required for to run and was not found installed on your machine. "
+                "Please visit https://learn.hashicorp.com/tutorials/terraform/install-cli to install it."
+            )
+            raise typer.Exit()
 
-        print_status(summary_message)
-        return typer.confirm(f"Are you happy for '{verb}' to run?")
+    def _validate_terraform_config(self) -> None:
+        """Validate the configuration used for creating resources.
 
-    def _build_resource_output(self, output_name: str) -> Tuple[str, str, str]:
-        """Build resource output for each Terraform output.
+        Raises:
+            typer.Exit: if `terraform.tfvars.json` file not found in current directory.
+        """
+        if not self.tfs.validate_config():
+            print_error(
+                "The file terraform.tfvars.json was not found in the "
+                f"current directory at {self.tfs.config.var_file}. Please "
+                "verify if it exists."
+            )
+            raise typer.Exit()
 
-        Args:
-            output_name (str): the name of the Terraform output.
+    def _validate_kubeconfig(self, base_path: str = ".kube/config") -> None:
+        """Check if kubeconfig file exists at location '~/.kube/config', if not create empty config file.
 
-        Returns:
-            Tuple[str, str, str]: the resource output for matcha.state.
+        Args:
+            base_path (str): Relative path to location of kubeconfig
         """
-        resource_type: str
+        self.tfs.verify_kubectl_config_file(base_path)
 
-        for key in RESOURCE_NAMES:
-            if key in output_name:
-                resource_type = key
-                break
+    def _initialize_terraform(self, msg: str = "", destroy: bool = False) -> None:
+        """Run terraform init to initialize Terraform .
 
-        if resource_type is None:
-            print_error(
-                "A valid resource type for the output '{output_name}' does not exist."
+        Raises:
+            MatchaTerraformError: if 'terraform init' failed.
+            msg (str) : Message to display. Default is empty string.
+            destroy (bool): whether this function is being called in a destructive context
+        """
+        if self.tf_state_dir.exists():
+            if not destroy:
+                # this directory gets created after a successful init command
+                print_status(
+                    build_status(
+                        f"matcha {Emojis.MATCHA.value} has already been initialized. Skipping this step..."
+                    )
+                )
+
+        else:
+            print_status(
+                build_status(
+                    f"\n{Emojis.WAITING.value} Brewing matcha {Emojis.MATCHA.value}...\n"
+                )
             )
-            raise MatchaInputError()
 
-        flavour_and_resource_name = output_name[len(resource_type) + 1 :]
+            with Spinner("Initializing"):
+                ret_code, _, err = self.tfs.init()
 
-        flavor, resource_name = flavour_and_resource_name.split("_", maxsplit=1)
-        resource_name = resource_name.replace("_", "-")
-        resource_type = resource_type.replace("_", "-")
+                if ret_code != 0:
+                    print_error("The command 'terraform init' failed.")
+                    raise MatchaTerraformError(tf_error=err)
+
+            print_status(
+                build_substep_success_status(
+                    f"{Emojis.CHECKMARK.value} {msg} {Emojis.MATCHA.value} initialized!\n"
+                )
+            )
 
-        return resource_type, flavor, resource_name
+    def _check_matcha_directory_exists(self) -> None:
+        """Checks if .matcha directory exists within the current working directory.
 
-    def _write_outputs_state(self) -> None:
-        """Write the outputs of the Terraform deployment to the state JSON file."""
-        tf_outputs = self.tfs.terraform_client.output()
-        state_outputs: Dict[str, Dict[str, str]] = defaultdict(dict)
+        Raises:
+            typer.Exit: if the .matcha directory does not exist.
+            typer.Exit: if the .matcha directory does not contain the required files to deploy resources.
+        """
+        if not self.tfs.check_matcha_directory_exists():
+            print_error(
+                f"Error, the .matcha directory does not exist in {os.getcwd()} . Please ensure you are trying to destroy resources that you have provisioned in the current working directory."
+            )
+            raise typer.Exit()
 
-        for output_name, properties in tf_outputs.items():
-            resource_type, flavor, resource_name = self._build_resource_output(
-                output_name
+        if not self.tfs.check_matcha_directory_integrity():
+            print_error(
+                "Error, the .matcha directory does not contain files relating to deployed resources. Please ensure you are trying to destroy resources that you have provisioned in the current working directory."
             )
-            state_outputs[resource_type].setdefault("flavor", flavor)
-            state_outputs[resource_type][resource_name] = properties["value"]
+            raise typer.Exit()
 
-        # Create a unique matcha state identifier
-        state_outputs["id"] = {"matcha_uuid": str(uuid.uuid4())}
+    def _apply_terraform(self) -> None:
+        """Run terraform apply to create resources on cloud.
 
-        self._update_state_file(state_outputs)
+        Raises:
+            MatchaTerraformError: if 'terraform apply' failed.
+        """
+        with Spinner("Applying"):
+            ret_code, _, err = self.tfs.apply()
 
-    def _update_state_file(self, state_outputs: Dict[str, Dict[str, str]]) -> None:
-        """Read and update the matcha state file with new provisioned resources.
+            if ret_code != 0:
+                raise MatchaTerraformError(tf_error=err)
+        print_status(
+            build_substep_success_status(
+                f"{Emojis.CHECKMARK.value} Matcha resources have been provisioned!\n"
+            )
+        )
 
-        Args:
-            state_outputs (Dict[str, Dict[str, str]]): Dictionary containing outputs to be written to state file.
-        """
-        with open(self.state_file, "w") as f:
-            json.dump(state_outputs, f, indent=4)
+    def _destroy_terraform(self, msg: str = "") -> None:
+        """Destroy the provisioned resources.
 
-    def _show_terraform_outputs(self) -> None:
-        """Print the terraform outputs from state file."""
-        self._write_outputs_state()
-        print_status(build_status("Here are the endpoints for what's been provisioned"))
-        # print terraform output from state file
-        with open(self.state_file) as fp:
-            resources_dict = hide_sensitive_in_output(json.loads(fp.read()))
-            resources_json = dict_to_json(resources_dict)
-            print_json(resources_json)
-
-    def _write_outputs_state_cloud_only(self) -> None:
-        """Write the outputs of the Terraform deployment to the state JSON file."""
-        with open(self.state_file) as f:
-            state_file_data = json.load(f)
-
-        updated_state_file_data = {}
-        for key, value in state_file_data.items():
-            if key in ["cloud", "id"]:
-                updated_state_file_data[key] = value
+        Raises:
+            MatchaTerraformError: if 'terraform destroy' failed.
+            msg (str) : Message to display. Default is empty string.
+        """
+        print()
+        print_status(
+            build_status(f"{Emojis.WAITING.value} Destroying {msg} resources...")
+        )
+        print()
+        with Spinner("Destroying"):
+            ret_code, _, err = self.tfs.destroy()
 
-        self._update_state_file(updated_state_file_data)
+            if ret_code != 0:
+                raise MatchaTerraformError(tf_error=err)
 
-    def provision(self) -> None:
+    def provision(self) -> Optional[Tuple[str, str, str]]:
         """Provision resources required for the deployment."""
-        self._check_terraform_installation()
-        self._validate_terraform_config()
-        self._validate_kubeconfig(base_path=".kube/config")
-        self._initialize_terraform(msg="Matcha")
-        self._apply_terraform()
-        self._show_terraform_outputs()
+        raise NotImplementedError
 
     def deprovision(self) -> None:
         """Destroy the provisioned resources."""
-        self._check_matcha_directory_exists()
-        self._check_terraform_installation()
-        self._initialize_terraform(msg="Matcha", destroy=True)
-        self._destroy_terraform(msg="Matcha")
-        self._write_outputs_state_cloud_only()
+        raise NotImplementedError
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/runners/remote_state_runner.py` & `matcha_ml-0.2.6/src/matcha_ml/runners/remote_state_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
         account_name = ""
         container_name = ""
         resource_group_name = ""
 
         prefix = "remote_state_storage"
         account_name = tf_outputs[f"{prefix}_account_name"]["value"]
-        resource_group_name = tf_outputs[f"{prefix}_resource_group_name"]["value"]
+        resource_group_name = tf_outputs[f"{prefix}_resource_group_name"][
+            "value"
+        ]
         container_name = tf_outputs[f"{prefix}_container_name"]["value"]
 
         return account_name, container_name, resource_group_name
 
     def _clean_up(self) -> None:
         """Remove the whole .matcha directory when destroy full is run."""
         matcha_template_dir = os.path.join(os.getcwd(), ".matcha")
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/services/_validation.py` & `matcha_ml-0.2.6/src/matcha_ml/services/_validation.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/services/azure_service.py` & `matcha_ml-0.2.6/src/matcha_ml/services/azure_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.has_permissions = self._check_required_role_assignments()
 
     def _check_authentication(self) -> bool:
         """Check whether the user is authenticated with 'az login'.
 
         Raises:
             MatchaAuthenticationError: when the Azure CLI is unable to be invoked.
-            MatchaAuthenticationError: when no access token is recieved.
+            MatchaAuthenticationError: when no access token is received.
 
         Returns:
             bool: True if the checks pass, an error is raised otherwise.
         """
         self._credential = AzureCliCredential()
         self._client = SubscriptionClient(self._credential)
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/services/global_parameters_service.py` & `matcha_ml-0.2.6/src/matcha_ml/services/global_parameters_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     _user_id: Optional[str] = None
     _analytics_opt_out: bool = False
 
     def __new__(cls) -> "GlobalParameters":
         """Creates a singleton instance of the GlobalParameters class.
 
         Returns:
-            GlobalParameters: Already existing initialised object, otherwise a new singleton object
+            GlobalParameters: Already existing initialized object, otherwise a new singleton object
         """
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             # Check if config.yaml file exists and read in variables to the class
             if os.path.exists(cls._instance.default_config_file_path):
                 cls._instance._read_global_config()
             else:
@@ -83,15 +83,15 @@
             yaml.dump(data, file)
 
     @property
     def user_id(self) -> str:
         """User ID getter.
 
         Returns:
-            str: Unqiue user ID string
+            str: Unique user ID string
         """
         if self._user_id is None:
             self._user_id = str(uuid4())
         return self._user_id
 
     @property
     def analytics_opt_out(self) -> bool:
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/services/terraform_service.py` & `matcha_ml-0.2.6/src/matcha_ml/services/terraform_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,14 @@
     """Configuration required for terraform."""
 
     # Path to terraform template are stored
     working_dir: str = os.path.join(
         os.getcwd(), ".matcha", "infrastructure", "resources"
     )
 
-    # state file to store output after terraform apply
-    @property
-    def state_file(self) -> str:
-        """The path to the state file."""
-        return os.path.join(self.working_dir, os.pardir, "matcha.state")
-
     # variables file
     @property
     def var_file(self) -> str:
         """The path to the variables file."""
         return os.path.join(self.working_dir, "terraform.tfvars.json")
 
     # if set to False terraform output will be printed to stdout/stderr
@@ -50,15 +44,16 @@
         """Initialize and/or return the terraform client.
 
         Returns:
             python_terraform.Terraform: The terraform client.
         """
         if self._terraform_client is None:
             self._terraform_client = python_terraform.Terraform(
-                working_dir=self.config.working_dir, var_file=self.config.var_file
+                working_dir=self.config.working_dir,
+                var_file=self.config.var_file,
             )
         return self._terraform_client
 
     def check_installation(self) -> bool:
         """Checks if terraform is installed on the host system.
 
         Raises:
@@ -67,15 +62,17 @@
         try:
             self.terraform_client.cmd(cmd="-help")
         except Exception:
             return False
 
         return True
 
-    def verify_kubectl_config_file(self, config_path: str = ".kube/config") -> None:
+    def verify_kubectl_config_file(
+        self, config_path: str = ".kube/config"
+    ) -> None:
         """Checks if kubeconfig is present at location ~/.kube/config.
 
         Args:
             config_path (str): Relative path to location of kubeconfig
 
         If not, it creates a empty config file.
         """
@@ -122,28 +119,28 @@
 
         Returns:
             Path: a Path object that represents the path to the `.terraform` folder.
         """
         return Path(os.path.join(self.config.working_dir, ".terraform"))
 
     def init(self) -> Tuple[int, str, str]:
-        """Run `terraform init` with the initialised Terraform client from the python_terraform module.
+        """Run `terraform init` with the initialized Terraform client from the python_terraform module.
 
         Returns:
             Tuple[int, str, str]: return code of Terraform, standard output and standard error.
         """
         ret_code, out, err = self.terraform_client.init(
             capture_output=self.config.capture_output,
             raise_on_error=False,
         )
 
         return ret_code, out, err
 
     def apply(self) -> Tuple[int, str, str]:
-        """Run `terraform apply` with the initialised Terraform client from the python_terraform module.
+        """Run `terraform apply` with the initialized Terraform client from the python_terraform module.
 
         Returns:
             Tuple[int, str, str]: return code of Terraform, standard output and standard error.
         """
         # once terraform init is success, call terraform apply
         ret_code, out, err = self.terraform_client.apply(
             input=False,
@@ -152,15 +149,15 @@
             skip_plan=True,
             auto_approve=True,
         )
 
         return ret_code, out, err
 
     def destroy(self) -> Tuple[int, str, str]:
-        """Destroy the provisioned resources with the initialised Terraform client from the python_terraform module..
+        """Destroy the provisioned resources with the initialized Terraform client from the python_terraform module..
 
         Returns:
             Tuple[int, str, str]: return code of terraform, standard output and standard error.
         """
         # Reference: https://github.com/beelit94/python-terraform/issues/108
         ret_code, out, err = self.terraform_client.destroy(
             capture_output=self.config.capture_output,
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/state/remote_state_manager.py` & `matcha_ml-0.2.6/src/matcha_ml/state/remote_state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from matcha_ml.cli.ui.print_messages import print_error, print_status
 from matcha_ml.cli.ui.status_message_builders import (
     build_step_success_status,
     build_warning_status,
 )
 from matcha_ml.constants import LOCK_FILE_NAME
 from matcha_ml.errors import MatchaError
-from matcha_ml.runners import RemoteStateRunner
+from matcha_ml.runners.remote_state_runner import RemoteStateRunner
 from matcha_ml.storage import AzureStorage
 from matcha_ml.templates import RemoteStateTemplate
 
 DEFAULT_CONFIG_NAME = "matcha.config.json"
 ALREADY_LOCKED_MESSAGE = (
     "Remote state is already locked, maybe someone else is using matcha?"
     " If you think this is a mistake, you can unlock the state by running 'matcha force-unlock'."
@@ -53,15 +53,15 @@
     """
 
     _azure_storage: Optional[AzureStorage] = None
 
     config_path: str
 
     def __init__(self, config_path: Optional[str] = None) -> None:
-        """Initialise Remote State Manager.
+        """Initialize Remote State Manager.
 
         Args:
             config_path (Optional[str]): optional configuration file path
         """
         if config_path is not None:
             self.config_path = config_path
         else:
@@ -211,28 +211,27 @@
             location=location, prefix=prefix
         )
         state_storage_template.build_template(config, template, destination, verbose)
 
         account_name, container_name, resource_group_name = template_runner.provision()
         self._write_matcha_config(account_name, container_name, resource_group_name)
         print_status(
-            build_step_success_status("Provisioning Matcha reources is complete!")
+            build_step_success_status(
+                "Provisioning Matcha resource group and remote state is complete!"
+            )
         )
         print()
 
     def deprovision_remote_state(self) -> None:
         """Destroy the state bucket provisioned."""
         # create a runner for deprovisioning resource with Terraform service.
         template_runner = RemoteStateRunner()
 
         template_runner.deprovision()
         self.remove_matcha_config()
-        print_status(
-            build_step_success_status("Destroying Matcha resources is complete!")
-        )
 
     def _write_matcha_config(
         self, account_name: str, container_name: str, resource_group_name: str
     ) -> None:
         """Write the outputs of the Terraform deployed state storage to a bucket config file.
 
         Args:
@@ -257,17 +256,18 @@
         print_status(
             build_step_success_status(
                 f"The matcha configuration is written to {self.config_path}"
             )
         )
 
     def remove_matcha_config(self) -> None:
-        """Remove the matcha.config.json file after destroy full is run."""
+        """Remove the matcha.config.json file."""
         try:
             os.remove(self.config_path)
+            self._azure_storage = None
         except FileNotFoundError:
             print_error(
                 f"Failed to remove the matcha.config.json file at {self.config_path}, file not found."
             )
 
     def download(self, dest_folder_path: str) -> None:
         """Download the remote state into the local matcha state directory.
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/storage/azure_storage.py` & `matcha_ml-0.2.6/src/matcha_ml/storage/azure_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Class to interact with Azure Storage."""
 import glob
 import hashlib
 import os
 import tempfile
-from typing import Set
+from typing import Optional, Set
 
 from azure.storage.blob import BlobClient, BlobServiceClient, ContainerClient
 
 from matcha_ml.constants import LOCK_FILE_NAME
 from matcha_ml.services.azure_service import AzureClient
 
 IGNORE_FOLDERS = [".terraform"]
 
 
 class AzureStorage:
     """Class to interact with Azure blob storage."""
 
     az_client: AzureClient
     blob_service_client: BlobServiceClient
+    account_name: Optional[str] = None
+    resource_group_name: Optional[str] = None
 
     def __init__(self, account_name: str, resource_group_name: str) -> None:
         """Initialize Azure Storage.
 
         Args:
             account_name (str): Azure storage account name
             resource_group_name (str): Name of resource group containing given account name
         """
+        self.account_name = account_name
+        self.resource_group_name = resource_group_name
         self.az_client = AzureClient()
         self.resource_group_exists = self.az_client.resource_group_exists(
             resource_group_name
         )
         if self.resource_group_exists:
             _conn_str = self.az_client.fetch_connection_string(
                 storage_account_name=account_name,
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/templates/azure_template.py` & `matcha_ml-0.2.6/src/matcha_ml/templates/azure_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Build a template for provisioning resources on Azure using terraform files."""
-import json
-import os
 from typing import Optional
 
+from matcha_ml.state import MatchaState, MatchaStateService
 from matcha_ml.templates.base_template import BaseTemplate, TemplateVariables
 
 SUBMODULE_NAMES = [
     "aks",
     "resource_group",
     "mlflow_module",
     "storage",
@@ -48,15 +47,12 @@
             template_src (str): path of the template to use.
             destination (str): destination path to write template to.
             verbose (Optional[bool]): additional output is shown when True. Defaults to False.
         """
         super().build_template(config, template_src, destination, verbose)
 
         # Add matcha.state file one directory above the template
-        state_file_destination = os.path.join(destination, os.pardir, "matcha.state")
-
         config_dict = vars(config)
         _ = config_dict.pop("password", None)
         initial_state_file_dict = {"cloud": config_dict}
-
-        with open(state_file_destination, "w") as f:
-            json.dump(initial_state_file_dict, f)
+        matcha_state = MatchaState.from_dict(initial_state_file_dict)
+        MatchaStateService(matcha_state=matcha_state)
```

### Comparing `matcha_ml-0.2.5/src/matcha_ml/templates/base_template.py` & `matcha_ml-0.2.6/src/matcha_ml/templates/base_template.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/src/matcha_ml/templates/remote_state_template.py` & `matcha_ml-0.2.6/src/matcha_ml/templates/remote_state_template.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.5/PKG-INFO` & `matcha_ml-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matcha-ml
-Version: 0.2.5
+Version: 0.2.6
 Summary: Matcha: An open source tool for provisioning MLOps environments to the cloud.
 Home-page: http://fuzzylabs.github.io/matcha
 License: Apache-2.0
 Keywords: production,mlops,devops,machine learning
 Author: FuzzyLabs
 Author-email: info@fuzzylabs.ai
 Requires-Python: >=3.8,<4.0
@@ -12,32 +12,27 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-mgmt-authorization (>=3.0.0,<4.0.0)
 Requires-Dist: azure-mgmt-confluent (>=1.0.0,<2.0.0)
 Requires-Dist: azure-mgmt-resource (>=23.0.0,<24.0.0)
 Requires-Dist: azure-mgmt-storage (>=21.0.0,<22.0.0)
 Requires-Dist: azure-mgmt-subscription (>=3.1.1,<4.0.0)
 Requires-Dist: azure-storage-blob (>=12.16.0,<13.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: python-terraform (>=0.10.1,<0.11.0)
-Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: segment-analytics-python (>=2.2.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0)
 Requires-Dist: types-urllib3 (>=1.26.25.13,<2.0.0.0)
 Requires-Dist: urllib3 (==1.26.6)
 Project-URL: Bug Tracker, https://github.com/fuzzylabs/matcha/issues
```

#### html2text {}

```diff
@@ -1,37 +1,33 @@
-Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.5 Summary: Matcha: An open
+Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.6 Summary: Matcha: An open
 source tool for provisioning MLOps environments to the cloud. Home-page: http:/
 /fuzzylabs.github.io/matcha License: Apache-2.0 Keywords:
 production,mlops,devops,machine learning Author: FuzzyLabs Author-email:
 info@fuzzylabs.ai Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: Implementation
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Dist: azure-identity
-(>=1.12.0,<2.0.0) Requires-Dist: azure-mgmt-authorization (>=3.0.0,<4.0.0)
-Requires-Dist: azure-mgmt-confluent (>=1.0.0,<2.0.0) Requires-Dist: azure-mgmt-
-resource (>=23.0.0,<24.0.0) Requires-Dist: azure-mgmt-storage
-(>=21.0.0,<22.0.0) Requires-Dist: azure-mgmt-subscription (>=3.1.1,<4.0.0)
-Requires-Dist: azure-storage-blob (>=12.16.0,<13.0.0) Requires-Dist:
-dataclasses-json (>=0.5.7,<0.6.0) Requires-Dist: python-terraform
-(>=0.10.1,<0.11.0) Requires-Dist: pyyaml (>=5.4.1,<6.0.0) Requires-Dist:
-requests (>=2.31.0,<3.0.0) Requires-Dist: segment-analytics-python
-(>=2.2.2,<3.0.0) Requires-Dist: typer[all] (>=0.7.0,<0.8.0) Requires-Dist:
-types-pyyaml (>=6.0.12.9,<7.0.0.0) Requires-Dist: types-urllib3
-(>=1.26.25.13,<2.0.0.0) Requires-Dist: urllib3 (==1.26.6) Project-URL: Bug
-Tracker, https://github.com/fuzzylabs/matcha/issues Project-URL: Documentation,
-http://fuzzylabs.github.io/matcha Project-URL: Repository, https://github.com/
-fuzzylabs/matcha Description-Content-Type: text/markdown
+Programming Language :: Python :: Implementation Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: azure-identity (>=1.12.0,<2.0.0) Requires-Dist: azure-
+mgmt-authorization (>=3.0.0,<4.0.0) Requires-Dist: azure-mgmt-confluent
+(>=1.0.0,<2.0.0) Requires-Dist: azure-mgmt-resource (>=23.0.0,<24.0.0)
+Requires-Dist: azure-mgmt-storage (>=21.0.0,<22.0.0) Requires-Dist: azure-mgmt-
+subscription (>=3.1.1,<4.0.0) Requires-Dist: azure-storage-blob
+(>=12.16.0,<13.0.0) Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0) Requires-
+Dist: python-terraform (>=0.10.1,<0.11.0) Requires-Dist: pyyaml
+(>=6.0.1,<7.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
+segment-analytics-python (>=2.2.2,<3.0.0) Requires-Dist: typer[all]
+(>=0.7.0,<0.8.0) Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0) Requires-
+Dist: types-urllib3 (>=1.26.25.13,<2.0.0.0) Requires-Dist: urllib3 (==1.26.6)
+Project-URL: Bug Tracker, https://github.com/fuzzylabs/matcha/issues Project-
+URL: Documentation, http://fuzzylabs.github.io/matcha Project-URL: Repository,
+https://github.com/fuzzylabs/matcha Description-Content-Type: text/markdown
    ****** [https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/
                                logo.png] ******
                     [Build] [License] [Release] [Downloads]
                **** Open source MLOps on Azure in one step ****
 If you train machine learning models, then you know the challenge of going from
 _experiment_ to _production_. There's a vast range of tools that promise to
 help, from experiment tracking through to model deployment, but setting these
```

