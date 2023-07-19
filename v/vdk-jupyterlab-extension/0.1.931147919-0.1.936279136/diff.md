# Comparing `tmp/vdk_jupyterlab_extension-0.1.931147919.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.936279136.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.931147919.tar` & `vdk_jupyterlab_extension-0.1.936279136.tar`

### file list

```diff
@@ -1,81 +1,79 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/install.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/jest.config.js
--rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/package-lock.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/tsconfig.json
--rw-r--r--   0        0        0   421787 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/schema/plugin.json
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/handler.ts
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/index.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/jobData.ts
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/vdkTags.ts
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/delete-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/DeleteJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/remoteEntry.b6f98de260318ecd5e13.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.931147919/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/install.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/jest.config.js
+-rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/package-lock.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/tsconfig.json
+-rw-r--r--   0        0        0   423537 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/schema/plugin.json
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/handler.ts
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/index.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/jobData.ts
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/vdkTags.ts
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    15543 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/381.0485c5d1f906c39de85e.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/remoteEntry.77b468e1169ec9f71a16.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.936279136/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/jest.config.js` & `vdk_jupyterlab_extension-0.1.936279136/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/package-lock.json` & `vdk_jupyterlab_extension-0.1.936279136/package-lock.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/package.json` & `vdk_jupyterlab_extension-0.1.936279136/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.936279136'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.931147919"
+    "version": "0.1.936279136"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/tsconfig.json` & `vdk_jupyterlab_extension-0.1.936279136/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/yarn.lock` & `vdk_jupyterlab_extension-0.1.936279136/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1197,17 +1197,17 @@
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
 "@jupyter/ydoc@~0.2.3", "@jupyter/ydoc@~0.2.4":
-  version "0.2.4"
-  resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.4.tgz#bc312f171777b58e286aadca62dadeca3a894dd1"
-  integrity sha512-QACcB4bF+Ew4UJmJP+3OyiyQm3vwRYF6iZCQK9q0nE2U5uAosQkfLyT6Bx71jPUXe4G9lEF6m9fjpZvSUX7Lyw==
+  version "0.2.5"
+  resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.5.tgz#8241bce5798a3c10761df7e7045c0b4e24abf868"
+  integrity sha512-XsAAkq55k6UCIv2kAFKbWahiuCsSxLQaRuWfULUuAhKVnA/QD2gqVMYx2yvnB0+AR7PKpKdf65uUxGxnSTBKqA==
   dependencies:
     "@jupyterlab/nbformat" "^3.0.0 || ^4.0.0-alpha.15"
     "@lumino/coreutils" "^1.11.0 || ^2.0.0-alpha.6"
     "@lumino/disposable" "^1.10.0 || ^2.0.0-alpha.6"
     "@lumino/signaling" "^1.10.0 || ^2.0.0-alpha.6"
     y-protocols "^1.0.5"
     yjs "^13.5.40"
@@ -2963,14 +2963,26 @@
   integrity sha512-HGyxoOTYUyCM6stUe6EJgnd4EoewAI7zMdfqO+kGjnlZmBDz/cR5pf8r/cR4Wq60sL/p0IkcjUEEPwS3GFrIyw==
 
 array-unique@^0.3.2:
   version "0.3.2"
   resolved "https://registry.yarnpkg.com/array-unique/-/array-unique-0.3.2.tgz#a894b75d4bc4f6cd679ef3244a9fd8f46ae2d428"
   integrity sha512-SleRWjh9JUud2wH1hPs9rZBZ33H6T9HOiL0uwGnGx9FpE6wKGyfWugmbkEOIs6qWrZhg0LWeLziLrEwQJhs5mQ==
 
+arraybuffer.prototype.slice@^1.0.1:
+  version "1.0.1"
+  resolved "https://registry.yarnpkg.com/arraybuffer.prototype.slice/-/arraybuffer.prototype.slice-1.0.1.tgz#9b5ea3868a6eebc30273da577eb888381c0044bb"
+  integrity sha512-09x0ZWFEjj4WD8PDbykUwo3t9arLn8NIzmmYEJFpYekOAQjpkGSyrQhNoRTcwwcFRu+ycWF78QZ63oWTqSjBcw==
+  dependencies:
+    array-buffer-byte-length "^1.0.0"
+    call-bind "^1.0.2"
+    define-properties "^1.2.0"
+    get-intrinsic "^1.2.1"
+    is-array-buffer "^3.0.2"
+    is-shared-array-buffer "^1.0.2"
+
 arrify@^1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/arrify/-/arrify-1.0.1.tgz#898508da2226f380df904728456849c1501a4b0d"
   integrity sha512-3CYzex9M9FGQjCGMGyi6/31c8GJbgb0qGyrx5HWxPd0aCwh4cB2YjMb2Xf9UuoogrMrlO9cTqnB5rI5GHZTcUA==
 
 assign-symbols@^1.0.0:
   version "1.0.0"
@@ -3292,17 +3304,17 @@
 
 camelcase@^6.0.0, camelcase@^6.2.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-6.3.0.tgz#5685b95eb209ac9c0c177467778c9c84df58ba9a"
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
 caniuse-lite@^1.0.30001503:
-  version "1.0.30001515"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001515.tgz#418aefeed9d024cd3129bfae0ccc782d4cb8f12b"
-  integrity sha512-eEFDwUOZbE24sb+Ecsx3+OvNETqjWIdabMy52oOkIgcUtAsQifjUG9q4U9dgTHJM2mfk4uEPxc0+xuFdJ629QA==
+  version "1.0.30001516"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001516.tgz#621b1be7d85a8843ee7d210fd9d87b52e3daab3a"
+  integrity sha512-Wmec9pCBY8CWbmI4HsjBeQLqDTqV91nFVR83DnZpYyRnPI1wePDsTg0bGLPC5VU/3OIZV1fmxEea1b+tFKe86g==
 
 capture-exit@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/capture-exit/-/capture-exit-2.0.0.tgz#fb953bfaebeb781f62898239dabb426d08a509a4"
   integrity sha512-PiT/hQmTonHhl/HFGN+Lx3JJUznrVYJ3+AQsnthneZbvW7x+f08Tk7yLJTLEOUvBTbduLeeBkxEaYXUOUrRq6g==
   dependencies:
     rsvp "^4.8.4"
@@ -3877,17 +3889,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.460"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.460.tgz#f360a5059c039c4a5fb4dfa99680ad8129dd9f84"
-  integrity sha512-kKiHnbrHME7z8E6AYaw0ehyxY5+hdaRmeUbjBO22LZMdqTYCO29EvF0T1cQ3pJ1RN5fyMcHl1Lmcsdt9WWJpJQ==
+  version "1.4.464"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.464.tgz#2f94bad78dff34e527aacbfc5d0b1a33cf046507"
+  integrity sha512-guZ84yoou4+ILNdj0XEbmGs6DEWj6zpVOWYpY09GU66yEb0DSYvP/biBPzHn0GuW/3RC/pnaYNUWlQE1fJYtgA==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -3963,19 +3975,20 @@
   version "1.3.2"
   resolved "https://registry.yarnpkg.com/error-ex/-/error-ex-1.3.2.tgz#b4ac40648107fdcdcfae242f428bea8a14d4f1bf"
   integrity sha512-7dFHNmqeFSEt2ZBsCriorKnn3Z2pj+fd9kmI6QoWw4//DL+icEBfc0U7qJCisqrTsKTjw4fNFy2pW9OqStD84g==
   dependencies:
     is-arrayish "^0.2.1"
 
 es-abstract@^1.19.0, es-abstract@^1.20.4:
-  version "1.21.3"
-  resolved "https://registry.yarnpkg.com/es-abstract/-/es-abstract-1.21.3.tgz#8aaa0ffc080e8a6fef6ace72631dc1ec5d47bf94"
-  integrity sha512-ZU4miiY1j3sGPFLJ34VJXEqhpmL+HGByCinGHv4HC+Fxl2fI2Z4yR6tl0mORnDr6PA8eihWo4LmSWDbvhALckg==
+  version "1.22.1"
+  resolved "https://registry.yarnpkg.com/es-abstract/-/es-abstract-1.22.1.tgz#8b4e5fc5cefd7f1660f0f8e1a52900dfbc9d9ccc"
+  integrity sha512-ioRRcXMO6OFyRpyzV3kE1IIBd4WG5/kltnzdxSCqoP8CMGs/Li+M1uF5o7lOkZVFjDs+NLesthnF66Pg/0q0Lw==
   dependencies:
     array-buffer-byte-length "^1.0.0"
+    arraybuffer.prototype.slice "^1.0.1"
     available-typed-arrays "^1.0.5"
     call-bind "^1.0.2"
     es-set-tostringtag "^2.0.1"
     es-to-primitive "^1.2.1"
     function.prototype.name "^1.1.5"
     get-intrinsic "^1.2.1"
     get-symbol-description "^1.0.0"
@@ -3994,18 +4007,21 @@
     is-string "^1.0.7"
     is-typed-array "^1.1.10"
     is-weakref "^1.0.2"
     object-inspect "^1.12.3"
     object-keys "^1.1.1"
     object.assign "^4.1.4"
     regexp.prototype.flags "^1.5.0"
+    safe-array-concat "^1.0.0"
     safe-regex-test "^1.0.0"
     string.prototype.trim "^1.2.7"
     string.prototype.trimend "^1.0.6"
     string.prototype.trimstart "^1.0.6"
+    typed-array-buffer "^1.0.0"
+    typed-array-byte-length "^1.0.0"
     typed-array-byte-offset "^1.0.0"
     typed-array-length "^1.0.4"
     unbox-primitive "^1.0.2"
     which-typed-array "^1.1.10"
 
 es-get-iterator@^1.1.3:
   version "1.1.3"
@@ -5306,23 +5322,19 @@
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/is-symbol/-/is-symbol-1.0.4.tgz#a6dac93b635b063ca6872236de88910a57af139c"
   integrity sha512-C/CPBqKWnvdcxqIARxyOh4v1UUEOCHpgDa0WYgpKDFMszcrPcffg5uhwSgPCLD2WWxmq6isisz87tzT01tuGhg==
   dependencies:
     has-symbols "^1.0.2"
 
 is-typed-array@^1.1.10, is-typed-array@^1.1.9:
-  version "1.1.10"
-  resolved "https://registry.yarnpkg.com/is-typed-array/-/is-typed-array-1.1.10.tgz#36a5b5cb4189b575d1a3e4b08536bfb485801e3f"
-  integrity sha512-PJqgEHiWZvMpaFZ3uTc8kHPM4+4ADTlDniuQL7cU/UDA0Ql7F70yGfHph3cLNe+c9toaigv+DFzTJKhc2CtO6A==
+  version "1.1.12"
+  resolved "https://registry.yarnpkg.com/is-typed-array/-/is-typed-array-1.1.12.tgz#d0bab5686ef4a76f7a73097b95470ab199c57d4a"
+  integrity sha512-Z14TF2JNG8Lss5/HMqt0//T9JeHXttXy5pH/DBU4vi98ozO2btxzq9MwYDZYnKwU8nRsz/+GVFVRDq3DkVuSPg==
   dependencies:
-    available-typed-arrays "^1.0.5"
-    call-bind "^1.0.2"
-    for-each "^0.3.3"
-    gopd "^1.0.1"
-    has-tostringtag "^1.0.0"
+    which-typed-array "^1.1.11"
 
 is-typedarray@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/is-typedarray/-/is-typedarray-1.0.0.tgz#e479c80858df0c1b11ddda6940f96011fcda4a9a"
   integrity sha512-cyA56iCMHAh5CdzjJIa4aohJyeO1YbwLi3Jc35MmRU6poroFjIGZzUzupGiRPOjgHg9TLu43xbpwXk523fMxKA==
 
 is-weakmap@^2.0.1:
@@ -7797,14 +7809,24 @@
 run-parallel@^1.1.9:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/run-parallel/-/run-parallel-1.2.0.tgz#66d1368da7bdf921eb9d95bd1a9229e7f21a43ee"
   integrity sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==
   dependencies:
     queue-microtask "^1.2.2"
 
+safe-array-concat@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.yarnpkg.com/safe-array-concat/-/safe-array-concat-1.0.0.tgz#2064223cba3c08d2ee05148eedbc563cd6d84060"
+  integrity sha512-9dVEFruWIsnie89yym+xWTAYASdpw3CJV7Li/6zBewGf9z2i1j31rP6jnY0pHEO4QZh6N0K11bFjWmdR8UGdPQ==
+  dependencies:
+    call-bind "^1.0.2"
+    get-intrinsic "^1.2.0"
+    has-symbols "^1.0.3"
+    isarray "^2.0.5"
+
 safe-buffer@^5.1.0, safe-buffer@~5.2.0:
   version "5.2.1"
   resolved "https://registry.yarnpkg.com/safe-buffer/-/safe-buffer-5.2.1.tgz#1eaf9fa9bdb1fdd4ec75f58f9cdb4e6b7827eec6"
   integrity sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==
 
 safe-regex-test@^1.0.0:
   version "1.0.0"
@@ -8504,17 +8526,17 @@
     "@jridgewell/trace-mapping" "^0.3.17"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
     terser "^5.16.8"
 
 terser@^5.16.8, terser@^5.3.4:
-  version "5.19.0"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.19.0.tgz#7b3137b01226bdd179978207b9c8148754a6da9c"
-  integrity sha512-JpcpGOQLOXm2jsomozdMDpd5f8ZHh1rR48OFgWUH3QsyZcfPgv2qDCYbcDEAYNd4OZRj2bWYKpwdll/udZCk/Q==
+  version "5.19.1"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.19.1.tgz#dbd7231f224a9e2401d0f0959542ed74d76d340b"
+  integrity sha512-27hxBUVdV6GoNg1pKQ7Z5cbR6V9txPVyBA+FQw3BaZ1Wuzvztce5p156DaP0NVZNrMZZ+6iG9Syf7WgMNKDg2Q==
   dependencies:
     "@jridgewell/source-map" "^0.3.3"
     acorn "^8.8.2"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
 test-exclude@^6.0.0:
@@ -8702,14 +8724,33 @@
   integrity sha512-q+MB8nYR1KDLrgr4G5yemftpMC7/QLqVndBmEEdqzmNj5dcFOO4Oo8qlwZE3ULT3+Zim1F8Kq4cBnikNhlCMlg==
 
 type-fest@^0.8.1:
   version "0.8.1"
   resolved "https://registry.yarnpkg.com/type-fest/-/type-fest-0.8.1.tgz#09e249ebde851d3b1e48d27c105444667f17b83d"
   integrity sha512-4dbzIzqvjtgiM5rw1k5rEHtBANKmdudhGyBEajN01fEyhaAIhsoKNy6y7+IN93IfpFtwY9iqi7kD+xwKhQsNJA==
 
+typed-array-buffer@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.yarnpkg.com/typed-array-buffer/-/typed-array-buffer-1.0.0.tgz#18de3e7ed7974b0a729d3feecb94338d1472cd60"
+  integrity sha512-Y8KTSIglk9OZEr8zywiIHG/kmQ7KWyjseXs1CbSo8vC42w7hg2HgYTxSWwP0+is7bWDc1H+Fo026CpHFwm8tkw==
+  dependencies:
+    call-bind "^1.0.2"
+    get-intrinsic "^1.2.1"
+    is-typed-array "^1.1.10"
+
+typed-array-byte-length@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.yarnpkg.com/typed-array-byte-length/-/typed-array-byte-length-1.0.0.tgz#d787a24a995711611fb2b87a4052799517b230d0"
+  integrity sha512-Or/+kvLxNpeQ9DtSydonMxCx+9ZXOswtwJn17SNLvhptaXYDJvkFFP5zbfU/uLmvnBJlI4yrnXRxpdWH/M5tNA==
+  dependencies:
+    call-bind "^1.0.2"
+    for-each "^0.3.3"
+    has-proto "^1.0.1"
+    is-typed-array "^1.1.10"
+
 typed-array-byte-offset@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/typed-array-byte-offset/-/typed-array-byte-offset-1.0.0.tgz#cbbe89b51fdef9cd6aaf07ad4707340abbc4ea0b"
   integrity sha512-RD97prjEt9EL8YgAgpOkf3O4IF9lhJFr9g0htQkm0rchFp/Vx7LW5Q8fSXXub7BXAODyUQohRMyOc3faCPd0hg==
   dependencies:
     available-typed-arrays "^1.0.5"
     call-bind "^1.0.2"
@@ -9052,17 +9093,17 @@
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5.41.1:
-  version "5.88.1"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.88.1.tgz#21eba01e81bd5edff1968aea726e2fbfd557d3f8"
-  integrity sha512-FROX3TxQnC/ox4N+3xQoWZzvGXSuscxR32rbzjpXgEzWudJFEJBpdlkkob2ylrv5yzzufD1zph1OoFsLtm6stQ==
+  version "5.88.2"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.88.2.tgz#f62b4b842f1c6ff580f3fcb2ed4f0b579f4c210e"
+  integrity sha512-JmcgNZ1iKj+aiR0OvTYtWQqJwq37Pf683dY9bVORwVbUrDhLhdn/PlO2sHsFHPkj7sHNQF3JwaAkp49V+Sq1tQ==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
     "@types/estree" "^1.0.0"
     "@webassemblyjs/ast" "^1.11.5"
     "@webassemblyjs/wasm-edit" "^1.11.5"
     "@webassemblyjs/wasm-parser" "^1.11.5"
     acorn "^8.7.1"
@@ -9136,25 +9177,24 @@
     is-weakset "^2.0.1"
 
 which-module@^2.0.0:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/which-module/-/which-module-2.0.1.tgz#776b1fe35d90aebe99e8ac15eb24093389a4a409"
   integrity sha512-iBdZ57RDvnOR9AGBhML2vFZf7h8vmBjhoaZqODJBFWHVtKkDmKuHai3cx5PgVMrX5YDNp27AofYbAwctSS+vhQ==
 
-which-typed-array@^1.1.10, which-typed-array@^1.1.9:
-  version "1.1.10"
-  resolved "https://registry.yarnpkg.com/which-typed-array/-/which-typed-array-1.1.10.tgz#74baa2789991905c2076abb317103b866c64e69e"
-  integrity sha512-uxoA5vLUfRPdjCuJ1h5LlYdmTLbYfums398v3WLkM+i/Wltl2/XyZpQWKbN++ck5L64SR/grOHqtXCUKmlZPNA==
+which-typed-array@^1.1.10, which-typed-array@^1.1.11, which-typed-array@^1.1.9:
+  version "1.1.11"
+  resolved "https://registry.yarnpkg.com/which-typed-array/-/which-typed-array-1.1.11.tgz#99d691f23c72aab6768680805a271b69761ed61a"
+  integrity sha512-qe9UWWpkeG5yzZ0tNYxDmd7vo58HDBc39mZ0xWWpolAGADdFOzkfamWLDxkOWcvHQKVmdTyQdLD4NOfjLWTKew==
   dependencies:
     available-typed-arrays "^1.0.5"
     call-bind "^1.0.2"
     for-each "^0.3.3"
     gopd "^1.0.1"
     has-tostringtag "^1.0.0"
-    is-typed-array "^1.1.10"
 
 which@^1.2.9, which@^1.3.1:
   version "1.3.1"
   resolved "https://registry.yarnpkg.com/which/-/which-1.3.1.tgz#a45043d54f5805316da8d62f9f50918d3da70b0a"
   integrity sha512-HxJdYWq1MTIQbJ3nw0cqssHoTNU267KlrDuGZ1WYlxDStUtKUhOaJmh112/TZmHxxUfuJqPXSOm7tDyas0OSIQ==
   dependencies:
     isexe "^2.0.0"
@@ -9358,17 +9398,17 @@
     get-caller-file "^2.0.5"
     require-directory "^2.1.1"
     string-width "^4.2.0"
     y18n "^5.0.5"
     yargs-parser "^20.2.2"
 
 yjs@^13.5.17, yjs@^13.5.40:
-  version "13.6.6"
-  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.6.6.tgz#586b2dd25121a8cdb55ba85bb8760ec8904e037c"
-  integrity sha512-VTvezMeMuOra9jKG1Ym5XuQ2H4xXOubIIIupv/B5oygasa9IqDE7Ufv93QTSe9uz69J5VZGMQb2WTEmJv4kJFQ==
+  version "13.6.7"
+  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.6.7.tgz#f1176c37f65eb566cf390bd813e2099d598795f4"
+  integrity sha512-mCZTh4kjvUS2DnaktsYN6wLH3WZCJBLqrTdkWh1bIDpA/sB/GNFaLA/dyVJj2Hc7KwONuuoC/vWe9bwBBosZLQ==
   dependencies:
     lib0 "^0.2.74"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.936279136/schema/plugin.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993622448979592%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {delete: [3]}}}}"}*

```diff
@@ -12,17 +12,14 @@
                     {
                         "type": "separator"
                     },
                     {
                         "command": "jp-vdk:menu-create"
                     },
                     {
-                        "command": "jp-vdk:menu-delete"
-                    },
-                    {
                         "command": "jp-vdk:menu-download"
                     },
                     {
                         "command": "jp-vdk:menu-convert-job-to-notebook"
                     },
                     {
                         "command": "jp-vdk:menu-create-deployment"
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/commandsAndMenu.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,28 @@
 import { Dialog, showErrorMessage } from '@jupyterlab/apputils';
 import { showRunJobDialog } from './components/RunJob';
 import { jobData, setJobDataToDefault } from './jobData';
 import { showCreateDeploymentDialog } from './components/DeployJob';
 import { showCreateJobDialog } from './components/CreateJob';
 import { showDownloadJobDialog } from './components/DownloadJob';
 import { showConvertJobToNotebookDialog } from './components/ConvertJobToNotebook';
-import { showDeleteJobDialog } from './components/DeleteJob';
 import { jobdDataRequest } from './serverRequests';
 import { VdkOption } from './vdkOptions/vdk_options';
 import { workingDirectory } from '.';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 
 var runningVdkOperation = false;
 
 export function updateVDKMenu(commands: CommandRegistry, docManager: IDocumentManager) {
   // Add Run job command
   add_command(commands, 'jp-vdk:menu-run','Run','Execute VDK Run Command', showRunJobDialog, docManager);
 
   // Add Create job command
   add_command(commands, 'jp-vdk:menu-create','Create','Execute VDK Create Command', showCreateJobDialog);
 
-  // Add Delete job command
-  add_command(commands, 'jp-vdk:menu-delete','Delete','Execute VDK Delete Command', showDeleteJobDialog);
-
   // Add Download job command
   add_command(commands, 'jp-vdk:menu-download','Download','Execute VDK Download Command', showDownloadJobDialog);
 
   // Add Convert Job To Notebook command
   add_command(commands, 'jp-vdk:menu-convert-job-to-notebook', 'Convert Job To Notebook', 'Convert Data Job To Jupyter Notebook', showConvertJobToNotebookDialog);
 
   // Add Create Deployment command
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/handler.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/index.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/delete-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/download-job-component.spec.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,64 @@
 /*
  * Copyright 2023-2023 VMware, Inc.
  * SPDX-License-Identifier: Apache-2.0
  */
-import DeleteJobDialog from '../components/DeleteJob';
+import DownloadJobDialog from '../components/DownloadJob';
 import { render, fireEvent } from '@testing-library/react';
 import { jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
-import { IJobNameAndTeamProps } from '../components/props';
+import { IJobPathProp } from '../components/props';
 
-const defaultProps: IJobNameAndTeamProps = {
-  jobName: 'test-name',
-  jobTeam: 'test-team'
+const defaultProps: IJobPathProp = {
+  jobPath: 'test-path'
 };
 
 // created with the expectation to compare a rendered value with expected value parsed from config.ini
 // yet to be implemented
 describe('#render()', () => {
   it('should return contain job name input with placeholder equal to jobName from props', () => {
-    const component = render(new DeleteJobDialog(defaultProps).render());
-    const input = component.getByPlaceholderText(defaultProps.jobName);
+    const component = render(new DownloadJobDialog(defaultProps).render());
+    const input = component.getByPlaceholderText('default-name');
     expect(input).toBe(component.getAllByLabelText('Job Name:')[0]);
   });
 
   it('should return contain job team input with placeholder equal to jobTeam from props', () => {
-    const component = render(new DeleteJobDialog(defaultProps).render());
-    const input = component.getByPlaceholderText(defaultProps.jobTeam);
+    const component = render(new DownloadJobDialog(defaultProps).render());
+    const input = component.getByPlaceholderText('default-team');
     expect(input).toBe(component.getAllByLabelText('Job Team:')[0]);
   });
+
+  it('should return contain job path input with placeholder equal to jobPath from props', () => {
+    const component = render(new DownloadJobDialog(defaultProps).render());
+    const input = component.getByPlaceholderText(defaultProps.jobPath);
+    expect(input).toBe(
+      component.getAllByLabelText('Path to job directory:')[0]
+    );
+  });
 });
 
 describe('#onNameChange', () => {
   it('should change the job name in jobData', () => {
-    const component = render(new DeleteJobDialog(defaultProps).render());
-    const input = component.getByPlaceholderText(defaultProps.jobName);
+    const component = render(new DownloadJobDialog(defaultProps).render());
+    const input = component.getByPlaceholderText('default-name');
     fireEvent.change(input, { target: { value: 'second-name' } });
     expect(jobData.get(VdkOption.NAME)).toEqual('second-name');
   });
 });
 
 describe('#onTeamChange', () => {
   it('should change the job team in jobData', () => {
-    const component = render(new DeleteJobDialog(defaultProps).render());
-    const input = component.getByPlaceholderText(defaultProps.jobTeam);
+    const component = render(new DownloadJobDialog(defaultProps).render());
+    const input = component.getByPlaceholderText('default-team');
     fireEvent.change(input, { target: { value: 'second-team' } });
     expect(jobData.get(VdkOption.TEAM)).toEqual('second-team');
   });
 });
+
+describe('#onPathChange', () => {
+  it('should change the path in jobData', () => {
+    const component = render(new DownloadJobDialog(defaultProps).render());
+    const input = component.getByPlaceholderText(defaultProps.jobPath);
+    fireEvent.change(input, { target: { value: 'other/path' } });
+    expect(jobData.get(VdkOption.PATH)).toEqual('other/path');
+  });
+});
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/show-dialog.spec.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import DownloadJobDialog, {
   showDownloadJobDialog
 } from '../components/DownloadJob';
 import DeployJobDialog, {
   showCreateDeploymentDialog
 } from '../components/DeployJob';
 import CreateJobDialog, { showCreateJobDialog } from '../components/CreateJob';
-import DeleteJobDialog, { showDeleteJobDialog } from '../components/DeleteJob';
 import { VdkErrorMessage } from '../components/VdkErrorMessage';
 
 // Mock the showDialog function
 jest.mock('@jupyterlab/apputils', () => ({
   showDialog: jest.fn(),
   Dialog: {
     okButton: jest.fn(),
@@ -196,70 +195,7 @@
 
   it('should call jobRequest function with "create" argument when user accepts dialog', async () => {
     await showCreateJobDialog();
 
     expect(jobRequest).toHaveBeenCalledWith('create');
   });
 });
-
-describe('showDeleteJobDialog', () => {
-  jobData.set(VdkOption.PATH, 'my-job');
-  jobData.set(VdkOption.NAME, 'my-team');
-
-  afterEach(() => {
-    jest.clearAllMocks();
-  });
-
-  it('should delete the job when the user confirms', async () => {
-    const showDialogMock = showDialog as jest.MockedFunction<typeof showDialog>;
-    const jobRequestMock = jobRequest as jest.MockedFunction<typeof jobRequest>;
-    const acceptResult = { button: { accept: true } };
-    const confirmResult = { button: { accept: true } };
-
-    // Mock the first dialog
-    (showDialogMock as jest.Mock).mockResolvedValueOnce(acceptResult);
-
-    // Mock the second dialog
-    (showDialogMock as jest.Mock).mockResolvedValueOnce(confirmResult);
-
-    // Call the function
-    await showDeleteJobDialog();
-
-    // Check the results
-    expect(showDialogMock).toHaveBeenCalledWith({
-      title: 'Delete Job',
-      body: (
-        <DeleteJobDialog
-          jobName={jobData.get(VdkOption.NAME)!}
-          jobTeam={jobData.get(VdkOption.TEAM)!}
-        ></DeleteJobDialog>
-      ),
-      buttons: [Dialog.okButton(), Dialog.cancelButton()]
-    });
-    expect(jobRequestMock).toHaveBeenCalledWith('delete');
-  });
-
-  it('should not delete the job when the user does not confirm', async () => {
-    const showDialogMock = showDialog as jest.MockedFunction<typeof showDialog>;
-    const jobRequestMock = jobRequest as jest.MockedFunction<typeof jobRequest>;
-    const refuseResult = { button: { accept: false } };
-
-    // Mock the first dialog
-    (showDialogMock as jest.Mock).mockResolvedValueOnce(refuseResult);
-
-    // Call the function
-    await showDeleteJobDialog();
-
-    // Check the results
-    expect(showDialogMock).toHaveBeenCalledWith({
-      title: 'Delete Job',
-      body: (
-        <DeleteJobDialog
-          jobName={jobData.get(VdkOption.NAME)!}
-          jobTeam={jobData.get(VdkOption.TEAM)!}
-        ></DeleteJobDialog>
-      ),
-      buttons: [Dialog.okButton(), Dialog.cancelButton()]
-    });
-    expect(jobRequestMock).toHaveBeenCalledTimes(0);
-  });
-});
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/DeleteJob.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/components/DeployJob.tsx`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import React, { Component } from 'react';
+import { checkIfVdkOptionDataIsDefined, jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';
-import { jobData } from '../jobData';
-import { jobRequest } from '../serverRequests';
-import { IJobNameAndTeamProps } from './props';
-import { DELETE_JOB_BUTTON_LABEL } from '../utils';
+import { jobRequest, jobRunRequest } from '../serverRequests';
+import { IJobFullProps } from './props';
+import { CREATE_DEP_BUTTON_LABEL } from '../utils';
 
-export default class DeleteJobDialog extends Component<IJobNameAndTeamProps> {
+export default class DeployJobDialog extends Component<IJobFullProps> {
   /**
-   * Returns a React component for rendering a delete menu.
+   * Returns a React component for rendering a Deploy menu.
    *
    * @param props - component properties
    * @returns React component
    */
-  constructor(props: IJobNameAndTeamProps) {
+  constructor(props: IJobFullProps) {
     super(props);
   }
   /**
-   * Renders a dialog for deleting data job.
+   * Renders a dialog for creating a new deployment of a Data Job.
    *
    * @returns React element
    */
   render(): React.ReactElement {
     return (
       <>
         <VDKTextInput
@@ -31,48 +31,97 @@
           label="Job Name:"
         ></VDKTextInput>
         <VDKTextInput
           option={VdkOption.TEAM}
           value={this.props.jobTeam}
           label="Job Team:"
         ></VDKTextInput>
+        <VDKTextInput
+          option={VdkOption.PATH}
+          value={this.props.jobPath}
+          label="Path to job directory:"
+        ></VDKTextInput>
+        <VDKTextInput
+          option={VdkOption.DEPLOYMENT_REASON}
+          value="reason"
+          label="Deployment reason:"
+        ></VDKTextInput>
+        <div>
+          <input
+            type="checkbox"
+            name="enable"
+            id="enable"
+            className="jp-vdk-checkbox"
+            onClick={this.onEnableClick()}
+          />
+          <label className="checkboxLabel" htmlFor="enable">
+            Enable
+          </label>
+        </div>
       </>
     );
   }
+  /**
+   * Callback invoked upon choosing Enable checkbox
+   */
+  private onEnableClick() {
+    return (event: React.MouseEvent) => {
+      const checkbox = document.getElementById('enable');
+      if (checkbox?.classList.contains('checked')) {
+        checkbox.classList.remove('checked');
+        jobData.set(VdkOption.DEPLOY_ENABLE, '');
+      } else {
+        checkbox?.classList.add('checked');
+        jobData.set(VdkOption.DEPLOY_ENABLE, '1');
+      }
+    };
+  }
 }
 
-export async function showDeleteJobDialog() {
+export async function showCreateDeploymentDialog() {
   const result = await showDialog({
-    title: DELETE_JOB_BUTTON_LABEL,
+    title: CREATE_DEP_BUTTON_LABEL,
     body: (
-      <DeleteJobDialog
+      <DeployJobDialog
         jobName={jobData.get(VdkOption.NAME)!}
+        jobPath={jobData.get(VdkOption.PATH)!}
         jobTeam={jobData.get(VdkOption.TEAM)!}
-      ></DeleteJobDialog>
+      ></DeployJobDialog>
     ),
     buttons: [Dialog.okButton(), Dialog.cancelButton()]
   });
-  if (result.button.accept) {
+  const resultButtonClicked = !result.value && result.button.accept;
+  if (resultButtonClicked) {
     try {
-      const finalResult = await showDialog({
-        title: DELETE_JOB_BUTTON_LABEL,
-        body:
-          'Do you really want to delete the job with name ' +
-          jobData.get(VdkOption.NAME) +
-          '?',
+      const runConfirmationResult = await showDialog({
+        title: CREATE_DEP_BUTTON_LABEL,
+        body: 'The job will be executed once before deployment.',
         buttons: [
           Dialog.cancelButton({ label: 'Cancel' }),
-          Dialog.okButton({ label: 'Yes' })
+          Dialog.okButton({ label: 'Continue' })
         ]
       });
-      if (finalResult.button.accept) {
-        await jobRequest('delete');
+      if (runConfirmationResult.button.accept) {
+        const { message, status } = await jobRunRequest();
+        if (status) {
+          if (
+            await checkIfVdkOptionDataIsDefined(VdkOption.DEPLOYMENT_REASON)
+          ) {
+            await jobRequest('deploy');
+          }
+        } else {
+          showErrorMessage(
+            'Encоuntered an error while running the job!',
+            message,
+            [Dialog.okButton()]
+          );
+        }
       }
     } catch (error) {
       await showErrorMessage(
-        'Encountered an error when deleting the job. Error:',
+        'Encountered an error when deploying the job. Error:',
         error,
         [Dialog.okButton()]
       );
     }
   }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.936279136/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.936279136/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/style/base.css` & `vdk_jupyterlab_extension-0.1.936279136/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.936279136/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.936279136/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.936279136/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.936279136/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.936279136/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files 16% similar despite different names*

```diff
@@ -91,59 +91,14 @@
   await page.getByRole('button', { name: 'OK' }).click();
   await page
     .locator('div')
     .filter({ hasText: 'Encountered an error when creating the job.' });
   await page.getByRole('button', { name: 'OK' }).click();
 });
 
-test('should open delete job pop up and then cancel the operation', async ({
-  page
-}) => {
-  await page.goto('');
-  await page.menu.open('VDK');
-  await page.locator('#jp-vdk-menu').getByText('Delete').click();
-  await page.locator('div').filter({ hasText: 'Delete Job' });
-  await page.getByRole('button', { name: 'Cancel' }).click();
-});
-
-test('should open delete job confirmation pop up', async ({ page }) => {
-  await page.goto('');
-  await page.menu.open('VDK');
-  await page.locator('#jp-vdk-menu').getByText('Delete').click();
-  await page.locator('div').filter({ hasText: 'Delete Job' });
-  await page.getByRole('button', { name: 'OK' }).click();
-  // this is tested with empty input that's why the message is with null
-  await page.locator('div').filter({
-    hasText: 'Do you really want to delete the job with name null from null?'
-  });
-  await page.getByRole('button', { name: 'Cancel' }).click();
-});
-
-test('should try to delete a job with empty input and get error', async ({
-  page
-}) => {
-  await page.goto('');
-  await page.menu.open('VDK');
-  await page.locator('#jp-vdk-menu').getByText('Delete').click();
-  await page.locator('div').filter({ hasText: 'Delete Job' });
-  await page.getByRole('button', { name: 'OK' }).click();
-  // this is tested with empty input that's why the message is with null
-  await page
-    .locator('div')
-    .filter({
-      hasText: 'Do you really want to delete the job with name null from null?'
-    })
-    .first()
-    .click();
-  await page.getByRole('button', { name: 'Yes' }).click();
-  await page
-    .locator('div')
-    .filter({ hasText: 'Encountered an error when deleting the job.' });
-});
-
 test('should open download job pop up and then cancel the operation', async ({
   page
 }) => {
   await page.goto('');
   await page.menu.open('VDK');
   await page.locator('#jp-vdk-menu').getByText('Download').click();
   await page.locator('div').filter({ hasText: 'Download Job' });
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,34 +64,14 @@
         run_result = VdkUI.run_job(
             input_data[VdkOption.PATH.value],
             input_data[VdkOption.ARGUMENTS.value],
         )
         self.finish(json.dumps(run_result))
 
 
-class DeleteJobHandler(APIHandler):
-    """
-    Class responsible for handling POST request for deleting a Data Job given its name, team and Rest API URL
-    Response: return a json formatted str including:
-        ::error field with error message if an error exists
-        ::message field with status of the Vdk operation
-    """
-
-    @tornado.web.authenticated
-    def post(self):
-        input_data = self.get_json_body()
-        try:
-            status = VdkUI.delete_job(
-                input_data[VdkOption.NAME.value], input_data[VdkOption.TEAM.value]
-            )
-            self.finish(json.dumps({"message": f"{status}", "error": ""}))
-        except Exception as e:
-            self.finish(json.dumps({"message": f"{e}", "error": "true"}))
-
-
 class DownloadJobHandler(APIHandler):
     """
     Class responsible for handling POST request for downloading a Data Job given its name, team,
     Rest API URL, and the path to where the job will be downloaded
     Response: return a json formatted str including:
         ::error field with error message if an error exists
         ::message field with status of the Vdk operation
@@ -200,15 +180,14 @@
         job_route_pattern = url_path_join(
             base_url, "vdk-jupyterlab-extension", endpoint
         )
         job_handlers = [(job_route_pattern, handler)]
         web_app.add_handlers(host_pattern, job_handlers)
 
     add_handler(RunJobHandler, "run")
-    add_handler(DeleteJobHandler, "delete")
     add_handler(DownloadJobHandler, "download")
     add_handler(ConvertJobToNotebookHandler, "convertJobToNotebook")
     add_handler(CreateJobHandler, "create")
     add_handler(LoadJobDataHandler, "job")
     add_handler(CreateDeploymentHandler, "deploy")
     add_handler(GetNotebookInfoHandler, "notebook")
     add_handler(GetVdkCellIndicesHandler, "vdkCellIndices")
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import pathlib
 import shlex
 import subprocess
 from pathlib import Path
 
 from vdk.internal.control.command_groups.job.create import JobCreate
-from vdk.internal.control.command_groups.job.delete import JobDelete
 from vdk.internal.control.command_groups.job.deploy_cli_impl import JobDeploy
 from vdk.internal.control.command_groups.job.download_job import JobDownloadSource
 from vdk.internal.control.utils import cli_utils
 
 
 class RestApiUrlConfiguration:
     @staticmethod
@@ -86,26 +85,14 @@
                         # the json is generated in vdk-notebook plugin
                         # you can see /vdk-notebook/src/vdk/notebook-plugin.py
                         error = json.load(file)
                         return {"message": error["details"]}
             return {"message": process.returncode}
 
     @staticmethod
-    def delete_job(name: str, team: str):
-        """
-        Execute `delete job`.
-        :param name: the name of the data job that will be deleted
-        :param team: the team of the data job that will be deleted
-        :return: message that the job is deleted
-        """
-        cmd = JobDelete(RestApiUrlConfiguration.get_rest_api_url())
-        cmd.delete_job(name, team)
-        return f"Deleted the job with name {name} from {team} team. "
-
-    @staticmethod
     def download_job(name: str, team: str, path: str):
         """
         Execute `download job`.
         :param name: the name of the data job that will be downloaded
         :param team: the team of the data job that will be downloaded
         :param path: the path to the directory where the job will be downloaded
         :return: message that the job is downloaded
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.77b468e1169ec9f71a16.js'}}",*

 * * "'version'": "'0.1.936279136'"}*

```diff
@@ -77,15 +77,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b6f98de260318ecd5e13.js",
+            "load": "static/remoteEntry.77b468e1169ec9f71a16.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -150,9 +150,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.931147919"
+    "version": "0.1.936279136"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.936279136'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.931147919"
+    "version": "0.1.936279136"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993622448979592%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {delete: [3]}}}}"}*

```diff
@@ -12,17 +12,14 @@
                     {
                         "type": "separator"
                     },
                     {
                         "command": "jp-vdk:menu-create"
                     },
                     {
-                        "command": "jp-vdk:menu-delete"
-                    },
-                    {
                         "command": "jp-vdk:menu-download"
                     },
                     {
                         "command": "jp-vdk:menu-convert-job-to-notebook"
                     },
                     {
                         "command": "jp-vdk:menu-create-deployment"
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/381.0485c5d1f906c39de85e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 "use strict";
 (self.webpackChunkvdk_jupyterlab_extension = self.webpackChunkvdk_jupyterlab_extension || []).push([
-    [800], {
-        800: (e, t, a) => {
+    [381], {
+        381: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Q,
-                workingDirectory: () => G
+                default: () => q,
+                workingDirectory: () => V
             });
             var n, o = a(38),
                 l = a(33),
                 s = a(271),
                 r = a.n(s);
             ! function(e) {
                 e.NAME = "jobName", e.TEAM = "jobTeam", e.PATH = "jobPath", e.CLOUD = "cloud", e.LOCAL = "local", e.ARGUMENTS = "jobArguments", e.DEPLOYMENT_REASON = "deploymentReason", e.DEPLOY_ENABLE = "enableDeploy"
@@ -27,19 +27,19 @@
                     cloud: c.get(n.CLOUD),
                     local: c.get(n.LOCAL),
                     jobArguments: c.get(n.ARGUMENTS),
                     deploymentReason: c.get(n.DEPLOYMENT_REASON),
                     enableDeploy: c.get(n.DEPLOY_ENABLE)
                 }
             }
-            async function m(e) {
+            async function d(e) {
                 return !!c.get(e) || (await (0, l.showErrorMessage)("Encountered an error while trying to execute operation. Error:", "The " + e + " should be defined!", [l.Dialog.okButton()]), !1)
             }
             i();
-            const d = e => {
+            const m = e => {
                 const t = e.split(/(?=[/\\])/);
                 return t[t.length - 1]
             };
             class p extends s.Component {
                 constructor(e) {
                     super(e), this.onInputChange = e => {
                         let t = e.currentTarget.value;
@@ -52,15 +52,15 @@
                     }, r().createElement("label", {
                         className: "jp-vdk-label",
                         htmlFor: this.props.option
                     }, this.props.label), r().createElement("input", {
                         type: "text",
                         id: this.props.option,
                         className: "jp-vdk-input",
-                        placeholder: d(this.props.value),
+                        placeholder: m(this.props.value),
                         onChange: this.onInputChange
                     })))
                 }
             }
             var h = a(142),
                 g = a(820);
             async function b(e = "", t = {}) {
@@ -81,15 +81,15 @@
                 if (!o.ok) throw new Error(o.statusText);
                 return l
             }
             const E = async e => {
                 await (0, l.showErrorMessage)("Encountered an error while trying to connect the server. Error:", e, [l.Dialog.okButton()])
             };
             async function v() {
-                if (!await m(n.PATH)) return {
+                if (!await d(n.PATH)) return {
                     message: "",
                     status: !1
                 };
                 try {
                     const e = await b("run", {
                         body: JSON.stringify(u()),
                         method: "POST"
@@ -101,26 +101,26 @@
                 } catch (e) {
                     return E(e), {
                         message: "",
                         status: !1
                     }
                 }
             }
-            async function y(e) {
-                if (await m(n.NAME) && await m(n.TEAM)) try {
+            async function k(e) {
+                if (await d(n.NAME) && await d(n.TEAM)) try {
                     const t = await b(e, {
                         body: JSON.stringify(u()),
                         method: "POST"
                     });
                     t.error ? await (0, l.showErrorMessage)("Encountered an error while trying the " + e + " operation. Error:", t.message, [l.Dialog.okButton()]) : alert(t.message)
                 } catch (e) {
                     E(e)
                 }
             }
-            class k {
+            class y {
                 constructor(e) {
                     this.exception_message = "", this.what_happened = "", this.why_it_happened = "", this.consequences = "", this.countermeasures = "", this.__parse_message(e)
                 }
                 __parse_message(e) {
                     const t = ["exception_message", "what_happened", "why_it_happened", "consequences", "countermeasures"],
                         a = ["ERROR : ", "WHAT HAPPENED :", "WHY IT HAPPENED :", "CONSEQUENCES :", "COUNTERMEASURES :"],
                         n = e.split("\n");
@@ -131,17 +131,16 @@
                             if (this[t[o]] = a[o] + n[l].substring(s + a[o].length), o++, o === t.length) break
                         } else this.exception_message = e
                     }
                 }
             }
             const w = "Convert Job To Notebook",
                 f = "Run Job",
-                N = "Create Deployment",
-                j = "Delete Job";
-            class D extends s.Component {
+                N = "Create Deployment";
+            class j extends s.Component {
                 constructor(e) {
                     super(e), this._onArgsChange = e => {
                         let t = e.currentTarget.value;
                         t && this._isJSON(t) && c.set(n.ARGUMENTS, t)
                     }, this._isJSON = e => {
                         try {
                             return JSON.parse(e), !0
@@ -168,18 +167,18 @@
                         onChange: this._onArgsChange
                     })), r().createElement("ul", {
                         id: "argumentsUl",
                         className: "hidden"
                     }))
                 }
             }
-            async function A(e) {
+            async function C(e) {
                 if ((await (0, l.showDialog)({
                         title: f,
-                        body: r().createElement(D, {
+                        body: r().createElement(j, {
                             jobPath: c.get(n.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
                     let {
                         message: t,
                         status: a
@@ -191,61 +190,61 @@
                         }, r().createElement("p", {
                             className: "vdk-run-dialog-message"
                         }, "The job was executed successfully!")),
                         buttons: [l.Dialog.okButton()]
                     });
                     else {
                         t = "ERROR : " + t;
-                        const a = new k(t);
-                        e && await L(a, e) || (0, l.showDialog)({
+                        const a = new y(t);
+                        e && await P(a, e) || (0, l.showDialog)({
                             title: f,
                             body: r().createElement("div", {
                                 className: "vdk-run-error-message "
                             }, r().createElement("p", null, a.exception_message), r().createElement("p", null, a.what_happened), r().createElement("p", null, a.why_it_happened), r().createElement("p", null, a.consequences), r().createElement("p", null, a.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
                     }
                 }
             }
-            const C = e => {
+            const A = e => {
                     const t = e.getElementsByClassName("jp-Cell-inputWrapper");
                     for (let e = 0; e < t.length; e++) {
                         const a = t[e].getElementsByClassName("jp-Cell-inputArea");
                         if (a.length > 0) {
                             const e = a[0].getElementsByClassName("jp-InputArea-prompt");
                             if (e.length > 0) return e[0]
                         }
                     }
                 },
-                T = e => {
-                    const t = C(e);
+                D = e => {
+                    const t = A(e);
                     null == t || t.classList.add("jp-vdk-failing-cell-prompt"), e.scrollIntoView(), e.classList.add("jp-vdk-failing-cell"), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
                         e.classList.remove("jp-vdk-failing-cell-num"), e.classList.add("jp-vdk-cell-num")
                     }))
                 },
-                P = e => {
+                T = e => {
                     e.classList.remove("jp-vdk-failing-cell");
-                    const t = C(e);
+                    const t = A(e);
                     null == t || t.classList.remove("jp-vdk-failing-cell-prompt")
                 },
-                L = async (e, t) => {
+                P = async (e, t) => {
                     const a = (e => {
                         const t = e.match(/cell_id:([0-9a-fA-F-]+)/);
                         return t ? t[1] : ""
                     })(e.what_happened);
                     if (a) {
                         const {
                             path: o,
                             cellIndex: s
                         } = await async function(e) {
                             const t = {
                                 cellId: e,
                                 jobPath: c.get(n.PATH)
                             };
-                            if (!await m(n.PATH)) return {
+                            if (!await d(n.PATH)) return {
                                 path: "",
                                 cellIndex: ""
                             };
                             try {
                                 const e = await b("notebook", {
                                     body: JSON.stringify(t),
                                     method: "POST"
@@ -272,15 +271,15 @@
                                             const n = e.children;
                                             if (t > n.length)(0, l.showDialog)({
                                                 title: "Run Failed",
                                                 body: r().createElement("div", null, r().createElement("p", null, "Sorry, something went wrong while trying to find the failing cell!"), r().createElement("p", null, "Please, check the ", a, " once more and try to run the job while the notebook is active!")),
                                                 buttons: [l.Dialog.cancelButton()]
                                             });
                                             else
-                                                for (let e = 0; e < n.length; e++) e === t ? T(n[e]) : P(n[e])
+                                                for (let e = 0; e < n.length; e++) e === t ? D(n[e]) : T(n[e])
                                         })(e, Number(s), o)
                                     }))
                                 }
                             };
                             return (await (0, l.showDialog)({
                                 title: f,
                                 body: r().createElement("div", {
@@ -290,15 +289,15 @@
                                     label: "See failing cell"
                                 }), l.Dialog.cancelButton()]
                             })).button.accept && a(), !0
                         }
                     }
                     return !1
                 };
-            class _ extends s.Component {
+            class L extends s.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return r().createElement(r().Fragment, null, r().createElement(p, {
                         option: n.NAME,
                         value: this.props.jobName,
@@ -329,18 +328,18 @@
                 onEnableClick() {
                     return e => {
                         const t = document.getElementById("enable");
                         (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), c.set(n.DEPLOY_ENABLE, "")) : (null == t || t.classList.add("checked"), c.set(n.DEPLOY_ENABLE, "1"))
                     }
                 }
             }
-            async function x() {
+            async function _() {
                 const e = await (0, l.showDialog)({
                     title: N,
-                    body: r().createElement(_, {
+                    body: r().createElement(L, {
                         jobName: c.get(n.NAME),
                         jobPath: c.get(n.PATH),
                         jobTeam: c.get(n.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                 });
                 if (!e.value && e.button.accept) try {
@@ -353,21 +352,21 @@
                                 label: "Continue"
                             })]
                         })).button.accept) {
                         const {
                             message: e,
                             status: t
                         } = await v();
-                        t ? await m(n.DEPLOYMENT_REASON) && await y("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
+                        t ? await d(n.DEPLOYMENT_REASON) && await k("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
                     }
                 } catch (e) {
                     await (0, l.showErrorMessage)("Encountered an error when deploying the job. Error:", e, [l.Dialog.okButton()])
                 }
             }
-            class B extends s.Component {
+            class x extends s.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return r().createElement(r().Fragment, null, r().createElement("div", {
                         className: "jp-vdk-checkbox-wrappers"
                     }, r().createElement("div", null, r().createElement("input", {
@@ -416,23 +415,23 @@
                     let t = document.getElementById(e);
                     (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), "Cloud" === e ? c.set(n.CLOUD, "") : c.set(n.LOCAL, "")) : (null == t || t.classList.add("checked"), "Cloud" === e ? c.set(n.CLOUD, "1") : c.set(n.LOCAL, "1"))
                 }
             }
             async function O() {
                 (await (0, l.showDialog)({
                     title: "Create Job",
-                    body: r().createElement(B, {
+                    body: r().createElement(x, {
                         jobPath: c.get(n.PATH),
                         jobName: c.get(n.NAME),
                         jobTeam: c.get(n.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await y("create")
+                })).button.accept && await k("create")
             }
-            class M extends s.Component {
+            class B extends s.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return r().createElement(r().Fragment, null, r().createElement(p, {
                         option: n.NAME,
                         value: "default-name",
@@ -444,52 +443,52 @@
                     }), r().createElement(p, {
                         option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function S() {
+            async function M() {
                 (await (0, l.showDialog)({
                     title: "Download Job",
-                    body: r().createElement(M, {
+                    body: r().createElement(B, {
                         jobPath: c.get(n.PATH)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await y("download")
+                })).button.accept && await k("download")
             }
-            class J extends s.Component {
+            class S extends s.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return r().createElement(r().Fragment, null, r().createElement(p, {
                         option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function R() {
+            async function J() {
                 if ((await (0, l.showDialog)({
                         title: w,
-                        body: r().createElement(J, {
+                        body: r().createElement(S, {
                             jobPath: c.get(n.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept && (await (0, l.showDialog)({
                         title: w,
                         body: r().createElement("p", null, "Are you sure you want to convert the Data Job with path:", " ", r().createElement("i", null, c.get(n.PATH)), " to notebook?"),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
                     let {
                         message: e,
                         status: t
                     } = await async function() {
-                        if (!await m(n.PATH)) return {
+                        if (!await d(n.PATH)) return {
                             message: "",
                             status: !1
                         };
                         try {
                             const e = await b("convertJobToNotebook", {
                                 body: JSON.stringify(u()),
                                 method: "POST"
@@ -512,111 +511,73 @@
                         }, r().createElement("p", {
                             className: "vdk-convert-to-notebook-dialog-message"
                         }, "The Data Job with path ", r().createElement("i", null, c.get(n.PATH)), " was converted to notebook successfully!")),
                         buttons: [l.Dialog.okButton()]
                     });
                     else {
                         e = "ERROR : " + e;
-                        const t = new k(e);
+                        const t = new y(e);
                         await (0, l.showDialog)({
                             title: w,
                             body: r().createElement("div", {
                                 className: "vdk-convert-to-notebook-error-message "
                             }, r().createElement("p", null, t.exception_message), r().createElement("p", null, t.what_happened), r().createElement("p", null, t.why_it_happened), r().createElement("p", null, t.consequences), r().createElement("p", null, t.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
                     }
                 }
             }
-            class H extends s.Component {
-                constructor(e) {
-                    super(e)
-                }
-                render() {
-                    return r().createElement(r().Fragment, null, r().createElement(p, {
-                        option: n.NAME,
-                        value: this.props.jobName,
-                        label: "Job Name:"
-                    }), r().createElement(p, {
-                        option: n.TEAM,
-                        value: this.props.jobTeam,
-                        label: "Job Team:"
-                    }))
-                }
-            }
-            async function F() {
-                if ((await (0, l.showDialog)({
-                        title: j,
-                        body: r().createElement(H, {
-                            jobName: c.get(n.NAME),
-                            jobTeam: c.get(n.TEAM)
-                        }),
-                        buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                    })).button.accept) try {
-                    (await (0, l.showDialog)({
-                        title: j,
-                        body: "Do you really want to delete the job with name " + c.get(n.NAME) + "?",
-                        buttons: [l.Dialog.cancelButton({
-                            label: "Cancel"
-                        }), l.Dialog.okButton({
-                            label: "Yes"
-                        })]
-                    })).button.accept && await y("delete")
-                } catch (e) {
-                    await (0, l.showErrorMessage)("Encountered an error when deleting the job. Error:", e, [l.Dialog.okButton()])
-                }
-            }
-            var I = !1;
+            var R = !1;
 
-            function U(e, t, a, o, s, r) {
+            function H(e, t, a, o, s, r) {
                 e.addCommand(t, {
                     label: a,
                     caption: o,
                     execute: async () => {
                         try {
-                            I ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (I = !0, c.set(n.PATH, G), await async function() {
+                            R ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (R = !0, c.set(n.PATH, V), await async function() {
                                 try {
                                     const e = await b("job", {
                                         body: JSON.stringify(JSON.stringify(u())),
                                         method: "POST"
                                     });
                                     e && (c.set(n.NAME, e[n.NAME]), c.set(n.TEAM, e[n.TEAM]), c.set(n.PATH, e[n.PATH]))
                                 } catch (e) {
                                     E(e)
                                 }
-                            }(), r ? await s(r) : await s(), i(), I = !1)
+                            }(), r ? await s(r) : await s(), i(), R = !1)
                         } catch (e) {
                             await (0, l.showErrorMessage)("Encountered an error when trying to open the dialog. Error:", e, [l.Dialog.okButton()])
                         }
                     }
                 })
             }
-            var W = a(280),
-                Y = a(123);
-            const V = (e, t) => {
+            var I = a(280),
+                F = a(123);
+            const U = (e, t) => {
                     const a = document.createElement("div");
                     a.innerText = String(e), t.classList.contains("jp-vdk-failing-cell") ? a.classList.add("jp-vdk-failing-cell-num") : a.classList.add("jp-vdk-cell-num"), t.appendChild(a)
                 },
-                q = e => {
+                W = e => {
                     const t = document.createElement("img");
                     t.setAttribute("src", "https://raw.githubusercontent.com/vmware/versatile-data-kit/dc15f7489f763a0e0e29370b2e06a714448fc234/support/images/versatile-data-kit-logo.svg"), t.setAttribute("width", "20"), t.setAttribute("height", "20"), t.classList.add("jp-vdk-logo"), e.appendChild(t)
                 };
-            var K = a(986);
-            let G = "";
-            const Q = {
+            var Y = a(986);
+            let V = "";
+            const q = {
                     id: "vdk-jupyterlab-extension:plugin",
                     autoStart: !0,
-                    optional: [o.ISettingRegistry, W.IFileBrowserFactory, Y.INotebookTracker, l.IThemeManager, K.IDocumentManager],
+                    optional: [o.ISettingRegistry, I.IFileBrowserFactory, F.INotebookTracker, l.IThemeManager, Y.IDocumentManager],
                     activate: async (e, t, a, n, o, l) => {
                         const {
                             commands: s
                         } = e;
                         ! function(e, t) {
-                            U(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", A, t), U(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", O), U(e, "jp-vdk:menu-delete", "Delete", "Execute VDK Delete Command", F), U(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", S), U(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", R), U(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", x)
-                        }(s, l), a.defaultBrowser.model.pathChanged.connect(z), ((e, t) => {
+                            H(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", C, t), H(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", O), H(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", M), H(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", J), H(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", _)
+                        }(s, l), a.defaultBrowser.model.pathChanged.connect(K), ((e, t) => {
                             const a = async () => {
                                 if (e.currentWidget && e.currentWidget.model && 0 !== e.currentWidget.model.cells.length) {
                                     let a = [],
                                         n = 0;
                                     for (; e.currentWidget && e.currentWidget.model && e.currentWidget.model.cells.get(n);) {
                                         const t = e.currentWidget.model.cells.get(n).metadata.get("tags");
                                         t && t.includes("vdk") && a.push(n), n++
@@ -639,21 +600,21 @@
                                             e.remove()
                                         })), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
                                             e.remove()
                                         })), Array.from(document.getElementsByClassName("jp-vdk-logo")).forEach((e => {
                                             e.remove()
                                         }));
                                         let o = 0;
-                                        for (let l = 0; l < e.length; l++) t.includes(l) ? (a.theme && a.isLight(a.theme.toString()) ? (e[l].classList.remove("jp-vdk-cell-dark"), e[l].classList.add("jp-vdk-cell")) : (e[l].classList.add("jp-vdk-cell"), e[l].classList.add("jp-vdk-cell-dark")), n && e[l] != n && q(e[l]), V(++o, e[l])) : (e[l].classList.remove("jp-vdk-cell"), e[l].classList.remove("jp-vdk-cell-dark"))
+                                        for (let l = 0; l < e.length; l++) t.includes(l) ? (a.theme && a.isLight(a.theme.toString()) ? (e[l].classList.remove("jp-vdk-cell-dark"), e[l].classList.add("jp-vdk-cell")) : (e[l].classList.add("jp-vdk-cell"), e[l].classList.add("jp-vdk-cell-dark")), n && e[l] != n && W(e[l]), U(++o, e[l])) : (e[l].classList.remove("jp-vdk-cell"), e[l].classList.remove("jp-vdk-cell-dark"))
                                     })(Array.from(e.activeCell.parent.node.children), a, t, e.activeCell.node)
                                 }
                             };
                             e.activeCellChanged.connect(a), t.themeChanged.connect(a)
                         })(n, o)
                     }
                 },
-                z = async (e, t) => {
-                    G = t.newValue
+                K = async (e, t) => {
+                    V = t.newValue
                 }
         }
     }
 ]);
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/remoteEntry.b6f98de260318ecd5e13.js` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/remoteEntry.77b468e1169ec9f71a16.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b = {
             913: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(800).then((() => () => t(800))),
-                        "./extension": () => t.e(800).then((() => () => t(800))),
+                        "./index": () => t.e(381).then((() => () => t(381))),
+                        "./extension": () => t.e(381).then((() => () => t(381))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,35 +43,35 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        747: "e678254df7945f8ed34d",
-        800: "8ed62c07893a05a3a69b"
+        381: "0485c5d1f906c39de85e",
+        747: "e678254df7945f8ed34d"
     } [e] + ".js?v=" + {
-        747: "e678254df7945f8ed34d",
-        800: "8ed62c07893a05a3a69b"
+        381: "0485c5d1f906c39de85e",
+        747: "e678254df7945f8ed34d"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "vdk-jupyterlab-extension:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
@@ -102,19 +102,19 @@
                 var a = y.S[t],
                     i = "vdk-jupyterlab-extension",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => y.e(800).then((() => () => y(800))),
+                        get: () => y.e(381).then((() => () => y(381))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.931147919"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.936279136"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,31 +164,31 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == s) {
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
                     if (!l || "u" != d) return !1
                 } else if (l)
-                    if (d == s)
+                    if (d == f)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
@@ -199,33 +199,33 @@
     }, i = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || s(l(e, t, o, n)), d(e[t][o])
-    }, s = e => {
+        return a(n, o) || f(l(e, t, o, n)), d(e[t][o])
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = y.I(r);
         return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
         271: () => p("default", "react", [1, 17, 0, 1]),
         280: () => p("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
         820: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         986: () => p("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
     }, v = {
-        800: [33, 38, 123, 142, 271, 280, 820, 986]
+        381: [33, 38, 123, 142, 271, 280, 820, 986]
     }, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
                     }
```

### Comparing `vdk_jupyterlab_extension-0.1.931147919/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/.gitignore` & `vdk_jupyterlab_extension-0.1.936279136/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/README.md` & `vdk_jupyterlab_extension-0.1.936279136/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/pyproject.toml` & `vdk_jupyterlab_extension-0.1.936279136/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.931147919/PKG-INFO` & `vdk_jupyterlab_extension-0.1.936279136/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.931147919
+Version: 0.1.936279136
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

