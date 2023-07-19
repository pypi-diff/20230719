# Comparing `tmp/reflex-0.2.1a1.tar.gz` & `tmp/reflex-0.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.1a1.tar", max compression
+gzip compressed data, was "reflex-0.2.1a2.tar", max compression
```

## Comparing `reflex-0.2.1a1.tar` & `reflex-0.2.1a2.tar`

### file list

```diff
@@ -1,177 +1,178 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.1a1/LICENSE
--rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.1a1/README.md
--rw-r--r--   0        0        0     2002 2023-07-17 23:59:03.104219 reflex-0.2.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.1a1/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-17 03:56:35.638995 reflex-0.2.1a1/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.1a1/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.1a1/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.1a1/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.1a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.1a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.1a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.1a1/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-14 23:13:37.771555 reflex-0.2.1a1/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.1a1/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.1a1/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1179 2023-07-14 23:13:37.771733 reflex-0.2.1a1/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.1a1/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.1a1/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.1a1/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.1a1/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.1a1/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     9692 2023-07-14 23:13:37.772301 reflex-0.2.1a1/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1917 2023-07-17 23:54:14.126636 reflex-0.2.1a1/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.1a1/reflex/admin.py
--rw-r--r--   0        0        0    23303 2023-07-17 23:29:33.626521 reflex-0.2.1a1/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.1a1/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.1a1/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.1a1/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.1a1/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8527 2023-07-17 23:54:14.127035 reflex-0.2.1a1/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7601 2023-07-17 23:54:14.127174 reflex-0.2.1a1/reflex/components/__init__.py
--rw-r--r--   0        0        0      229 2023-07-17 23:54:14.127269 reflex-0.2.1a1/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.1a1/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.1a1/reflex/components/base/body.py
--rw-r--r--   0        0        0      721 2023-07-17 23:54:14.127363 reflex-0.2.1a1/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.1a1/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.1a1/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.1a1/reflex/components/base/meta.py
--rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.1a1/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.1a1/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.1a1/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.1a1/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.1a1/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.1a1/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.1a1/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.1a1/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.1a1/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5785 2023-07-14 23:13:37.774148 reflex-0.2.1a1/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.1a1/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.1a1/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.1a1/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.1a1/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.1a1/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.1a1/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.1a1/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1565 2023-07-14 23:13:37.774654 reflex-0.2.1a1/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.1a1/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.1a1/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.1a1/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.1a1/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.1a1/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.1a1/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.1a1/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.1a1/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.1a1/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.1a1/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.1a1/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.1a1/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.1a1/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.1a1/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.1a1/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.1a1/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.1a1/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.1a1/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.1a1/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.1a1/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.1a1/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.1a1/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.1a1/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.1a1/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.1a1/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.1a1/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.1a1/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.1a1/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.1a1/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.1a1/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.1a1/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.1a1/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.1a1/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.1a1/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.1a1/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.1a1/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.1a1/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.1a1/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.1a1/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.1a1/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.1a1/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.1a1/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.1a1/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.1a1/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.1a1/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.1a1/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.1a1/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.1a1/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.1a1/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.1a1/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.1a1/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.1a1/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.1a1/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.1a1/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.1a1/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.1a1/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.1a1/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.1a1/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.1a1/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.1a1/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.1a1/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.1a1/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.1a1/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.1a1/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.1a1/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.1a1/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.1a1/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.1a1/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.1a1/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.1a1/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.1a1/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.1a1/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2294 2023-07-14 23:13:37.779060 reflex-0.2.1a1/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.1a1/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.1a1/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.1a1/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.1a1/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.1a1/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.1a1/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.1a1/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.1a1/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7215 2023-07-14 23:13:37.779630 reflex-0.2.1a1/reflex/config.py
--rw-r--r--   0        0        0    10821 2023-07-17 23:29:33.627808 reflex-0.2.1a1/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.1a1/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.1a1/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.1a1/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.1a1/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.1a1/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.1a1/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.1a1/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.1a1/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.1a1/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.1a1/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.1a1/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.1a1/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     8611 2023-07-17 23:29:30.479899 reflex-0.2.1a1/reflex/model.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.1a1/reflex/py.typed
--rw-r--r--   0        0        0     9136 2023-07-17 23:29:33.627991 reflex-0.2.1a1/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.1a1/reflex/route.py
--rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.1a1/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.1a1/reflex/style.py
--rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.1a1/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.1a1/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7585 2023-07-17 23:29:30.480212 reflex-0.2.1a1/reflex/utils/build.py
--rw-r--r--   0        0        0     1759 2023-07-14 23:13:37.781884 reflex-0.2.1a1/reflex/utils/console.py
--rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.1a1/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.1a1/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.1a1/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.1a1/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    12672 2023-07-17 23:29:30.480515 reflex-0.2.1a1/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.1a1/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.1a1/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.1a1/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.1a1/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-14 23:13:37.782718 reflex-0.2.1a1/reflex/vars.py
--rw-r--r--   0        0        0     9545 1970-01-01 00:00:00.000000 reflex-0.2.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.1a2/LICENSE
+-rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.1a2/README.md
+-rw-r--r--   0        0        0     2002 2023-07-19 01:58:40.554124 reflex-0.2.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.1a2/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.1a2/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.1a2/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.1a2/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.1a2/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.1a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.1a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.1a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.1a2/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.1a2/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.1a2/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.1a2/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1209 2023-07-19 01:58:26.537471 reflex-0.2.1a2/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.1a2/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.1a2/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.1a2/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.1a2/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.1a2/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10096 2023-07-19 01:58:26.537790 reflex-0.2.1a2/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.1a2/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.1a2/reflex/admin.py
+-rw-r--r--   0        0        0    23515 2023-07-19 01:58:26.539090 reflex-0.2.1a2/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.1a2/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.1a2/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.1a2/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.1a2/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.1a2/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.1a2/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.1a2/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.1a2/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.1a2/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.1a2/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.1a2/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.1a2/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.1a2/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.1a2/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.1a2/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.1a2/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.1a2/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.1a2/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.1a2/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.1a2/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.1a2/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.1a2/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.1a2/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5762 2023-07-19 01:58:26.540483 reflex-0.2.1a2/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.1a2/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.1a2/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.1a2/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.1a2/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.1a2/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.1a2/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.1a2/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.1a2/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.1a2/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.1a2/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.1a2/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.1a2/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.1a2/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.1a2/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.1a2/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.1a2/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.1a2/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.1a2/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.1a2/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.1a2/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.1a2/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.1a2/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.1a2/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.1a2/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.1a2/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.1a2/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.1a2/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.1a2/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.1a2/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.1a2/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.1a2/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.1a2/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.1a2/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.1a2/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.1a2/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.1a2/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.1a2/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.1a2/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.1a2/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.1a2/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.1a2/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.1a2/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.1a2/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.1a2/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.1a2/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.1a2/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.1a2/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.1a2/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.1a2/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.1a2/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.1a2/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.1a2/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.1a2/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.1a2/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.1a2/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.1a2/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.1a2/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.1a2/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.1a2/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.1a2/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.1a2/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.1a2/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.1a2/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.1a2/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.1a2/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.1a2/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.1a2/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.1a2/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.1a2/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.1a2/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.1a2/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.1a2/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.1a2/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.1a2/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.1a2/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.1a2/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.1a2/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.1a2/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.1a2/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.1a2/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2294 2023-07-14 23:13:37.779060 reflex-0.2.1a2/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.1a2/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.1a2/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.1a2/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.1a2/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.1a2/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.1a2/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.1a2/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.1a2/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7215 2023-07-14 23:13:37.779630 reflex-0.2.1a2/reflex/config.py
+-rw-r--r--   0        0        0    10821 2023-07-17 23:29:33.627808 reflex-0.2.1a2/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.1a2/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.1a2/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.1a2/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.1a2/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.1a2/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.1a2/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.1a2/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.1a2/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.1a2/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.1a2/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.1a2/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.1a2/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9473 2023-07-18 01:07:12.549028 reflex-0.2.1a2/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.1a2/reflex/py.typed
+-rw-r--r--   0        0        0    11041 2023-07-19 01:58:26.540979 reflex-0.2.1a2/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.1a2/reflex/route.py
+-rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.1a2/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.1a2/reflex/style.py
+-rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.1a2/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.1a2/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8232 2023-07-19 01:58:26.541268 reflex-0.2.1a2/reflex/utils/build.py
+-rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.1a2/reflex/utils/console.py
+-rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.1a2/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.1a2/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.1a2/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.1a2/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    14056 2023-07-19 01:58:26.541782 reflex-0.2.1a2/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.1a2/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.1a2/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.1a2/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.1a2/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-14 23:13:37.782718 reflex-0.2.1a2/reflex/vars.py
+-rw-r--r--   0        0        0     9586 1970-01-01 00:00:00.000000 reflex-0.2.1a2/PKG-INFO
```

### Comparing `reflex-0.2.1a1/LICENSE` & `reflex-0.2.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/README.md` & `reflex-0.2.1a2/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/pyproject.toml` & `reflex-0.2.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.1a1"
+version = "0.2.1a2"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
@@ -41,14 +41,15 @@
 uvicorn = "^0.20.0"
 watchdog = "^2.3.1"
 watchfiles = "^0.19.0"
 websockets = "^10.4"
 starlette-admin = "^0.9.0"
 python-dotenv = "^0.13.0"
 importlib-metadata = {version = "^6.7.0", python = ">=3.7, <3.8"}
