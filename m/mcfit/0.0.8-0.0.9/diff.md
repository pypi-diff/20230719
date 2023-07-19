# Comparing `tmp/mcfit-0.0.8.tar.gz` & `tmp/mcfit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mcfit-0.0.8.tar", last modified: Wed Apr 18 22:32:14 2018, max compression
+gzip compressed data, was "dist/mcfit-0.0.9.tar", last modified: Wed Jun 13 02:24:51 2018, max compression
```

## Comparing `mcfit-0.0.8.tar` & `mcfit-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-04-18 22:32:14.000000 mcfit-0.0.8/
-drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit/
--rw-r--r--   0 tg        (1000) users      (100)    12685 2018-04-18 17:39:31.000000 mcfit-0.0.8/mcfit/mcfit.py
-drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit/tests/
--rw-r--r--   0 tg        (1000) users      (100)     1174 2018-04-18 21:43:07.000000 mcfit-0.0.8/mcfit/tests/test_mcfit.py
--rw-r--r--   0 tg        (1000) users      (100)      659 2017-09-08 12:27:17.000000 mcfit-0.0.8/mcfit/tests/test_transforms.py
--rw-r--r--   0 tg        (1000) users      (100)        0 2017-06-07 04:15:59.000000 mcfit-0.0.8/mcfit/tests/__init__.py
--rw-r--r--   0 tg        (1000) users      (100)     4089 2018-03-29 17:15:04.000000 mcfit-0.0.8/mcfit/transforms.py
--rw-r--r--   0 tg        (1000) users      (100)     2238 2018-04-17 03:35:06.000000 mcfit-0.0.8/mcfit/cosmology.py
--rw-r--r--   0 tg        (1000) users      (100)     3744 2018-03-29 16:11:26.000000 mcfit-0.0.8/mcfit/kernels.py
--rw-r--r--   0 tg        (1000) users      (100)      138 2018-04-14 21:44:34.000000 mcfit-0.0.8/mcfit/__init__.py
--rw-r--r--   0 tg        (1000) users      (100)     1149 2017-10-16 18:07:42.000000 mcfit-0.0.8/README.rst
--rw-r--r--   0 tg        (1000) users      (100)      317 2018-04-18 22:32:14.000000 mcfit-0.0.8/PKG-INFO
--rw-r--r--   0 tg        (1000) users      (100)       38 2018-04-18 22:32:14.000000 mcfit-0.0.8/setup.cfg
--rw-r--r--   0 tg        (1000) users      (100)      473 2018-04-18 21:47:08.000000 mcfit-0.0.8/setup.py
-drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit.egg-info/
--rw-r--r--   0 tg        (1000) users      (100)        1 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit.egg-info/dependency_links.txt
--rw-r--r--   0 tg        (1000) users      (100)      317 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit.egg-info/PKG-INFO
--rw-r--r--   0 tg        (1000) users      (100)      333 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit.egg-info/SOURCES.txt
--rw-r--r--   0 tg        (1000) users      (100)        6 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit.egg-info/top_level.txt
--rw-r--r--   0 tg        (1000) users      (100)       19 2018-04-18 22:32:14.000000 mcfit-0.0.8/mcfit.egg-info/requires.txt
+drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-06-13 02:24:51.000000 mcfit-0.0.9/
+drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit/
+-rw-r--r--   0 tg        (1000) users      (100)    13233 2018-06-01 18:35:57.000000 mcfit-0.0.9/mcfit/mcfit.py
+drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit/tests/
+-rw-r--r--   0 tg        (1000) users      (100)     1329 2018-06-01 21:25:08.000000 mcfit-0.0.9/mcfit/tests/test_mcfit.py
+-rw-r--r--   0 tg        (1000) users      (100)      659 2017-09-08 12:27:17.000000 mcfit-0.0.9/mcfit/tests/test_transforms.py
+-rw-r--r--   0 tg        (1000) users      (100)        0 2017-06-07 04:15:59.000000 mcfit-0.0.9/mcfit/tests/__init__.py
+-rw-r--r--   0 tg        (1000) users      (100)     3907 2018-05-22 05:07:01.000000 mcfit-0.0.9/mcfit/transforms.py
+-rw-r--r--   0 tg        (1000) users      (100)     1996 2018-05-22 05:07:27.000000 mcfit-0.0.9/mcfit/cosmology.py
+-rw-r--r--   0 tg        (1000) users      (100)     3744 2018-03-29 16:11:26.000000 mcfit-0.0.9/mcfit/kernels.py
+-rw-r--r--   0 tg        (1000) users      (100)      138 2018-04-14 21:44:34.000000 mcfit-0.0.9/mcfit/__init__.py
+-rw-r--r--   0 tg        (1000) users      (100)     2703 2018-04-27 04:08:20.000000 mcfit-0.0.9/README.rst
+-rw-r--r--   0 tg        (1000) users      (100)      317 2018-06-13 02:24:51.000000 mcfit-0.0.9/PKG-INFO
+-rw-r--r--   0 tg        (1000) users      (100)       38 2018-06-13 02:24:51.000000 mcfit-0.0.9/setup.cfg
+-rw-r--r--   0 tg        (1000) users      (100)      473 2018-06-13 02:17:53.000000 mcfit-0.0.9/setup.py
+drwxr-xr-x   0 tg        (1000) users      (100)        0 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit.egg-info/
+-rw-r--r--   0 tg        (1000) users      (100)        1 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit.egg-info/dependency_links.txt
+-rw-r--r--   0 tg        (1000) users      (100)      317 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit.egg-info/PKG-INFO
+-rw-r--r--   0 tg        (1000) users      (100)      333 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit.egg-info/SOURCES.txt
+-rw-r--r--   0 tg        (1000) users      (100)        6 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit.egg-info/top_level.txt
+-rw-r--r--   0 tg        (1000) users      (100)       19 2018-06-13 02:24:51.000000 mcfit-0.0.9/mcfit.egg-info/requires.txt
```

### Comparing `mcfit-0.0.8/mcfit/mcfit.py` & `mcfit-0.0.9/mcfit/mcfit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,110 @@
-from __future__ import print_function, division
+from __future__ import division
 import numpy
 
 
 class mcfit(object):
     r"""Compute integral transforms as a multiplicative convolution.
 
     The generic form is
-    .. math:: G(y) = \int_0^\infty F(x) K(xy) \,\frac{\mathrm{d}x}x
+    .. math:: G(y) = \int_0^\infty F(x) K(xy) \frac{dx}x
 
     Here :math:`F(x)` is the input function, :math:`G(y)` is the output
     function, and :math:`K(xy)` is the integral kernel.
     One is free to scale all three functions by a power law
 
-    .. math:: g(y) = \int_0^\infty f(x) k(xy) \,\frac{\mathrm{d}x}x
+    .. math:: g(y) = \int_0^\infty f(x) k(xy) \frac{dx}x
 
     in which :math:`f(x) = x^{-q} F(x)`, :math:`g(y) = y^q G(y)`, and
     :math:`k(t) = t^q K(t)`.
     The tilt parameter :math:`q` shifts power of :math:`x` between the input
     function and the kernel.
 
     Parameters
     ----------
     x : (Nin,) array_like
         log-evenly spaced input argument
     UK : callable
         Mellin transform of the kernel
-        .. math:: U_K(z) \equiv \int_0^\infty t^z K(t) \, \mathrm{d}t
+        .. math:: U_K(z) \equiv \int_0^\infty t^z K(t) dt
     q : float
-        power-law tilt, can be used to balance f at large and small x.
-        Avoid the singularities in UK
+        power-law tilt, can be used to balance :math:`f` at large and small
+        :math:`x`. Avoid the singularities in `UK`
     N : int, optional
         length of FFT, defaults to the smallest power of 2 that doubles the
-        length of x
+        length of `x`; the input function is padded symmetrically to this
+        length with extrapolations or zeros before convolution
     lowring : bool, optional
-        if True and N is even, set y according to the low-ringing condition,
-        otherwise
-        :math:`x_\mathrm{min} * y_\mathrm{max} = x_\mathrm{max} * y_\mathrm{min} = 1`
+        if True and `N` is even, set `y` according to the low-ringing
+        condition, otherwise see `xy`
+    xy : float, optional
+        reciprocal product :math:`x_{min} y_{max} = x_{max} y_{min}` if
+        `lowring` is False or `N` is odd
 
     Attributes
     ----------
     Nin : int
-        input length
+        (unpadded) input (and output) length
     x : (Nin,) ndarray
-        log-evenly spaced input argument
+        (unpadded) input argument
     y : (Nin,) ndarray
-        log-evenly spaced output argument
+        (unpadded) output argument
     _x_ : (N,) ndarray
         padded input argument
     _y_ : (N,) ndarray
         padded output argument
     prefac : array_like
-        a function of x (excluding the tilt factor :math:`x^{-q}` to be added
-        automatically) to multiply before the convolution.
-        Set it to convert the integral to the generic form
+        a function of `x` (excluding the tilt factor :math:`x^{-q}` to be added
+        automatically) to multiply before the convolution
     postfac : array_like
-        a function of y (excluding the tilt factor :math:`y^{-q}` to be added
-        automatically) to multiply after the convolution.
-        Set it to convert the integral to the generic form
+        a function of `y` (excluding the tilt factor :math:`y^{-q}` to be added
+        automatically) to multiply after the convolution
 
     Methods
     -------
     __call__
     matrix
     check
 
     Examples
     --------
     >>> x = numpy.logspace(-3, 3, num=60, endpoint=False)
-    >>> F = 1 / (1 + x*x)**1.5
+    >>> A = 1 / (1 + x*x)**1.5
     >>> H = mcfit.mcfit(x, mcfit.kernels.Mellin_BesselJ(0), q=1)
-    >>> y, G = H(x**2 * F) # x^2 factor to reduce it to the generic form
-    >>> Gexact = numpy.exp(-y)
-    >>> numpy.allclose(G, Gexact)
+    >>> y, B = H(x**2 * A)
+    >>> Bexact = numpy.exp(-y)
+    >>> numpy.allclose(B, Bexact)
 
     More conveniently, use the Hankel transform subclass
-    >>> y, G = mcfit.transforms.Hankel(x)(F)
+    >>> y, B = mcfit.transforms.Hankel(x)(A)
 
     Notes
     -----
     Caveats about q
 
     References
     ----------
     .. [1] J. D. Talman. Numerical Fourier and Bessel Transforms in Logarithmic Variables.
             Journal of Computational Physics, 29:35-48, October 1978.
     .. [2] A. J. S. Hamilton. Uncorrelated modes of the non-linear power spectrum.
             MNRAS, 312:257-284, February 2000.
     """
 
