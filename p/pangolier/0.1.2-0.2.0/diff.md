# Comparing `tmp/pangolier-0.1.2-py3-none-any.whl.zip` & `tmp/pangolier-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 5175 bytes, number of entries: 10
+Zip file size: 5750 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 22-Aug-07 02:48 pangolier/__init__.py
--rw-rw-r--  2.0 unx      336 b- defN 23-Jun-12 03:36 pangolier/common.py
--rw-rw-r--  2.0 unx      707 b- defN 23-Jul-05 09:20 pangolier/filters.py
--rw-rw-r--  2.0 unx     2930 b- defN 23-Jan-16 03:51 pangolier/functions.py
--rw-rw-r--  2.0 unx     3153 b- defN 23-Jun-12 03:36 pangolier/metrics.py
--rw-rw-r--  2.0 unx     1121 b- defN 22-Aug-08 12:44 pangolier/prefixes.py
--rw-rw-r--  2.0 unx     3701 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-Jul-05 09:21 pangolier-0.1.2.dist-info/RECORD
-10 files, 12816 bytes uncompressed, 3875 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      377 b- defN 23-Jul-19 06:54 pangolier/common.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jul-19 06:54 pangolier/filters.py
+-rw-rw-r--  2.0 unx     3367 b- defN 23-Jul-19 06:54 pangolier/functions.py
+-rw-rw-r--  2.0 unx     3985 b- defN 23-Jul-19 06:54 pangolier/metrics.py
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-19 06:54 pangolier/prefixes.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-19 06:54 pangolier/py.typed
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-19 06:55 pangolier-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-19 06:55 pangolier-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-19 06:55 pangolier-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      838 b- defN 23-Jul-19 06:55 pangolier-0.2.0.dist-info/RECORD
+11 files, 14753 bytes uncompressed, 4338 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -12,20 +12,23 @@
 
 Filename: pangolier/metrics.py
 Comment: 
 
 Filename: pangolier/prefixes.py
 Comment: 
 
-Filename: pangolier-0.1.2.dist-info/METADATA
+Filename: pangolier/py.typed
 Comment: 
 
-Filename: pangolier-0.1.2.dist-info/WHEEL
+Filename: pangolier-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pangolier-0.1.2.dist-info/top_level.txt
+Filename: pangolier-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pangolier-0.1.2.dist-info/RECORD
+Filename: pangolier-0.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: pangolier-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pangolier/common.py

```diff
@@ -1,15 +1,15 @@
 from textwrap import indent
 
 
-def indent_body(body):
+def indent_body(body: str) -> str:
     return indent(body, ' ' * 4)
 
 
-def format_modifier(name, args, pretty):
+def format_modifier(name: str, args: list[str], pretty: bool) -> str:
     if not args:
         return name
 
     body = ', '.join(args)
 
     if pretty:
         return '%s(\n%s\n)' % (
```

## pangolier/filters.py

```diff
@@ -1,31 +1,40 @@
+from typing import Union
+
+
 class FilterBase:
-    def __init__(self, expression):
+    expression: str
+
+    def __init__(self, expression: str):
         self.expression = expression
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         raise NotImplementedError
 
 
 class EqualFilter(FilterBase):
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         return '="%s"' % self.expression
 
 
 class NotEqualFilter(FilterBase):
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         return '!="%s"' % self.expression
 
 
 class RegexpFilter(FilterBase):
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         return '=~"%s"' % self.expression
 
 
-def _make_filter(value):
+FilterValueType = Union[str, FilterBase]
+FilterTuple = tuple[str, FilterBase]
+
+
+def _make_filter(value: FilterValueType) -> FilterBase:
     if isinstance(value, str):
         return EqualFilter(value)
 
     if isinstance(value, FilterBase):
         return value
 
     raise ValueError('cannot parse filter: %r' % value)
```

## pangolier/functions.py