+alembic = "^1.11.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
 pyright = "^1.1.229"
 darglint = "^1.8.1"
 toml = "^0.10.2"
@@ -58,15 +59,14 @@
 ruff = "^0.0.244"
 pandas = [
     {version = "^1.5.3", python = ">=3.8,<4.0"},
     {version = "^1.1", python = ">=3.7, <3.8"}
 ]
 asynctest = "^0.13.0"
 pre-commit = {version = "^3.2.1", python = ">=3.8,<4.0"}
-alembic = "^1.11.1"
 selenium = "^4.10.0"
 
 [tool.poetry.scripts]
 reflex = "reflex.reflex:main"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
```

### Comparing `reflex-0.2.1a1/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.1a2/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/apps/default/default.py` & `reflex-0.2.1a2/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/assets/favicon.ico` & `reflex-0.2.1a2/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.1a2/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.1a2/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/web/bun.lockb` & `reflex-0.2.1a2/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/web/package.json` & `reflex-0.2.1a2/reflex/.templates/web/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'dependencies'": "{'next-sitemap': '^4.1.8'}"}*

```diff
@@ -9,14 +9,15 @@
         "chakra-react-select": "^4.6.0",
         "focus-visible": "^5.2.0",
         "framer-motion": "^10.12.4",
         "gridjs": "^6.0.6",
         "gridjs-react": "^6.0.1",
         "json5": "^2.2.3",
         "next": "^13.3.1",
+        "next-sitemap": "^4.1.8",
         "plotly.js": "^2.22.0",
         "react": "^18.2.0",
         "react-debounce-input": "^3.3.0",
         "react-dom": "^18.2.0",
         "react-dropzone": "^14.2.3",
         "react-markdown": "^8.0.7",
         "react-player": "^2.12.0",
```

### Comparing `reflex-0.2.1a1/reflex/.templates/web/pages/_app.js` & `reflex-0.2.1a2/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.1a2/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/.templates/web/utils/state.js` & `reflex-0.2.1a2/reflex/.templates/web/utils/state.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -335,29 +335,36 @@
             "files",
             files[i],
             getToken() + ":" + handler + ":" + files[i].name
         );
     }
 
     // Send the file to the server.