-    def __init__(self, x, UK, q, N=None, lowring=True, prefac=None, postfac=None):
+    def __init__(self, x, UK, q, N=None, lowring=True, xy=1):
         self.x = numpy.asarray(x)
         self.Nin = len(x)
         self.UK = UK
         self.q = q
         self.N = N
         self.lowring = lowring
+        self.xy = xy
+
         self._setup()
-        self.prefac = 1 if prefac is None else prefac
-        self.postfac = 1 if postfac is None else postfac
-        if prefac is not None or postfac is not None:
-            import warnings
-            msg = "prefac and postfac as parameters are deprecated. " \
-            "Use them as attributes instead. See cosmology.xi2P.__init__ " \
-            "for an example. This gives the flexibility that postfac can " \
-            "be made a function of the output argument."
-            warnings.warn(msg, FutureWarning)
+        self.prefac = 1
+        self.postfac = 1
 
 
     @property
     def prefac(self):
         return self._prefac
 
     @prefac.setter
@@ -124,240 +120,272 @@
     def postfac(self, value):
         self._postfac = value
         self._yfac = self._postfac * self.y**(-self.q)
 
     @property
     def _x_(self):
         if not hasattr(self, "_x"):
-            self._x = self._pad(self.x, True, False)
+            self._x = self._pad(self.x, 0, True, False)
         return self._x
 
     @property
     def _y_(self):
         if not hasattr(self, "_y"):