```diff
@@ -1,29 +1,35 @@
+from typing import Union
+
 from .common import indent_body
 from .metrics import MetricBase
 
+ArgType = Union[int, float, str, MetricBase]
+
 
 class FunctionBase(MetricBase):
     pass
 
 
-def _format_arg(arg, pretty=False):
+def _format_arg(arg: ArgType, pretty: bool = False) -> str:
     if isinstance(arg, MetricBase):
         return arg.to_str(pretty=pretty)
 
     return str(arg)
 
 
 class SimpleFunction(FunctionBase):
+    argv: list[ArgType]
+
     name = 'unknown'
 
-    def __init__(self, *argv):
-        self.argv = argv
+    def __init__(self, *argv: ArgType):
+        self.argv = list(argv)
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         formatted_argv = [
             _format_arg(arg, pretty=pretty)
             for arg in self.argv
         ]
 
         if pretty:
             return '%s(\n%s\n)' % (
@@ -35,62 +41,68 @@
             )
 
         return '%s(%s)' % (
             self.name, ', '.join(formatted_argv)
         )
 
 
-def function(name):
+def function(name: str) -> type[SimpleFunction]:
     return type(
         'simple_function_%s' % name,
         (SimpleFunction,),
         {'name': name}
     )
 
 
 class RangeFunction(FunctionBase):
+    origin_metric: MetricBase
+    timespan: str
+
     name = 'unknown'
 
-    def __init__(self, origin_metric, timespan):
+    def __init__(self, origin_metric: MetricBase, timespan: str):
         self.origin_metric = origin_metric
         self.timespan = timespan
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         body = self.origin_metric.to_str(pretty=pretty)
 
         if pretty:
             return '%s(\n%s[%s]\n)' % (
                 self.name,
                 indent_body(body),
                 self.timespan
             )
 
         return '%s(%s[%s])' % (self.name, body, self.timespan)
 
 
-def range_function(name):
+def range_function(name: str) -> type[RangeFunction]:
     return type(
         'range_function_%s' % name,
         (RangeFunction,),
         {'name': name}
     )
 
 
 class AggregationOperator(FunctionBase):
+    argv: list[ArgType]
+    kwargs: dict[str, list[str]]
+
     name = 'unknown'
 
-    def __init__(self, *argv, **kwargs):
-        self.argv = argv
+    def __init__(self, *argv: ArgType, **kwargs: list[str]):
+        self.argv = list(argv)
 
         if len(kwargs) > 1:
             raise ValueError('too many kwargs: %s' % kwargs)
 
         self.kwargs = kwargs
 
-    def _make_clause(self, pretty=False):
+    def _make_clause(self, pretty: bool = False) -> str:
         if self.kwargs:
             key, value = next(iter(self.kwargs.items()))
 
             body = ', '.join(value)
 
             if pretty:
                 return ' %s(\n%s\n)' % (
@@ -98,15 +110,15 @@
                     indent_body(body)
                 )
 
             return ' %s(%s)' % (key, body)
 
         return ''
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         clause = self._make_clause(pretty=pretty)
 
         formatted_argv = [
             _format_arg(arg, pretty=pretty)
             for arg in self.argv
         ]
 
@@ -121,13 +133,13 @@
             )
 
         return '%s%s(%s)' % (
             self.name, clause, ', '.join(formatted_argv)
         )
 
 
-def aggregation_operator(name):
+def aggregation_operator(name: str) -> type[AggregationOperator]:
     return type(
         'aggregation_operator_%s' % name,
         (AggregationOperator,),
         {'name': name}
     )
```

## pangolier/metrics.py