-    await axios.post(UPLOADURL, formdata, headers).then((response) => {
-        // Apply the delta and set the result.
-        const update = response.data;
-        applyDelta(state, update.delta);
-
-        // Set processing to false and return.
-        setResult({
-            state: state,
-            events: update.events,
-            final: true,
-            processing: false,
-        });
-    });
-
-    return true;
+    await axios.post(UPLOADURL, formdata, headers)
+        .then(() => {
+            return true;
+        })
+        .catch(
+            error => {
+                if (error.response) {
+                    // The request was made and the server responded with a status code
+                    // that falls out of the range of 2xx
+                    console.log(error.response.data);
+                } else if (error.request) {
+                    // The request was made but no response was received
+                    // `error.request` is an instance of XMLHttpRequest in the browser and an instance of
+                    // http.ClientRequest in node.js
+                    console.log(error.request);
+                } else {
+                    // Something happened in setting up the request that triggered an Error
+                    console.log(error.message);
+                }
+                return false;
+            }
+        )
 };
 
 /**
  * Create an event object.
  * @param name The name of the event.
  * @param payload The payload of the event.
  * @param use_websocket Whether the event uses websocket.
```

### Comparing `reflex-0.2.1a1/reflex/__init__.py` & `reflex-0.2.1a2/reflex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from . import el as el
 from .admin import AdminDash as AdminDash
 from .app import App as App
 from .app import UploadFile as UploadFile
 from .base import Base as Base
 from .compiler.utils import get_asset_path
 from .components import *
+from .components.base.script import client_side
 from .components.component import custom_component as memo
 from .components.graphing.victory import data as data
 from .config import Config as Config
 from .config import DBConfig as DBConfig
 from .constants import Env as Env
 from .constants import Transports as Transports
 from .event import EVENT_ARG as EVENT_ARG
```

### Comparing `reflex-0.2.1a1/reflex/app.py` & `reflex-0.2.1a2/reflex/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
 
     # Admin dashboard
     admin_dash: Optional[AdminDash] = None
 
     # The component to render if there is a connection error to the server.
     connect_error_component: Optional[Component] = None
 
+    # The async server name space
+    event_namespace: Optional[AsyncNamespace] = None
+
     def __init__(self, *args, **kwargs):
         """Initialize the app.
 
         Args:
             *args: Args to initialize the app with.
             **kwargs: Kwargs to initialize the app with.
         """
@@ -123,19 +126,18 @@
             ping_timeout=constants.PING_TIMEOUT,
         )
 
         # Create the socket app. Note event endpoint constant replaces the default 'socket.io' path.
         self.socket_app = ASGIApp(self.sio, socketio_path="")
 
         # Create the event namespace and attach the main app. Not related to any paths.
-        event_namespace = EventNamespace("/event", self)
+        self.event_namespace = EventNamespace("/event", self)
 
         # Register the event namespace with the socket.
-        self.sio.register_namespace(event_namespace)
-
+        self.sio.register_namespace(self.event_namespace)
         # Mount the socket app with the API.
         self.api.mount(str(constants.Endpoint.EVENT), self.socket_app)
 
         # Set up the admin dash.
         self.setup_admin_dash()
 
     def __repr__(self) -> str:
@@ -448,18 +450,14 @@
 
         for render, kwargs in DECORATED_ROUTES:
             self.add_page(render, **kwargs)
 
         # Get the env mode.
         config = get_config()
 
-        # Update models during hot reload.
-        if config.db_url is not None and not Model.automigrate():
-            Model.create_all()
-
         # Empty the .web pages directory
         compiler.purge_web_pages_dir()
 
         # Store the compile results.
         compile_results = []
 
         # Compile the pages in parallel.
@@ -592,29 +590,26 @@
 
     async def upload_file(files: List[UploadFile]):
         """Upload a file.
 
         Args:
             files: The file(s) to upload.
 
-        Returns:
-            The state update after processing the event.
-
         Raises:
             ValueError: if there are no args with supported annotation.
         """
         assert files[0].filename is not None
         token, handler = files[0].filename.split(":")[:2]
         for file in files:
             assert file.filename is not None
             file.filename = file.filename.split(":")[-1]
-
         # Get the state for the session.
         state = app.state_manager.get_state(token)
-
+        # get the current session ID
+        sid = state.get_sid()
         # get the current state(parent state/substate)
         path = handler.split(".")[:-1]
         current_state = state.get_substate(path)
         handler_upload_param: Tuple = ()
 
         # get handler function
         func = getattr(current_state, handler.split(".")[-1])
@@ -636,20 +631,25 @@
             )
 
         event = Event(
             token=token,
             name=handler,
             payload={handler_upload_param[0]: files},
         )
-        # TODO: refactor this to handle yields.
-        update = await state._process(event).__anext__()
-
+        async for update in state._process(event):
+            # Postprocess the event.
+            update = await app.postprocess(state, event, update)
+            # Send update to client
+            await asyncio.create_task(
+                app.event_namespace.emit(  # type: ignore
+                    str(constants.SocketEvent.EVENT), update.json(), to=sid
+                )
+            )
         # Set the state for the session.
         app.state_manager.set_state(event.token, state)
-        return update
 
     return upload_file
 
 
 class EventNamespace(AsyncNamespace):
     """The event namespace."""
```

### Comparing `reflex-0.2.1a1/reflex/base.py` & `reflex-0.2.1a2/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/compiler/compiler.py` & `reflex-0.2.1a2/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/compiler/templates.py` & `reflex-0.2.1a2/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/compiler/utils.py` & `reflex-0.2.1a2/reflex/compiler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     Description,
     DocumentHead,
     Head,
     Html,
     Image,
     Main,
     Meta,
+    NextScript,
     RawLink,
-    Script,
     Title,
 )
 from reflex.components.component import Component, ComponentStyle, CustomComponent
 from reflex.event import get_hydrate_event
 from reflex.state import State
 from reflex.style import Style
 from reflex.utils import format, imports, path_ops
@@ -119,15 +119,18 @@
 
     Args:
         state: The app state object.
 
     Returns:
         A dictionary of the compiled state.
     """
-    initial_state = state().dict()
+    try:
+        initial_state = state().dict()
+    except Exception:
+        initial_state = state().dict(include_computed=False)
     initial_state.update(
         {
             "events": [{"name": get_hydrate_event(state)}],
             "files": [],
         }
     )
     return format.format_state(initial_state)
@@ -179,15 +182,15 @@
     """
     sheets = [RawLink.create(rel="stylesheet", href=href) for href in stylesheets]
     return Html.create(
         DocumentHead.create(*sheets),
         Body.create(
             ColorModeScript.create(),
             Main.create(),
-            Script.create(),
+            NextScript.create(),
         ),
     )
 
 
 def create_theme(style: ComponentStyle) -> Dict:
     """Create the base style for the app.
```

### Comparing `reflex-0.2.1a1/reflex/components/__init__.py` & `reflex-0.2.1a2/reflex/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Import all the components."""
 from __future__ import annotations
 
-from .base import ScriptTag
+from .base import Script
 from .component import Component
 from .datadisplay import *
 from .disclosure import *
 from .feedback import *
 from .forms import *
 from .graphing import *
 from .layout import *
@@ -234,13 +234,13 @@
 popover_trigger = PopoverTrigger.create
 tooltip = Tooltip.create
 heading = Heading.create
 highlight = Highlight.create
 markdown = Markdown.create
 span = Span.create
 text = Text.create
-script = ScriptTag.create
+script = Script.create
 aspect_ratio = AspectRatio.create
 kbd = KeyboardKey.create
 color_mode_button = ColorModeButton.create
 color_mode_icon = ColorModeIcon.create
 color_mode_switch = ColorModeSwitch.create
```

### Comparing `reflex-0.2.1a1/reflex/components/base/bare.py` & `reflex-0.2.1a2/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/base/document.py` & `reflex-0.2.1a2/reflex/components/base/document.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class Main(NextDocumentLib):
     """The document main section."""
 
     tag = "Main"
 
 
-class Script(NextDocumentLib):
+class NextScript(NextDocumentLib):
     """The document main scripts."""
 
     tag = "NextScript"
 
 
 class ColorModeScript(ChakraComponent):
     """Chakra color mode script."""
```

### Comparing `reflex-0.2.1a1/reflex/components/base/link.py` & `reflex-0.2.1a2/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/base/meta.py` & `reflex-0.2.1a2/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/component.py` & `reflex-0.2.1a2/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/code.py` & `reflex-0.2.1a2/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/datatable.py` & `reflex-0.2.1a2/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/divider.py` & `reflex-0.2.1a2/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/list.py` & `reflex-0.2.1a2/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/stat.py` & `reflex-0.2.1a2/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/table.py` & `reflex-0.2.1a2/reflex/components/datadisplay/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,16 @@
     @classmethod
     def create(cls, *children, cell_type: str = "", cells=None, **props) -> Component:
         """Create a table row component.
 
         Args:
             children: The children of the component.
             props: The properties of the component.
-            cell_type (str): the type of cells in this table row. "header" or "data". Defaults to None.
-            cells (list, optional): The cells value to add in the table row. Defaults to None.
+            cell_type: the type of cells in this table row. "header" or "data". Defaults to None.
+            cells: The cells value to add in the table row. Defaults to None.
 
         Returns:
             The table row component
         """
         types = {"header": Th, "data": Td}
         cell_cls = types.get(cell_type)
         if len(children) == 0 and cell_cls:
```

### Comparing `reflex-0.2.1a1/reflex/components/datadisplay/tag.py` & `reflex-0.2.1a2/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/disclosure/accordion.py` & `reflex-0.2.1a2/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/disclosure/tabs.py` & `reflex-0.2.1a2/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/disclosure/transition.py` & `reflex-0.2.1a2/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/feedback/alert.py` & `reflex-0.2.1a2/reflex/components/feedback/alert.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     def create(
         cls, *children, icon=True, title="Alert title", desc=None, **props
     ) -> Component:
         """Create an alert component.
 
         Args:
             children: The children of the component.
-            icon (bool): The icon of the alert.
-            title (str): The title of the alert.
-            desc (str): The description of the alert
+            icon: The icon of the alert.
+            title: The title of the alert.
+            desc: The description of the alert
             props: The properties of the component.
 
         Returns:
             The alert component.
         """
         if len(children) == 0:
             children = []
```

### Comparing `reflex-0.2.1a1/reflex/components/feedback/circularprogress.py` & `reflex-0.2.1a2/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/feedback/progress.py` & `reflex-0.2.1a2/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/feedback/skeleton.py` & `reflex-0.2.1a2/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/feedback/spinner.py` & `reflex-0.2.1a2/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/__init__.py` & `reflex-0.2.1a2/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/button.py` & `reflex-0.2.1a2/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/checkbox.py` & `reflex-0.2.1a2/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.1a2/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.1a2/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/debounce.py` & `reflex-0.2.1a2/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/editable.py` & `reflex-0.2.1a2/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/form.py` & `reflex-0.2.1a2/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/iconbutton.py` & `reflex-0.2.1a2/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/input.py` & `reflex-0.2.1a2/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/multiselect.py` & `reflex-0.2.1a2/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/numberinput.py` & `reflex-0.2.1a2/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/pininput.py` & `reflex-0.2.1a2/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/radio.py` & `reflex-0.2.1a2/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/rangeslider.py` & `reflex-0.2.1a2/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/select.py` & `reflex-0.2.1a2/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/slider.py` & `reflex-0.2.1a2/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/switch.py` & `reflex-0.2.1a2/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/textarea.py` & `reflex-0.2.1a2/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/forms/upload.py` & `reflex-0.2.1a2/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/graphing/plotly.py` & `reflex-0.2.1a2/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/graphing/victory.py` & `reflex-0.2.1a2/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/__init__.py` & `reflex-0.2.1a2/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/box.py` & `reflex-0.2.1a2/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/card.py` & `reflex-0.2.1a2/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/cond.py` & `reflex-0.2.1a2/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/flex.py` & `reflex-0.2.1a2/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/foreach.py` & `reflex-0.2.1a2/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/grid.py` & `reflex-0.2.1a2/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/html.py` & `reflex-0.2.1a2/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/responsive.py` & `reflex-0.2.1a2/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/stack.py` & `reflex-0.2.1a2/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/layout/wrap.py` & `reflex-0.2.1a2/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/libs/react_player.py` & `reflex-0.2.1a2/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/media/avatar.py` & `reflex-0.2.1a2/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/media/icon.py` & `reflex-0.2.1a2/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/media/image.py` & `reflex-0.2.1a2/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.1a2/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/navigation/link.py` & `reflex-0.2.1a2/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.1a2/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/navigation/stepper.py` & `reflex-0.2.1a2/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/__init__.py` & `reflex-0.2.1a2/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/alertdialog.py` & `reflex-0.2.1a2/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/banner.py` & `reflex-0.2.1a2/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/drawer.py` & `reflex-0.2.1a2/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/menu.py` & `reflex-0.2.1a2/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/modal.py` & `reflex-0.2.1a2/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/popover.py` & `reflex-0.2.1a2/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/overlay/tooltip.py` & `reflex-0.2.1a2/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/tags/iter_tag.py` & `reflex-0.2.1a2/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/tags/tag.py` & `reflex-0.2.1a2/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/tags/tagless.py` & `reflex-0.2.1a2/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/typography/highlight.py` & `reflex-0.2.1a2/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/components/typography/markdown.py` & `reflex-0.2.1a2/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/config.py` & `reflex-0.2.1a2/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/constants.py` & `reflex-0.2.1a2/reflex/constants.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/el/constants/html.py` & `reflex-0.2.1a2/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/el/constants/react.py` & `reflex-0.2.1a2/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/el/constants/reflex.py` & `reflex-0.2.1a2/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/el/element.py` & `reflex-0.2.1a2/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/el/elements/__init__.py` & `reflex-0.2.1a2/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/el/precompile.py` & `reflex-0.2.1a2/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/event.py` & `reflex-0.2.1a2/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.1a2/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/middleware/middleware.py` & `reflex-0.2.1a2/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/model.py` & `reflex-0.2.1a2/reflex/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 """Database built into Reflex."""
 
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Optional
 
+import alembic.autogenerate
+import alembic.command
+import alembic.config
+import alembic.operations.ops
+import alembic.runtime.environment
+import alembic.script
+import alembic.util
 import sqlalchemy
 import sqlmodel
 
+from reflex import constants
 from reflex.base import Base
 from reflex.config import get_config
-
-from . import constants
-
-try:
-    import alembic.autogenerate  # pyright: ignore [reportMissingImports]
-    import alembic.command  # pyright: ignore [reportMissingImports]
-    import alembic.operations.ops  # pyright: ignore [reportMissingImports]
-    import alembic.runtime.environment  # pyright: ignore [reportMissingImports]
-    import alembic.script  # pyright: ignore [reportMissingImports]
-    import alembic.util  # pyright: ignore [reportMissingImports]
-    from alembic.config import Config  # pyright: ignore [reportMissingImports]
-
-    has_alembic = True
-except ImportError:
-    has_alembic = False
+from reflex.utils import console
 
 
 def get_engine(url: Optional[str] = None):
     """Get the database engine.
 
     Args:
         url: the DB url to use.
@@ -38,14 +32,18 @@
     Raises:
         ValueError: If the database url is None.
     """
     conf = get_config()
     url = url or conf.db_url
     if url is None:
         raise ValueError("No database url configured")
+    if not Path(constants.ALEMBIC_CONFIG).exists():
+        console.print(
+            "[red]Database is not initialized, run [bold]reflex db init[/bold] first."
+        )
     return sqlmodel.create_engine(
         url,
         echo=False,
         connect_args={"check_same_thread": False} if conf.admin_dash else {},
     )
 
 
@@ -96,15 +94,15 @@
     @staticmethod
     def _alembic_config():
         """Get the alembic configuration and script_directory.
 
         Returns:
             tuple of (config, script_directory)
         """
-        config = Config(constants.ALEMBIC_CONFIG)
+        config = alembic.config.Config(constants.ALEMBIC_CONFIG)
         return config, alembic.script.ScriptDirectory(
             config.get_main_option("script_location", default="version"),
         )
 
     @staticmethod
     def _alembic_render_item(
         type_: str,
@@ -116,51 +114,70 @@
         This method is called to provide python code for the given obj,
         but currently it is only used to add `sqlmodel` to the import list
         when generating migration scripts.
 
         See https://alembic.sqlalchemy.org/en/latest/api/runtime.html
 
         Args:
-            type_: one of "schema", "table", "column", "index",
-                "unique_constraint", or "foreign_key_constraint"
-            obj: the object being rendered
-            autogen_context: shared AutogenContext passed to each render_item call
+            type_: One of "schema", "table", "column", "index",
+                "unique_constraint", or "foreign_key_constraint".
+            obj: The object being rendered.
+            autogen_context: Shared AutogenContext passed to each render_item call.
 
         Returns:
-            False - indicating that the default rendering should be used.
+            False - Indicating that the default rendering should be used.
         """
         autogen_context.imports.add("import sqlmodel")
         return False
 
     @classmethod
-    def _alembic_autogenerate(cls, connection: sqlalchemy.engine.Connection) -> bool:
+    def alembic_init(cls):
+        """Initialize alembic for the project."""
+        alembic.command.init(
+            config=alembic.config.Config(constants.ALEMBIC_CONFIG),
+            directory=str(Path(constants.ALEMBIC_CONFIG).parent / "alembic"),
+        )
+
+    @classmethod
+    def alembic_autogenerate(
+        cls,
+        connection: sqlalchemy.engine.Connection,
+        message: Optional[str] = None,
+        write_migration_scripts: bool = True,
+    ) -> bool:
         """Generate migration scripts for alembic-detectable changes.
 
         Args:
-            connection: sqlalchemy connection to use when detecting changes
+            connection: SQLAlchemy connection to use when detecting changes.
+            message: Human readable identifier describing the generated revision.
+            write_migration_scripts: If True, write autogenerated revisions to script directory.
 
         Returns:
             True when changes have been detected.
         """
+        if not Path(constants.ALEMBIC_CONFIG).exists():
+            return False
+
         config, script_directory = cls._alembic_config()
         revision_context = alembic.autogenerate.api.RevisionContext(
             config=config,
             script_directory=script_directory,
             command_args=defaultdict(
                 lambda: None,
                 autogenerate=True,
                 head="head",
+                message=message,
             ),
         )
         writer = alembic.autogenerate.rewriter.Rewriter()
 
         @writer.rewrites(alembic.operations.ops.AddColumnOp)
         def render_add_column_with_server_default(context, revision, op):
             # Carry the sqlmodel default as server_default so that newly added
-            # columns get the desired default value in existing rows
+            # columns get the desired default value in existing rows.
             if op.column.default is not None and op.column.server_default is None:
                 op.column.server_default = sqlalchemy.DefaultClause(
                     sqlalchemy.sql.expression.literal(op.column.default.arg),
                 )
             return op
 
         def run_autogenerate(rev, context):
@@ -180,68 +197,75 @@
             )
             env.run_migrations()
         changes_detected = False
         if revision_context.generated_revisions:
             upgrade_ops = revision_context.generated_revisions[-1].upgrade_ops
             if upgrade_ops is not None:
                 changes_detected = bool(upgrade_ops.ops)
-        if changes_detected:
-            for _script in revision_context.generate_scripts():
-                pass  # must iterate to actually generate the scripts
+        if changes_detected and write_migration_scripts:
+            # Must iterate the generator to actually write the scripts.
+            _ = tuple(revision_context.generate_scripts())
         return changes_detected
 
     @classmethod
     def _alembic_upgrade(
         cls,
         connection: sqlalchemy.engine.Connection,
         to_rev: str = "head",
     ) -> None:
         """Apply alembic migrations up to the given revision.
 
         Args:
-            connection: sqlalchemy connection to use when performing upgrade
-            to_rev: revision to migrate towards
+            connection: SQLAlchemy connection to use when performing upgrade.
+            to_rev: Revision to migrate towards.
         """
         config, script_directory = cls._alembic_config()
 
         def run_upgrade(rev, context):
             return script_directory._upgrade_revs(to_rev, rev)
 
-        # apply updates to database
         with alembic.runtime.environment.EnvironmentContext(
             config=config,
             script=script_directory,
             fn=run_upgrade,
         ) as env:
             env.configure(connection=connection)
             env.run_migrations()
 
     @classmethod
-    def automigrate(cls) -> Optional[bool]:
-        """Generate and execute migrations for all sqlmodel Model classes.
+    def migrate(cls, autogenerate: bool = False) -> Optional[bool]:
+        """Execute alembic migrations for all sqlmodel Model classes.
 
         If alembic is not installed or has not been initialized for the project,
         then no action is performed.
 
+        If there are no revisions currently tracked by alembic, then
+        an initial revision will be created based on sqlmodel metadata.
+
         If models in the app have changed in incompatible ways that alembic
         cannot automatically generate revisions for, the app may not be able to
         start up until migration scripts have been corrected by hand.
 
+        Args:
+            autogenerate: If True, generate migration script and use it to upgrade schema
+                (otherwise, just bring the schema to current "head" revision).
+
         Returns:
-            True - indicating the process was successful
-            None - indicating the process was skipped
+            True - indicating the process was successful.
+            None - indicating the process was skipped.
         """
-        if not has_alembic or not Path(constants.ALEMBIC_CONFIG).exists():
+        if not Path(constants.ALEMBIC_CONFIG).exists():
             return
 
         with cls.get_db_engine().connect() as connection:
             cls._alembic_upgrade(connection=connection)
-            changes_detected = cls._alembic_autogenerate(connection=connection)
-            if changes_detected:
-                cls._alembic_upgrade(connection=connection)
+            if autogenerate:
+                changes_detected = cls.alembic_autogenerate(connection=connection)
+                if changes_detected:
+                    cls._alembic_upgrade(connection=connection)
             connection.commit()
         return True
 
     @classmethod
     @property
     def select(cls):
         """Select rows from the table.
```

### Comparing `reflex-0.2.1a1/reflex/reflex.py` & `reflex-0.2.1a2/reflex/reflex.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import platform
 import signal
 import threading
 from pathlib import Path
 
 import httpx
 import typer
+from alembic.util.exc import CommandError
 
-from reflex import constants
+from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import build, console, exec, prerequisites, processes, telemetry
 
 # Create the app.
 cli = typer.Typer()
 
 
@@ -128,14 +129,17 @@
     # Get the app module.
     console.rule("[bold]Starting Reflex App")
     app = prerequisites.get_app()
 
     # Check the admin dashboard settings.
     prerequisites.check_admin_settings()
 
+    # Warn if schema is not up to date.
+    prerequisites.check_schema_up_to_date()
+
     # Get the frontend and backend commands, based on the environment.
     setup_frontend = frontend_cmd = backend_cmd = None
     if env == constants.Env.DEV:
         setup_frontend, frontend_cmd, backend_cmd = (
             build.setup_frontend,
             exec.run_frontend,
             exec.run_backend,
@@ -154,15 +158,14 @@
     # Run the frontend and backend.
     if frontend:
         setup_frontend(Path.cwd(), loglevel)
         threading.Thread(
             target=frontend_cmd, args=(Path.cwd(), frontend_port, loglevel)
         ).start()
     if backend:
-        build.setup_backend()
         threading.Thread(
             target=backend_cmd,
             args=(app.__name__, backend_host, backend_port, loglevel),
         ).start()
 
     # Display custom message when there is a keyboard interrupt.
     signal.signal(signal.SIGINT, processes.catch_keyboard_interrupt)
@@ -254,11 +257,64 @@
     else:
         console.rule(
             """Backend & Frontend compiled. See [green bold]app[/green bold]
             and [green bold].web/_static[/green bold] directories."""
         )
 
 
+db_cli = typer.Typer()
+
+
+@db_cli.command(name="init")
+def db_init():
+    """Create database schema and migration configuration."""
+    if get_config().db_url is None:
+        console.print("[red]db_url is not configured, cannot initialize.")
+    if Path(constants.ALEMBIC_CONFIG).exists():
+        console.print(
+            "[red]Database is already initialized. Use "
+            "[bold]reflex db makemigrations[/bold] to create schema change "
+            "scripts and [bold]reflex db migrate[/bold] to apply migrations "
+            "to a new or existing database.",
+        )
+        return
+    prerequisites.get_app()
+    model.Model.alembic_init()
+    model.Model.migrate(autogenerate=True)
+
+
+@db_cli.command()
+def migrate():
+    """Create or update database schema from migration scripts."""
+    prerequisites.get_app()
+    if not prerequisites.check_db_initialized():
+        return
+    model.Model.migrate()
+    prerequisites.check_schema_up_to_date()
+
+
+@db_cli.command()
+def makemigrations(
+    message: str = typer.Option(
+        None, help="Human readable identifier for the generated revision."
+    ),
+):
+    """Create autogenerated alembic migration scripts."""
+    prerequisites.get_app()
+    if not prerequisites.check_db_initialized():
+        return
+    with model.Model.get_db_engine().connect() as connection:
+        try:
+            model.Model.alembic_autogenerate(connection=connection, message=message)
+        except CommandError as command_error:
+            if "Target database is not up to date." not in str(command_error):
+                raise
+            console.print(
+                f"[red]{command_error} Run [bold]reflex db migrate[/bold] to update database."
+            )
+
+
+cli.add_typer(db_cli, name="db", help="Subcommands for managing the database schema")
 main = cli
 
 if __name__ == "__main__":
     main()
```

### Comparing `reflex-0.2.1a1/reflex/route.py` & `reflex-0.2.1a2/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/state.py` & `reflex-0.2.1a2/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/style.py` & `reflex-0.2.1a2/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/testing.py` & `reflex-0.2.1a2/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/build.py` & `reflex-0.2.1a2/reflex/utils/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import json
 import os
 import random
 import subprocess
 from pathlib import Path
 from typing import Optional, Union
 
-from rich.progress import Progress
+from rich.progress import MofNCompleteColumn, Progress, TimeElapsedColumn
 
 from reflex import constants
 from reflex.config import get_config
-from reflex.utils import path_ops, prerequisites
+from reflex.utils import console, path_ops, prerequisites
 from reflex.utils.processes import new_process
 
 
 def update_json_file(file_path: str, update_dict: dict[str, Union[int, str]]):
     """Update the contents of a json file.
 
     Args:
@@ -62,15 +62,15 @@
     """
     for key, value in kwargs.items():
         if not value:
             continue
         os.environ[key.upper()] = value
 
 
-def generate_sitemap(deploy_url: str):
+def generate_sitemap_config(deploy_url: str):
     """Generate the sitemap config file.
 
     Args:
         deploy_url: The URL of the deployed app.
     """
     # Import here to avoid circular imports.
     from reflex.compiler import templates
@@ -82,14 +82,23 @@
         }
     )
 
     with open(constants.SITEMAP_CONFIG_FILE, "w") as f:
         f.write(templates.SITEMAP_CONFIG(config=config))
 
 
+def generate_sitemap():
+    """Generate the actual sitemap."""
+    subprocess.run(
+        [prerequisites.get_package_manager(), "run", "next-sitemap"],
+        cwd=constants.WEB_DIR,
+        stdout=subprocess.PIPE,
+    )
+
+
 def export_app(
     backend: bool = True,
     frontend: bool = True,
     zip: bool = False,
     deploy_url: Optional[str] = None,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
@@ -103,47 +112,69 @@
         loglevel: The log level to use.
     """
     # Remove the static folder.
     path_ops.rm(constants.WEB_STATIC_DIR)
 
     # Generate the sitemap file.
     if deploy_url is not None:
-        generate_sitemap(deploy_url)
+        generate_sitemap_config(deploy_url)
 
     # Create a progress object
-    progress = Progress()
+    progress = Progress(
+        *Progress.get_default_columns()[:-1],
+        MofNCompleteColumn(),
+        TimeElapsedColumn(),
+    )
+
+    checkpoints = [
+        "Linting and checking ",
+        "Compiled successfully",
+        "Route (pages)",
+        "Collecting page data",
+        "automatically rendered as static HTML",
+        'Copying "static build" directory',
+        'Copying "public" directory',
+        "Finalizing page optimization",
+        "Export successful",
+    ]
 
     # Add a single task to the progress object
-    task = progress.add_task("Building app... ", total=500)
+    task = progress.add_task("Creating Production Build: ", total=len(checkpoints))
 
     # Start the subprocess with the progress bar.
-    with progress, new_process(
-        [prerequisites.get_package_manager(), "run", "export"],
-        cwd=constants.WEB_DIR,
-    ) as export_process:
-        assert export_process.stdout is not None, "No stdout for export process."
-        for line in export_process.stdout:
-            # Print the line in debug mode.
-            if loglevel == constants.LogLevel.DEBUG:
-                print(line, end="")
-
-            # Check for special strings and update the progress bar.
-            if "Linting and checking " in line:
-                progress.update(task, advance=100)
-            elif "Compiled successfully" in line:
-                progress.update(task, advance=100)
-            elif "Route (pages)" in line:
-                progress.update(task, advance=100)
-            elif "automatically rendered as static HTML" in line:
-                progress.update(task, advance=100)
-            elif "Export successful" in line:
-                progress.update(task, completed=500)
-                break  # Exit the loop if the completion message is found
+    try:
+        with progress, new_process(
+            [prerequisites.get_package_manager(), "run", "export"],
+            cwd=constants.WEB_DIR,
+        ) as export_process:
+            assert export_process.stdout is not None, "No stdout for export process."
+            for line in export_process.stdout:
+                if loglevel == constants.LogLevel.DEBUG:
+                    print(line, end="")
+
+                # Check for special strings and update the progress bar.
+                for special_string in checkpoints:
+                    if special_string in line:
+                        if special_string == "Export successful":
+                            progress.update(task, completed=len(checkpoints))
+                            break  # Exit the loop if the completion message is found
+                        else:
+                            progress.update(task, advance=1)
+                            break
+
+    except Exception as e:
+        console.print(f"[red]Export process errored: {e}")
+        console.print(
+            "[red]Run in with [bold]--loglevel debug[/bold] to see the full error."
+        )
+        os._exit(1)
 
-        print("Export process completed.")
+    # Generate the actual sitemap.
+    if deploy_url is not None:
+        generate_sitemap()
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
@@ -235,21 +266,8 @@
 
     Args:
         root: The root path of the project.
         loglevel: The log level to use.
         disable_telemetry: Whether to disable the Next telemetry.
     """
     setup_frontend(root, loglevel, disable_telemetry)
-    export_app(loglevel=loglevel)
-
-
-def setup_backend():
-    """Set up backend.
-
-    Specifically ensures backend database is updated when running --no-frontend.
-    """
-    # Import here to avoid circular imports.
-    from reflex.model import Model
-
-    config = get_config()
-    if config.db_url is not None:
-        Model.create_all()
+    export_app(loglevel=loglevel, deploy_url=get_config().deploy_url)
```

### Comparing `reflex-0.2.1a1/reflex/utils/console.py` & `reflex-0.2.1a2/reflex/utils/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,58 +21,58 @@
     _console.print(f"[yellow]DeprecationWarning: {msg}[/yellow]")
 
 
 def log(msg: str) -> None:
     """Takes a string and logs it to the console.
 
     Args:
-        msg (str): The message to log.
+        msg: The message to log.
     """
     _console.log(msg)
 
 
 def print(msg: str) -> None:
     """Prints the given message to the console.
 
     Args:
-        msg (str): The message to print to the console.
+        msg: The message to print to the console.
     """
     _console.print(msg)
 
 
 def rule(title: str) -> None:
     """Prints a horizontal rule with a title.
 
     Args:
-        title (str): The title of the rule.
+        title: The title of the rule.
     """
     _console.rule(title)
 
 
 def ask(
     question: str, choices: Optional[List[str]] = None, default: Optional[str] = None
 ) -> str:
     """Takes a prompt question and optionally a list of choices
      and returns the user input.
 
     Args:
-        question (str): The question to ask the user.
-        choices (Optional[List[str]]): A list of choices to select from.
-        default(Optional[str]): The default option selected.
+        question: The question to ask the user.
+        choices: A list of choices to select from.
+        default: The default option selected.
 
     Returns:
         A string
     """
     return Prompt.ask(question, choices=choices, default=default)  # type: ignore
 
 
 def status(msg: str) -> Status:
     """Returns a status,
     which can be used as a context manager.
 
     Args:
-        msg (str): The message to be used as status title.
+        msg: The message to be used as status title.
 
     Returns:
         The status of the console.
     """
     return _console.status(msg)
```

### Comparing `reflex-0.2.1a1/reflex/utils/exec.py` & `reflex-0.2.1a2/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/format.py` & `reflex-0.2.1a2/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/imports.py` & `reflex-0.2.1a2/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/path_ops.py` & `reflex-0.2.1a2/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/prerequisites.py` & `reflex-0.2.1a2/reflex/utils/prerequisites.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 from datetime import datetime
 from fileinput import FileInput
 from pathlib import Path
 from types import ModuleType
 from typing import Optional
 
 import typer
+from alembic.util.exc import CommandError
 from packaging import version
 from redis import Redis
 
-from reflex import constants
+from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import console, path_ops
 
 
 def check_node_version(min_version=constants.MIN_NODE_VERSION):
     """Check the version of Node.js.
 
@@ -304,15 +305,15 @@
 
 
 def install_frontend_packages(web_dir: str):
     """Installs the base and custom frontend packages
     into the given web directory.
 
     Args:
-        web_dir (str): The directory where the frontend code is located.
+        web_dir: The directory where the frontend code is located.
     """
     # Install the frontend packages.
     console.rule("[bold]Installing frontend packages")
 
     # Install the base packages.
     subprocess.run(
         [get_package_manager(), "install"],
@@ -366,14 +367,49 @@
                 f"[yellow][Admin Dashboard][/yellow] Admin enabled, building admin dashboard. Time: {current_time}"
             )
             console.print(
                 "Admin dashboard running at: [bold green]http://localhost:8000/admin[/bold green]"
             )
 
 
+def check_db_initialized() -> bool:
+    """Check if the database migrations are initialized.
+
+    Returns:
+        True if alembic is initialized (or if database is not used).
+    """
+    if get_config().db_url is not None and not Path(constants.ALEMBIC_CONFIG).exists():
+        console.print(
+            "[red]Database is not initialized. Run [bold]reflex db init[/bold] first."
+        )
+        return False
+    return True
+
+
+def check_schema_up_to_date():
+    """Check if the sqlmodel metadata matches the current database schema."""
+    if get_config().db_url is None or not Path(constants.ALEMBIC_CONFIG).exists():
+        return
+    with model.Model.get_db_engine().connect() as connection:
+        try:
+            if model.Model.alembic_autogenerate(
+                connection=connection,
+                write_migration_scripts=False,
+            ):
+                console.print(
+                    "[red]Detected database schema changes. Run [bold]reflex db makemigrations[/bold] "
+                    "to generate migration scripts.",
+                )
+        except CommandError as command_error:
+            if "Target database is not up to date." in str(command_error):
+                console.print(
+                    f"[red]{command_error} Run [bold]reflex db migrate[/bold] to update database."
+                )
+
+
 def migrate_to_reflex():
     """Migration from Pynecone to Reflex."""
     # Check if the old config file exists.
     if not os.path.exists(constants.OLD_CONFIG_FILE):
         return
 
     # Ask the user if they want to migrate.
```

### Comparing `reflex-0.2.1a1/reflex/utils/processes.py` & `reflex-0.2.1a2/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/telemetry.py` & `reflex-0.2.1a2/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/types.py` & `reflex-0.2.1a2/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/utils/watch.py` & `reflex-0.2.1a2/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/reflex/vars.py` & `reflex-0.2.1a2/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a1/PKG-INFO` & `reflex-0.2.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.1a1
+Version: 0.2.1a2
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: plotly (>=5.13.0,<6.0.0)
```