-            self._y = self._pad(self.y, True, True)
+            self._y = self._pad(self.y, 0, True, True)
         return self._y
 
 
     def _setup(self):
-        """Validate x, set N and y, and compute :math:`u_m`.
-        """
         if self.Nin < 2:
             raise ValueError("input length too short")
         Delta = numpy.log(self.x[-1] / self.x[0]) / (self.Nin - 1)
         if not numpy.allclose(self.x[1:] / self.x[:-1], numpy.exp(Delta), rtol=1e-3):
             raise ValueError("input not log-evenly spaced")
 
         if self.N is None:
             folds = int(numpy.ceil(numpy.log2(self.Nin))) + 1
             self.N = 2**folds
         if self.N < self.Nin:
             raise ValueError("total length shorter than input length")
 
-        lnxy = 0 # = lnxmin + lnymax = lnxmax + lnymin
+        lnxy = numpy.log(self.xy)
         if self.lowring and self.N % 2 == 0:
             lnxy = Delta / numpy.pi * numpy.angle(self.UK(self.q + 1j * numpy.pi / Delta))
         self.y = numpy.exp(lnxy - Delta) / self.x[::-1]
 
         m = numpy.arange(0, self.N//2 + 1)
         self._u = self.UK(self.q + 2j * numpy.pi / self.N / Delta * m)
         self._u *= numpy.exp(-2j * numpy.pi * lnxy / self.N / Delta * m)
 
         # following is unnecessary because hfft ignores the imag at Nyquist anyway
         #if not self.lowring and self.N % 2 == 0:
         #    self._u[self.N//2] = self._u[self.N//2].real
 
 
-    def __call__(self, F, extrap=True, interp=False):
+    def __call__(self, F, axis=-1, extrap=True, keeppads=False):
         """Evaluate the integral.
 
         Parameters
         ----------
-        F : (Nin,) array_like
-            input function, internally padded symmetrically to length N with
-            power-law extrapolations or zeros
+        F : (..., Nin, ...) array_like
+            input function
+        axis : int, optional
+            axis along which to integrate
         extrap : bool or 2-tuple of bools, optional
-            whether to extrapolate F with power laws or to just pad with zeros;
-            for a tuple, the two elements are for the left and right pads
-        interp : bool, optional
-            when True return an interpolant computed using padded input,
-            otherwise return unpadded arrays
+            whether to extrapolate `F` with power laws or to pad it with zeros,
+            to length `N`, before convolution; for a tuple, the two elements
+            are for the left and right pads
+        keeppads : bool, optional
+            whether to keep the padding in the output
 
         Returns
         -------
-        y : (Nin,) ndarray
-            log-evenly spaced output argument, unpadded
-        G : (Nin,) ndarray
-            output function, unpadded
-        Gy : scipy.interpolate.CubicSpline
-            output interpolant computed using padded input
+        y : (Nin,) or (N,) ndarray
+            log-evenly spaced output argument
+        G : (..., Nin, ...) or (..., N, ...) ndarray
+            output function
+
+        Notes
+        -----
+        `y`, and `G` are unpadded by default. Pads can be kept if `keeppads` is
+        set to True.
         """
-        if len(F) != self.Nin:
-            raise ValueError("lengths of input function and argument must match")
 
-        f = self._xfac * F
-        f = self._pad(f, extrap, False)
+        F = numpy.asarray(F)
+
+        to_axis = [1] * F.ndim
+        to_axis[axis] = -1
+
+        f = self._xfac.reshape(to_axis) * F
+        f = self._pad(f, axis, extrap, False)
 
         # convolution
-        f = numpy.fft.rfft(f) # f(x_n) -> f_m
-        g = f * self._u # f_m -> g_m
-        g = numpy.fft.hfft(g, n=self.N) / self.N # g_m -> g(y_n)
-
-        if not interp:
-            g = self._unpad(g, True)
-            G = self._yfac * g
+        f = numpy.fft.rfft(f, axis=axis) # f(x_n) -> f_m
+        g = f * self._u.reshape(to_axis) # f_m -> g_m
+        g = numpy.fft.hfft(g, n=self.N, axis=axis) / self.N # g_m -> g(y_n)
+
+        if not keeppads:
+            g = self._unpad(g, axis, True)
+            G = self._yfac.reshape(to_axis) * g
             return self.y, G
         else:
-            _G_ = self._pad(self._yfac, True, True) * g
-            from scipy.interpolate import CubicSpline
-            Gy = CubicSpline(self._y_, _G_)
-            return Gy
+            _G_ = self._pad(self._yfac, 0, True, True).reshape(to_axis) * g
+            return self._y_, _G_
 
 
-    def matrix(self, full=False):
+    def matrix(self, full=False, keeppads=True):
         """Return matrix form of the integral transform.
 
         Parameters
         ----------
         full : bool, optional
             when False return two vector factors and convolution matrix
             separately, otherwise return full transformation matrix
+        keeppads : bool, optional
+            whether to keep the padding in the output
 
         Returns
         -------
         If full is False, output separately
-        a : (1, N) ndarray
-            "After" factor, function of y including the `postfac` and the
+        a : (1, N) or (1, Nin) ndarray
+            "After" factor, function of `y` including the `postfac` and the
             power-law tilt
-        b : (N,) ndarray
-            "Before" factor, function of x including the `prefac` and the
+        b : (N,) or (Nin,) ndarray
+            "Before" factor, function of `x` including the `prefac` and the
             power-law tilt
-        C : (N, N) ndarray
+        C : (N, N) or (Nin, Nin) ndarray
             Convolution matrix, circulant
 
-        Otherwise, output the full matrix, combining a, b, and C
-        M : (N, N) ndarray
+        Otherwise, output the full matrix, combining `a`, `b`, and `C`
+        M : (N, N) or (Nin, Nin) ndarray
             Full transformation matrix, `M = a * C * b`
 
         Notes
         -----
-        M, a, b, and C are padded.
+        `M`, `a`, `b`, and `C` are padded by default. Pads can be discarded if
+        `keeppads` is set to False.
 
         This is not meant for evaluation with matrix multiplication but in case
         one is interested in the tranformation itself.
 
-        When N is even and lowing is False, :math:`C C^{-1}` and :math:`M
+        When `N` is even and `lowring` is False, :math:`C C^{-1}` and :math:`M
         M^{-1}` can deviate from the identity matrix because the imaginary part
         of the Nyquist modes are dropped.
 
         The convolution matrix is a circulant matrix, with its first row and
         first column being the Fourier transform of :math:`u_m`.
         Indeed :math:`u_m` are the eigenvalues of the convolution matrix, that
         are diagonalized by the DFT matrix.
         Thus :math:`1/u_m` are the eigenvalues of the inverse convolution
         matrix.
         """
-        a = self._pad(self._yfac, True, True)[:, numpy.newaxis]
-        b = self._pad(self._xfac, True, False)
+
+        if keeppads:
+            a = self._pad(self._yfac, 0, True, True)
+            b = self._pad(self._xfac, 0, True, False)
+        else:
+            a = self._yfac.copy()
+            b = self._xfac.copy()
+        a = a.reshape(-1, 1)
+
         v = numpy.fft.hfft(self._u, n=self.N) / self.N
         idx = sum(numpy.ogrid[0:self.N, -self.N:0])
         C = v[idx] # follow scipy.linalg.{circulant,toeplitz,hankel}
+        if not keeppads:
+            C = self._unpad(C, 0, True)
+            C = self._unpad(C, 1, False)
+
         if not full:
             return a, b, C
         else:
             return a * C * b
 
 
-    def _pad(self, a, extrap, out):
+    def _pad(self, a, axis, extrap, out):
         """Pad an array with power-law extrapolations or zeros.
 
         Parameters
         ----------
-        a : (Nin,) ndarray
-            array to be padded to length N
+        a : (..., Nin, ...) ndarray
+            array to be padded to length `N`
+        axis : int
+            axis along which to pad
         extrap : bool or 2-tuple of bools
-            whether to extrapolate a with power laws or to just pad with zeros;
-            for a tuple, the two elements are for the left and right pads
+            whether to extrapolate `a` with power laws or to just pad with
+            zeros; for a tuple, the two elements are for the left and right
+            pads
         out : bool
-            pad the input when False, otherwise the output;
-            the two cases have their left and right pad sizes reversed
+            pad the output if True, otherwise the input; the two cases have
+            their left and right pad sizes reversed
         """
-        assert len(a) == self.Nin
 
-        if isinstance(extrap, bool):
-            _extrap = extrap_ = extrap
-        elif isinstance(extrap, tuple) and len(extrap) == 2 and \
-                all(isinstance(e, bool) for e in extrap):
-            _extrap, extrap_ = extrap
-        else:
-            raise TypeError("extrap neither one bool nor a tuple of two")
+        assert a.shape[axis] == self.Nin
+
+        to_axis = [1] * a.ndim
+        to_axis[axis] = -1
+
+        _extrap, extrap_ = extrap, extrap if numpy.isscalar(extrap) else extrap
 
         Npad = self.N - self.Nin
         if out:
             _Npad, Npad_ = Npad - Npad//2, Npad//2
         else:
             _Npad, Npad_ = Npad//2, Npad - Npad//2
         if _extrap:
-            _a = a[0] * (a[1] / a[0]) ** numpy.arange(-_Npad, 0)
+            start = numpy.take(a, [0], axis=axis)
+            ratio = numpy.take(a, [1], axis=axis) / start
+            exp = numpy.arange(-_Npad, 0).reshape(to_axis)
+            _a = start * ratio ** exp
         else:
-            _a = numpy.zeros(_Npad)
+            _a = numpy.zeros(a.shape[:axis] + (_Npad,) + a.shape[axis+1:])
         if extrap_:
-            a_ = a[-1] * (a[-1] / a[-2]) ** numpy.arange(1, Npad_ + 1)
+            start = numpy.take(a, [-1], axis=axis)
+            ratio = start / numpy.take(a, [-2], axis=axis)
+            exp = numpy.arange(1, Npad_ + 1).reshape(to_axis)
+            a_ = start * ratio ** exp
         else:
-            a_ = numpy.zeros(Npad_)
+            a_ = numpy.zeros(a.shape[:axis] + (Npad_,) + a.shape[axis+1:])
 
-        return numpy.concatenate((_a, a, a_))
+        return numpy.concatenate((_a, a, a_), axis=axis)
 
 
-    def _unpad(self, a, out):
+    def _unpad(self, a, axis, out):
         """Undo padding in an array.
 
         Parameters
         ----------
-        a : (N,) ndarray
-            array to be trimmed to length Nin
+        a : (..., N, ...) ndarray
+            array to be trimmed to length `Nin`
+        axis : int
+            axis along which to unpad
         out : bool
-            trim the output when True, otherwise the input;
-            the two cases have their left and right pad sizes reversed
+            trim the output if True, otherwise the input; the two cases have
+            their left and right pad sizes reversed
         """
-        assert len(a) == self.N
+
+        assert a.shape[axis] == self.N
 
         Npad = self.N - self.Nin
         if out:
             _Npad, Npad_ = Npad - Npad//2, Npad//2
         else:
             _Npad, Npad_ = Npad//2, Npad - Npad//2
 
-        return a[_Npad : self.N - Npad_]
+        return numpy.take(a, range(_Npad, self.N - Npad_), axis=axis)
 
 
     def check(self, F):
         """Rough sanity checks on the input function.
         """
+
+        assert F.ndim == 1, "checker only supports 1D"
+
         f = self._xfac * F
         fabs = numpy.abs(f)
 
         iQ1, iQ3 = numpy.searchsorted(fabs.cumsum(), numpy.array([0.25, 0.75]) * fabs.sum())
         assert 0 != iQ1 != iQ3 != self.Nin, "checker giving up"
         fabs_l = fabs[:iQ1].mean()
         fabs_m = fabs[iQ1:iQ3].mean()
         fabs_r = fabs[iQ3:].mean()
+
+        import warnings
         if fabs_l > fabs_m:
-            print("left wing seems heavy: {:.2g} vs {:.2g}, "
-                    "change tilt and mind convergence".format(fabs_l, fabs_m))
+            warnings.warn("left wing seems heavy: {:.2g} vs {:.2g}, "
+                    "change tilt and mind convergence".format(fabs_l, fabs_m), RuntimeWarning)
         if fabs_m < fabs_r:
-            print("right wing seems heavy: {:.2g} vs {:.2g}, "
-                    "change tilt and mind convergence".format(fabs_m, fabs_r))
+            warnings.warn("right wing seems heavy: {:.2g} vs {:.2g}, "
+                    "change tilt and mind convergence".format(fabs_m, fabs_r), RuntimeWarning)
 
         if fabs[0] > fabs[1]:
-            print("left tail may blow up: {:.2g} vs {:.2g}, "
-                    "change tilt or avoid extrapolation".format(f[0], f[1]))
+            warnings.warn("left tail may blow up: {:.2g} vs {:.2g}, "
+                    "change tilt or avoid extrapolation".format(f[0], f[1]), RuntimeWarning)
         if fabs[-2] < fabs[-1]:
-            print("right tail may blow up: {:.2g} vs {:.2g}, "
-                    "change tilt or avoid extrapolation".format(f[-2], f[-1]))
+            warnings.warn("right tail may blow up: {:.2g} vs {:.2g}, "
+                    "change tilt or avoid extrapolation".format(f[-2], f[-1]), RuntimeWarning)
 
         if f[0]*f[1] <= 0:
-            print("left tail looks wiggly: {:.2g} vs {:.2g}, "
-                    "avoid extrapolation".format(f[0], f[1]))
+            warnings.warn("left tail looks wiggly: {:.2g} vs {:.2g}, "
+                    "avoid extrapolation".format(f[0], f[1]), RuntimeWarning)
         if f[-2]*f[-1] <= 0:
-            print("right tail looks wiggly: {:.2g} vs {:.2g}, "
-                    "avoid extrapolation".format(f[-2], f[-1]))
+            warnings.warn("right tail looks wiggly: {:.2g} vs {:.2g}, "
+                    "avoid extrapolation".format(f[-2], f[-1]), RuntimeWarning)
```

### Comparing `mcfit-0.0.8/mcfit/tests/test_mcfit.py` & `mcfit-0.0.9/mcfit/tests/test_mcfit.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,16 +27,20 @@
     assert_allclose(M1 @ M2, numpy.eye(N), rtol=0, atol=1e-9)
     assert_allclose(M2 @ M1, numpy.eye(N), rtol=0, atol=1e-9)
 
 
 def test_pad():
     x = numpy.logspace(-3, 3, num=6, endpoint=False)
     _x_ = numpy.logspace(-6, 6, num=13, endpoint=True)
-    y, _y_ = 1/x[::-1], 1/_x_[::-1]
+    y = numpy.logspace(-3, 3, num=6, endpoint=False)
+    _y_ = numpy.logspace(-7, 5, num=13, endpoint=True)
 
-    H = Hankel(x, N=13)
+    H = Hankel(x, N=13, xy=1)
 
-    assert_allclose(H._pad(x, True, False), _x_)
-    assert_allclose(H._pad(y, True, True), _y_)
+    assert_allclose(H._x_, _x_)
+    assert_allclose(H._y_, _y_)
 
-    assert_allclose(H._unpad(_x_, False), x)
-    assert_allclose(H._unpad(_y_, True), y)
+    assert_allclose(H._pad(x, 0, True, False), _x_)
+    assert_allclose(H._pad(y, 0, True, True), _y_)
+
+    assert_allclose(H._unpad(_x_, 0, False), x)
+    assert_allclose(H._unpad(_y_, 0, True), y)
```

### Comparing `mcfit-0.0.8/mcfit/tests/test_transforms.py` & `mcfit-0.0.9/mcfit/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `mcfit-0.0.8/mcfit/transforms.py` & `mcfit-0.0.9/mcfit/transforms.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,128 +12,130 @@
 
 
 __all__ = ['Hankel', 'SphericalBessel', 'DoubleBessel', 'DoubleSphericalBessel',
             'FourierSine', 'FourierCosine', 'TophatSmooth', 'GaussSmooth']
 
 
 class Hankel(mcfit):
-    """Hankel transform pair
+    """Hankel transform pair.
     """
-    def __init__(self, x, nu=0, q=1, N=None, lowring=True):
+    def __init__(self, x, nu=0, q=1, **kwargs):
         self.nu = nu
         UK = kernels.Mellin_BesselJ(nu)
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x**2
 
 
 class SphericalBessel(mcfit):
-    """Spherical Bessel transform pair
+    """Spherical Bessel transform pair.
     """
-    def __init__(self, x, nu=0, q=1.5, N=None, lowring=True):
+    def __init__(self, x, nu=0, q=1.5, **kwargs):
         self.nu = nu
         UK = kernels.Mellin_SphericalBesselJ(nu)
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x**3
 
 
 class FourierSine(mcfit):
-    """Fourier sine transform pair
+    """Fourier sine transform pair.
     """
-    def __init__(self, x, q=0.5, N=None, lowring=True):
+    def __init__(self, x, q=0.5, **kwargs):
         UK = kernels.Mellin_FourierSine()
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x
 
 
 class FourierCosine(mcfit):
-    """Fourier cosine transform pair
+    """Fourier cosine transform pair.
     """
-    def __init__(self, x, q=0.5, N=None, lowring=True):
+    def __init__(self, x, q=0.5, **kwargs):
         UK = kernels.Mellin_FourierCosine()
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x
 
 
 class DoubleBessel(mcfit):
-    r"""Compute integrals with two Bessel functions
+    r"""Compute integrals with two Bessel functions.
+
     .. math:: G(y_1; \alpha) \equiv G(y_1, y_2=\alpha y_1)
                 = \int_0^\infty F(x) J_{\nu_1}(xy_1) J_{\nu_2}(xy_2) \,x\d x
 
     Parameters
     ----------
     alpha : float
         y2 / y1
     nu : float, optional
         default is 0
     nu1 : float, optional
         default is nu
     nu2 : float, optional
         default is nu
     """
-    def __init__(self, x, alpha, nu=0, nu1=None, nu2=None, q=None, N=None, lowring=True):
+    def __init__(self, x, alpha, nu=0, nu1=None, nu2=None, q=None, **kwargs):
         self.alpha = alpha
         if nu1 is None:
             nu1 = nu
         if nu2 is None:
             nu2 = nu
         self.nu1 = nu1
         self.nu2 = nu2
         UK = kernels.Mellin_DoubleBesselJ(alpha, nu1, nu2)
         if q is None:
             q = 1
             if alpha == 1:
                 q = 0.5
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x**2
 
 
 class DoubleSphericalBessel(mcfit):
-    r"""Compute integrals with two spherical Bessel functions
+    r"""Compute integrals with two spherical Bessel functions.
+
     .. math:: G(y_1; \alpha) \equiv G(y_1, y_2=\alpha y_1)
                 = \int_0^\infty F(x) j_{\nu_1}(xy_1) j_{\nu_2}(xy_2) \,x^2\d x
 
     Parameters
     ----------
     alpha : float
         y2 / y1
     nu : float, optional
         default is 0
     nu1 : float, optional
         default is nu
     nu2 : float, optional
         default is nu
     """
-    def __init__(self, x, alpha, nu=0, nu1=None, nu2=None, q=None, N=None, lowring=True):
+    def __init__(self, x, alpha, nu=0, nu1=None, nu2=None, q=None, **kwargs):
         self.alpha = alpha
         if nu1 is None:
             nu1 = nu
         if nu2 is None:
             nu2 = nu
         self.nu1 = nu1
         self.nu2 = nu2
         UK = kernels.Mellin_DoubleSphericalBesselJ(alpha, nu1, nu2)
         if q is None:
             q = 1.5
             if alpha == 1:
                 q = 1
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x**3
 
 
 class TophatSmooth(mcfit):
-    """Top-hat smoothing of a radial function
+    """Top-hat smoothing of a radial function.
     """
-    def __init__(self, x, d=3, q=0, N=None, lowring=True):
+    def __init__(self, x, d=3, q=0, **kwargs):
         self.d = d
         UK = kernels.Mellin_Tophat(d)
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x**d / (2**(d-1) * numpy.pi**(d/2) * gamma(d/2))
 
 
 class GaussSmooth(mcfit):
-    """Gaussian smoothing of a radial function
+    """Gaussian smoothing of a radial function.
     """
-    def __init__(self, x, d=3, q=0, N=None, lowring=True):
+    def __init__(self, x, d=3, q=0, **kwargs):
         self.d = d
         UK = kernels.Mellin_Gauss()
-        mcfit.__init__(self, x, UK, q, N=N, lowring=lowring)
+        mcfit.__init__(self, x, UK, q, **kwargs)
         self.prefac *= self.x**d / (2**(d-1) * numpy.pi**(d/2) * gamma(d/2))
```

### Comparing `mcfit-0.0.8/mcfit/kernels.py` & `mcfit-0.0.9/mcfit/kernels.py`

 * *Files identical despite different names*