```diff
@@ -1,54 +1,61 @@
+from typing import Optional
+
 from .common import indent_body, format_modifier
-from .filters import _make_filter
+from .filters import _make_filter, FilterValueType, FilterTuple
 
 
 class MetricBase:
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         raise NotImplementedError
 
-    def __add__(self, other):
+    def __add__(self, other: 'MetricBase') -> 'MetricBase':
         return BinOp('+', self, other)
 
-    def __sub__(self, other):
+    def __sub__(self, other: 'MetricBase') -> 'MetricBase':
         return BinOp('-', self, other)
 
-    def __mul__(self, other):
+    def __mul__(self, other: 'MetricBase') -> 'MetricBase':
         return BinOp('*', self, other)
 
-    def __truediv__(self, other):
+    def __truediv__(self, other: 'MetricBase') -> 'MetricBase':
         return BinOp('/', self, other)
 
-    def __mod__(self, other):
+    def __mod__(self, other: 'MetricBase') -> 'MetricBase':
         return BinOp('%', self, other)
 
-    def __xor__(self, other):
+    def __xor__(self, other: 'MetricBase') -> 'MetricBase':
         return BinOp('^', self, other)
 
 
 class Metric(MetricBase):
-    def __init__(self, name):
+    name: str
+
+    def __init__(self, name: str):
         self.name = name
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         return self.name
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs: FilterValueType) -> 'FilteredMetric':
         return FilteredMetric(self, [
             (k, _make_filter(v))
             for k, v in kwargs.items()
         ])
 
 
 class FilteredMetric(MetricBase):
-    def __init__(self, origin_metric, filters):
+    origin_metric: MetricBase
+    filters: list[FilterTuple]
+
+    def __init__(self, origin_metric: MetricBase, filters: list[FilterTuple]):
         self.origin_metric = origin_metric
         self.filters = filters
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         if not self.filters:
             return self.origin_metric.to_str(pretty=pretty)
 
         body_parts = [
             '%s%s' % (k, f.to_str(pretty=pretty))
             for k, f in self.filters
         ]
@@ -60,61 +67,76 @@
             )
 
         return '%s{%s}' % (
             self.origin_metric.to_str(),
             ', '.join(body_parts)
         )
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs: FilterValueType) -> 'FilteredMetric':
         append_filters = [
             (k, _make_filter(v))
             for k, v in kwargs.items()
         ]
 
         return FilteredMetric(
             self.origin_metric,
             self.filters + append_filters
         )
 
 
 class GroupBase(MetricBase):
     modifier = ''
+    labels: list[str]
 
-    def __init__(self, *labels):
-        self.labels = labels
+    def __init__(self, *labels: str):
+        self.labels = list(labels)
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         return format_modifier(self.modifier, self.labels, pretty=pretty)
 
 
 class GroupLeft(GroupBase):
     modifier = 'group_left'
 
 
 class GroupRight(GroupBase):
     modifier = 'group_right'
 
 
 class BinOp(MetricBase):
+    op: str
+    first: MetricBase
+    second: MetricBase
+
+    on: Optional[list[str]]
+    ignoring: Optional[list[str]]
+    group: Optional[GroupBase]
+
     def __init__(
-        self, op, first, second,
-        *, on=None, ignoring=None, group=None,
+        self,
+        op: str,
+        first: MetricBase,
+        second: MetricBase,
+        *,
+        on: Optional[list[str]] = None,
+        ignoring: Optional[list[str]] = None,
+        group: Optional[GroupBase] = None,
     ):
         if on and ignoring:
             raise ValueError('can not specific both `on` and `ignoring`')
 
         self.op = op
         self.first = first
         self.second = second
 
         self.on = on
         self.ignoring = ignoring
         self.group = group
 
-    def to_str(self, pretty=False):
+    def to_str(self, pretty: bool = False) -> str:
         parts = []
 
         parts.append(self.first.to_str(pretty=pretty))
         parts.append(self.op)
 
         if self.on:
             parts.append(
```

## pangolier/prefixes.py

```diff
@@ -1,46 +1,55 @@
-from .filters import _make_filter
-from .metrics import Metric, FilteredMetric
+from .filters import _make_filter, FilterValueType, FilterTuple
+from .metrics import MetricBase, Metric, FilteredMetric
 
 
 class PrefixBase:
-    def add_suffix(self, suffix):
+    def add_suffix(self, suffix: str) -> MetricBase:
         raise NotImplementedError
 
 
 class MetricPrefix(PrefixBase):
-    def __init__(self, name):
+    name: str
+
+    def __init__(self, name: str):
         self.name = name
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs: FilterValueType) -> 'FilteredMetricPrefix':
         return FilteredMetricPrefix(self, [
             (k, _make_filter(v))
             for k, v in kwargs.items()
         ])
 
-    def add_suffix(self, suffix):
+    def add_suffix(self, suffix: str) -> Metric:
         return Metric(
             name=self.name + suffix
         )
 
 
 class FilteredMetricPrefix(PrefixBase):
-    def __init__(self, origin_metric, filters):
+    origin_metric: MetricPrefix
+    filters: list[FilterTuple]
+
+    def __init__(
+        self,
+        origin_metric: MetricPrefix,
+        filters: list[FilterTuple]
+    ):
         self.origin_metric = origin_metric
         self.filters = filters
 
-    def filter(self, **kwargs):
+    def filter(self, **kwargs: FilterValueType) -> 'FilteredMetricPrefix':
         append_filters = [
             (k, _make_filter(v))
             for k, v in kwargs.items()
         ]
 
         return FilteredMetricPrefix(
             self.origin_metric,
             self.filters + append_filters
         )
 
-    def add_suffix(self, suffix):
+    def add_suffix(self, suffix: str) -> FilteredMetric:
         return FilteredMetric(
             origin_metric=self.origin_metric.add_suffix(suffix),
             filters=self.filters
         )
```

## Comparing `pangolier-0.1.2.dist-info/METADATA` & `pangolier-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangolier
-Version: 0.1.2
+Version: 0.2.0
 Summary: prometheus query builder
 Home-page: https://github.com/lexdene/pangolier
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 
 # Pangolier
 
@@ -82,15 +82,15 @@
 `aggregation_operator` shoule be used for aggregation operators:
 
     from pangolier.functions import aggregation_operator
 
     sum_ = aggregation_operator('sum')
     print(sum_(
         Metric('http_requests_total'),
-        by=('job', 'group'),
+        by=['job', 'group'],
     ).to_str(pretty=True))
 
 output:
 
     sum by(
         job, group
     )(
@@ -106,15 +106,15 @@
     print(histogram_quantile(
         0.9,
         sum_(
             rate(
                 Metric('http_request_duration_seconds_bucket'),
                 timespan='5m',
             ),
-            by=('le',)
+            by=['le']
         )
     ).to_str(pretty=True))
 
 output:
 
     histogram_quantile(
         0.9,
@@ -174,15 +174,15 @@
 
     from pangolier.metrics import Metric, BinOp, GroupLeft
 
     print(BinOp(
         '*',
         Metric('foo'),
         Metric('bar'),
-        on=('interface', 'job'),
+        on=['interface', 'job'],
         group=GroupLeft('node', 'resource'),
     ).to_str(pretty=True))
 
 output:
 
     foo * on(
         interface, job
```

## Comparing `pangolier-0.1.2.dist-info/RECORD` & `pangolier-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 pangolier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pangolier/common.py,sha256=6CiIILgtgsnSlYkreEOirY1Ox85e_iNBUqTnAmawxgM,336
-pangolier/filters.py,sha256=i5H3myifUoQWFHvnQhAb-dTLJf3AFbrsg5dtQR5uOCA,707
-pangolier/functions.py,sha256=wLnItRKEoCT5tnKX0ZgIbl6gPGB-_qosCz4v0qba8fI,2930
-pangolier/metrics.py,sha256=D47ly81aVF1jEKZPFtzhdP_Dyg7Ukh18QqvfCztwBzw,3153
-pangolier/prefixes.py,sha256=5lgLpoRUF2oP3eT5BEzWyOOxTb_dGdl6LR8YBvtWKtU,1121
-pangolier-0.1.2.dist-info/METADATA,sha256=tu_KDa5D39W2fUi-4HD4dkwHY8Lt_DQ09S6Nr36SeSE,3701
-pangolier-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pangolier-0.1.2.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
-pangolier-0.1.2.dist-info/RECORD,,
+pangolier/common.py,sha256=enIr17z5ft5Yc1RB0t-gSuspvFaPxv2efJF2ZxS8sLc,377
+pangolier/filters.py,sha256=tTKNnyQERNe7EvzLqVjlqqlI0F2O5fiCxkKzVcMeUrQ,931
+pangolier/functions.py,sha256=OqE9ZoZ0FmDPtl85_b14Na_QXhCnxGwqNXfgflynUrY,3367
+pangolier/metrics.py,sha256=cLr4uY9SXs-M-oVpiDDiz_K8EyqfHd9qJEnfNmfE9KI,3985
+pangolier/prefixes.py,sha256=H5gT5EPUEpnU9ObfpxILnANxhMHj2PgHfQZXEA02_54,1453
+pangolier/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pangolier-0.2.0.dist-info/METADATA,sha256=jQC1uENvJ4AuVHOf6obWTHUeIYPhNcpUXpl_s6T_vvU,3700
+pangolier-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pangolier-0.2.0.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
+pangolier-0.2.0.dist-info/RECORD,,
```

