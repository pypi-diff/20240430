# Comparing `tmp/bpwave-0.0.2.tar.gz` & `tmp/bpwave-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpwave-0.0.2.tar", last modified: Tue Feb 27 09:28:19 2024, max compression
+gzip compressed data, was "bpwave-0.0.3.tar", last modified: Tue Apr 30 08:24:14 2024, max compression
```

## Comparing `bpwave-0.0.2.tar` & `bpwave-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-02-27 09:28:19.231721 bpwave-0.0.2/
--rw-rw-r--   0 repatt    (1000) repatt    (1000)      582 2024-02-27 09:26:15.000000 bpwave-0.0.2/CHANGELOG.rst
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     1070 2024-01-11 23:58:46.000000 bpwave-0.0.2/LICENSE.txt
--rw-rw-r--   0 repatt    (1000) repatt    (1000)       23 2024-01-11 23:58:46.000000 bpwave-0.0.2/MANIFEST.in
--rw-r--r--   0 repatt    (1000) repatt    (1000)     4231 2024-02-27 09:28:19.231721 bpwave-0.0.2/PKG-INFO
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     2511 2024-01-11 23:58:46.000000 bpwave-0.0.2/README.rst
-drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-02-27 09:28:19.231721 bpwave-0.0.2/bpwave/
--rw-rw-r--   0 repatt    (1000) repatt    (1000)       82 2024-01-11 23:58:46.000000 bpwave-0.0.2/bpwave/__init__.py
--rw-rw-r--   0 repatt    (1000) repatt    (1000)       22 2024-02-27 09:26:15.000000 bpwave-0.0.2/bpwave/_version.py
--rw-rw-r--   0 repatt    (1000) repatt    (1000)        0 2024-01-11 23:58:46.000000 bpwave-0.0.2/bpwave/py.typed
--rw-rw-r--   0 repatt    (1000) repatt    (1000)    30606 2024-02-27 09:26:15.000000 bpwave-0.0.2/bpwave/signal.py
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     1847 2024-01-11 23:58:46.000000 bpwave-0.0.2/bpwave/visu.py
-drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-02-27 09:28:19.231721 bpwave-0.0.2/bpwave.egg-info/
--rw-r--r--   0 repatt    (1000) repatt    (1000)     4231 2024-02-27 09:28:19.000000 bpwave-0.0.2/bpwave.egg-info/PKG-INFO
--rw-rw-r--   0 repatt    (1000) repatt    (1000)      372 2024-02-27 09:28:19.000000 bpwave-0.0.2/bpwave.egg-info/SOURCES.txt
--rw-rw-r--   0 repatt    (1000) repatt    (1000)        1 2024-02-27 09:28:19.000000 bpwave-0.0.2/bpwave.egg-info/dependency_links.txt
--rw-rw-r--   0 repatt    (1000) repatt    (1000)      130 2024-02-27 09:28:19.000000 bpwave-0.0.2/bpwave.egg-info/requires.txt
--rw-rw-r--   0 repatt    (1000) repatt    (1000)        7 2024-02-27 09:28:19.000000 bpwave-0.0.2/bpwave.egg-info/top_level.txt
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     1551 2024-01-11 23:58:46.000000 bpwave-0.0.2/pyproject.toml
--rw-rw-r--   0 repatt    (1000) repatt    (1000)       38 2024-02-27 09:28:19.231721 bpwave-0.0.2/setup.cfg
-drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-02-27 09:28:19.231721 bpwave-0.0.2/tests/
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     2858 2024-02-27 09:26:15.000000 bpwave-0.0.2/tests/test_cpindices.py
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     7314 2024-02-27 09:26:15.000000 bpwave-0.0.2/tests/test_signal.py
--rw-rw-r--   0 repatt    (1000) repatt    (1000)     5171 2024-02-27 09:26:15.000000 bpwave-0.0.2/tests/test_signal_slicing.py
+drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-04-30 08:24:14.513767 bpwave-0.0.3/
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     1121 2024-04-30 08:23:59.000000 bpwave-0.0.3/CHANGELOG.rst
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     1070 2024-04-14 19:29:12.000000 bpwave-0.0.3/LICENSE.txt
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)       23 2024-04-14 19:29:12.000000 bpwave-0.0.3/MANIFEST.in
+-rw-r--r--   0 repatt    (1000) repatt    (1000)     4770 2024-04-30 08:24:14.509767 bpwave-0.0.3/PKG-INFO
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     2511 2024-04-14 19:29:12.000000 bpwave-0.0.3/README.rst
+drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-04-30 08:24:14.509767 bpwave-0.0.3/bpwave/
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)      149 2024-04-30 08:23:59.000000 bpwave-0.0.3/bpwave/__init__.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)       22 2024-04-30 08:23:59.000000 bpwave-0.0.3/bpwave/_version.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)    10533 2024-04-30 08:23:59.000000 bpwave-0.0.3/bpwave/io.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)        0 2024-04-14 19:29:12.000000 bpwave-0.0.3/bpwave/py.typed
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)    34083 2024-04-30 08:23:59.000000 bpwave-0.0.3/bpwave/signal.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     3035 2024-04-30 08:23:59.000000 bpwave-0.0.3/bpwave/visu.py
+drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-04-30 08:24:14.509767 bpwave-0.0.3/bpwave.egg-info/
+-rw-r--r--   0 repatt    (1000) repatt    (1000)     4770 2024-04-30 08:24:14.000000 bpwave-0.0.3/bpwave.egg-info/PKG-INFO
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)      425 2024-04-30 08:24:14.000000 bpwave-0.0.3/bpwave.egg-info/SOURCES.txt
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)        1 2024-04-30 08:24:14.000000 bpwave-0.0.3/bpwave.egg-info/dependency_links.txt
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)      130 2024-04-30 08:24:14.000000 bpwave-0.0.3/bpwave.egg-info/requires.txt
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)        7 2024-04-30 08:24:14.000000 bpwave-0.0.3/bpwave.egg-info/top_level.txt
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     1551 2024-04-14 19:29:12.000000 bpwave-0.0.3/pyproject.toml
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)       38 2024-04-30 08:24:14.513767 bpwave-0.0.3/setup.cfg
+drwxrwxr-x   0 repatt    (1000) repatt    (1000)        0 2024-04-30 08:24:14.509767 bpwave-0.0.3/tests/
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     3265 2024-04-30 08:23:59.000000 bpwave-0.0.3/tests/test_chpoints.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     3584 2024-04-30 08:23:59.000000 bpwave-0.0.3/tests/test_cpindices.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     3234 2024-04-30 08:23:59.000000 bpwave-0.0.3/tests/test_io.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     7631 2024-04-30 08:23:59.000000 bpwave-0.0.3/tests/test_signal.py
+-rw-rw-r--   0 repatt    (1000) repatt    (1000)     5515 2024-04-30 08:23:59.000000 bpwave-0.0.3/tests/test_signal_slicing.py
```

### Comparing `bpwave-0.0.2/LICENSE.txt` & `bpwave-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpwave-0.0.2/PKG-INFO` & `bpwave-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpwave
-Version: 0.0.2
+Version: 0.0.3
 Summary: Blood pressure waveform processing toolbox
 Author-email: Répai Attila <repai.attila@hallgato.ppke.hu>
 Project-URL: Homepage, https://github.com/repat8/bpwave
 Project-URL: Issues, https://github.com/repat8/bpwave/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -119,14 +119,29 @@
     https://doi.org/10.13026/2hsy-t491.
 .. [PhysioNet] Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P. C.,
     Mark, R., ... & Stanley, H. E. (2000).
     PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research
     resource for complex physiologic signals. Circulation [Online]. 101 (23),
     pp. e215–e220.
 
+0.0.3 (2024-04-30)
+    Features:
+
+    * ``SignalReader`` base class and ``CsvReader``.
+    * ``Signal.plot``: grid on by default. New parameter ``t0``.
+    * ``to_csv``: simple CSV export
+    * ``ChPoints.plot``: plot independently of the containing signal.
+    * Slicing of ``ChPoints``, shifting indices with scalar (``+, -``)
+    * ``visu.plot_signal_slices``.
+
+    Fixes:
+
+    * ``Signal.__getitem__`` can no longer produce empty slices in ``Signal.slices``.
+    * ``Signal.slices`` validation error messages now contain the ``key``.
+
 0.0.2 (2024-02-27)
     Breaking changes:
 
     * ``Signal.copy``: arguments made keyword-only
 
     Features:
```

### Comparing `bpwave-0.0.2/README.rst` & `bpwave-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `bpwave-0.0.2/bpwave/signal.py` & `bpwave-0.0.3/bpwave/signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,79 +17,104 @@
 
 
 @_dc.dataclass(kw_only=True, frozen=True)
 class CpIndices:
     """Indices of the characteristic points of a single period of an ABP signal.
 
     Fields are optional; missing entries get negative value.
+
+    .. warning::
+        Please don't use negative (backwards) indexing, set values must be >= 0.
     """
 
     NAMES: _t.ClassVar[tuple[str, str, str, str, str, str]] = (
         "onset",
         "sys_peak",
         "refl_onset",
         "refl_peak",
         "dicr_notch",
         "dicr_peak",
     )
     """Index names in the same order as values in :meth:`to_array`."""
 
-    onset: int = -1
+    UNSET: _t.ClassVar[int] = -1
+    """Value representing unset value.
+
+    .. versionadded:: 0.0.3
+    """
+
+    onset: int = UNSET
     """Onset."""
 
-    sys_peak: int = -1
+    sys_peak: int = UNSET
     """Systolic peak."""
 
-    refl_onset: int = -1
+    refl_onset: int = UNSET
     """Onset of the reflected wave."""
 
-    refl_peak: int = -1
+    refl_peak: int = UNSET
     """Peak of the reflected wave."""
 
-    dicr_notch: int = -1
+    dicr_notch: int = UNSET
     """Dicrotic notch."""
 
-    dicr_peak: int = -1
+    dicr_peak: int = UNSET
     """Peak of the dicrotic wave."""
 
     def __post_init__(self):
-        if (self.to_array() < 0).all():
+        if (self.to_array() == self.UNSET).all():
             warnings.warn("None of the indices are set.")
 
-    def __sub__(self, shift: int) -> "CpIndices":
-        """Subtracts the same scalar from all indices."""
+    def __add__(self, shift: int) -> "CpIndices":
+        """Adds the same scalar to all indices.
+
+        A possible use case is when characteristic points are detected on a
+        shorter section of a signal, but the result needs to be trasferred to
+        the full length one.
+
+        .. versionadded:: 0.0.3
+        """
         return CpIndices(
             **{
-                n: shifted if (shifted := v - shift) >= 0 else -1
+                n: shifted if (shifted := v + shift) >= 0 else self.UNSET
                 for n, v in self.without_unset().items()
             }
         )
 
+    def __sub__(self, shift: int) -> "CpIndices":
+        """Subtracts the same scalar from all indices.
+
+        .. versionadded:: 0.0.3
+        """
+        return self + -shift
+
     def min(self) -> int:
         """Smallest set index."""
-        return min(self.without_unset().values(), default=-1)
+        return min(self.without_unset().values(), default=self.UNSET)
 
     def max(self) -> int:
         """Largest set index."""
-        return max(self.without_unset().values(), default=-1)
+        return max(self.without_unset().values(), default=self.UNSET)
 
     def clamped(self, start: int | None = None, stop: int | None = None) -> "CpIndices":
         """Keeps only the indices contained in the specified range."""
         start = start or 0
-        stop = stop or _np.iinfo(int).max
+        stop = _np.iinfo(int).max if stop is None else stop
         return CpIndices(
             **{
-                n: v if start <= v < stop else -1
+                n: v if start <= v < stop else self.UNSET
                 for n, v in self.without_unset().items()
             }
         )
 
     def without_unset(self) -> dict[str, int]:
         """Returns the existing points in a ``dict``."""
-        return {name: value for name, value in self.__dict__.items() if value >= 0}
+        return {
+            name: value for name, value in self.__dict__.items() if value != self.UNSET
+        }
 
     def to_array(self) -> _npt.NDArray[_np.int64]:
         """The points as numpy array."""
         return _np.array(_dc.astuple(self))
 
 
 @_dc.dataclass(kw_only=True, frozen=True)
@@ -104,14 +129,105 @@
 
     version: str
     """Version of the algorithm's package or ISO date in case of human."""
 
     params: dict[str, _t.Any]
     """Parameters of the algorithm, if any."""
 
+    def __getitem__(self, slc: slice) -> "ChPoints":
+        """Returns a copy with sliced ``indices``.
+
+        Negative (backwards) indices and setting ``step`` is not supported.
+
+        .. versionadded:: 0.0.3
+        """
+        if not isinstance(slc, slice):
+            raise NotImplementedError("Only slicing is supported")
+        if slc.step is not None:
+            raise NotImplementedError("Step is not yet supported")
+        if (slc.start is not None and slc.start < 0) or (
+            slc.stop is not None and slc.stop < 0
+        ):
+            raise NotImplementedError("Negative indices not supported")
+
+        start = slc.start or 0
+        stop = _np.iinfo(int).max if slc.stop is None else slc.stop
+
+        return _dc.replace(
+            self,
+            indices=[
+                ci.clamped(start, stop) - start
+                for ci in self.indices
+                if (
+                    (ci.min() >= start and ci.max() < stop)
+                    or (ci.min() <= start <= ci.max())
+                    or (ci.min() < stop <= ci.max())
+                )
+            ],
+        )
+
+    def __add__(self, shift: int) -> "ChPoints":
+        """Adds the same scalar to all indices.
+
+        A possible use case is when characteristic points are detected on a
+        shorter section of a signal, but the result needs to be trasferred to
+        the full length one.
+
+        .. versionadded:: 0.0.3
+        """
+        return _dc.replace(
+            self,
+            indices=[ci + shift for ci in self.indices],
+        )
+
+    def __sub__(self, shift: int) -> "ChPoints":
+        """Subtracts the same scalar from all indices.
+
+        .. versionadded:: 0.0.3
+        """
+        return self + -shift
+
+    def plot(
+        self,
+        ax: _plt.Axes,
+        *,
+        t: _np.ndarray,
+        y: _np.ndarray,
+        points: _t.Literal[True] | set[str] = True,
+    ) -> _plt.Axes:
+        """Plots the points on the given axes ``ax`` using timestamps ``t`` and
+        amplitudes ``y``.
+
+        The purpose of this method is to be able to plot characteristic points
+        independently of the containing signal, useful for previewing results
+        of a detection algorithm.
+
+        For plotting the own characteristic points of a signal, please use
+        :meth:`Signal.plot`.
+
+        .. warning::
+            This method doesn't validate ``t`` and ``y`` against the indices.
+
+        :param ax: subplot axes.
+        :param t: timestamps.
+        :param y: amplitudes.
+        :param points: set to filter points by name. ``True`` means all.
+        :return: the axes.
+
+        .. versionadded:: 0.0.3
+        """
+        all_indices = _col.defaultdict(list)
+        for ci in self.indices:
+            for name, index in ci.without_unset().items():
+                if points is True or name in points:
+                    all_indices[name].append(index)
+        for name, indices in all_indices.items():
+            ax.plot(t[indices], y[indices], "+", label=name)
+        return ax
+
 
 class _MarksProxy(_col.UserDict):
     def __init__(
         self,
         markers: _t.Union[dict[str, _ca.Iterable[int]], "_MarksProxy"],
         stop: int,
     ):
@@ -137,22 +253,22 @@
     ):
         self._stop = stop
         super().__init__(slices)
 
     def __setitem__(self, key: str, value: _ca.Sequence[slice]) -> None:
         for i, slc in enumerate(value):
             if slc.step is not None:
-                warnings.warn(f"Handling `step` is not implemented (value[{i}])")
+                warnings.warn(f"Handling `step` is not implemented (value[{key}][{i}])")
             if slc.start < 0 or slc.start >= self._stop:
                 raise ValueError(
-                    f"`value[{i}].start must be valid nonnegative index of `y`"
+                    f"`value[{key}][{i}].start must be valid nonnegative index of `y`"
                 )
             if slc.stop < 0 or slc.stop > self._stop:
                 raise ValueError(
-                    f"`value[{i}].stop must be valid nonnegative index of `y`"
+                    f"`value[{key}][{i}].stop must be valid nonnegative index of `y`"
                 )
         super().__setitem__(key, list(value))
 
 
 class _SignalIndexer:
     def __init__(self, signal: "Signal"):
         self._signal = signal
@@ -470,50 +586,36 @@
             start = slc.start if slc.start >= 0 else length + slc.start
 
         if slc.stop is None:
             stop = length
         else:
             stop = slc.stop if slc.stop >= 0 else length + slc.stop
 
+        def crop_slices(slcs) -> list[slice]:
+            cropped = [
+                slice(max(0, s.start - start), min(s.stop - start, stop - start))
+                for s in slcs
+                if start <= s.start < stop or start <= s.stop <= stop
+            ]
+            # Remove empty slices
+            cropped = [s for s in cropped if s.stop > s.start]
+            return cropped
+
         section = type(self)(
             y=self.y[slc],
             unit=self.unit,
             t=self.t[slc],  # intentionally the t property
             fs=None,
             label=self.label,
-            chpoints=(
-                None
-                if self.chpoints is None
-                else _dc.replace(
-                    self.chpoints,
-                    indices=[
-                        ci.clamped(start, stop) - start
-                        for ci in self.chpoints.indices
-                        if (
-                            (ci.min() >= start and ci.max() < stop)
-                            or (ci.min() <= start <= ci.max())
-                            or (ci.min() < stop <= ci.max())
-                        )
-                    ],
-                )
-            ),
+            chpoints=(None if self.chpoints is None else self.chpoints[start:stop]),
             marks={
                 name: v[(v >= start) & (v < stop)] - start
                 for name, v in self.marks.items()
             },
-            slices={
-                name: [
-                    slice(
-                        max(0, slc.start - start), min(slc.stop - start, stop - start)
-                    )
-                    for slc in slcs
-                    if start <= slc.start < stop or start <= slc.stop <= stop
-                ]
-                for name, slcs in self.slices.items()
-            },
+            slices={name: crop_slices(slcs) for name, slcs in self.slices.items()},
             meta=self.meta,
         )
         section._fs = self._fs
         section._t_from_fs = self._t_from_fs
         # ^ We don't want t to be recalculated from 0, as we want to preserve
         # the original timestamps.
 
@@ -662,59 +764,65 @@
         ax: _plt.Axes | None = None,
         *fmt_args,
         onsets: bool = True,
         points: bool | set[str] = True,
         marks: bool | set[str] = True,
         legend: str = "auto",
         title: str | None = None,
+        t0: float | None = None,
         **plot_kw,
     ) -> _plt.Axes:
         """Plots the signal.
 
         :param ax: target axes. If ``None``, a new figure is created.
         :param onsets: show onsets.
         :param points: show other points. ``True`` to plot all, ``set`` of names
             to filter (see :class:`CpIndices`).
         :param marks: show marks. ``True`` to plot all, ``set`` of names
             to filter.
         :param legend: ``auto``: show legend when needed,
             ``off``: don't show, ``outside``: move legend out of plot area.
         :param title: plot title.
+        :param t0: shift timestamps to start from ``t0``, without copying or
+            modifying the object (unlike :meth:`shift_t`).
+
+            .. versionadded:: 0.0.3
         :param fmt_args: line style and color shorthand for :func:`visu.plot_signal`.
         :param plot_kw: keyword arguments for :func:`visu.plot_signal`.
         :return: the axes object.
+
+        .. versionchanged:: 0.0.3
+            Grid is on by default.
         """
         if not ax:
             _, ax = _plt.subplots()
         assert ax  # Make mypy happy
 
         if self.label and "label" not in plot_kw:
             plot_kw = {"label": self.label, **plot_kw}
         has_legend = "label" in plot_kw
 
         _v.plot_signal(
             ax,
-            self.t,
+            self.t if t0 is None else self.t - self.t[0] + t0,
             self.y,
             *fmt_args,
             y_unit=self.unit,
             t_unit="s",
             **plot_kw,
         )
 
         if points and self.chpoints:
-            all_indices = _col.defaultdict(list)
-            for ci in self.chpoints.indices:
-                for name, index in ci.without_unset().items():
-                    if (points is True or name in points) and not (
-                        onsets and name == "onset"
-                    ):
-                        all_indices[name].append(index)
-            for name, indices in all_indices.items():
-                ax.plot(self.t[indices], self.y[indices], "+", label=name)
+            points_: bool | set[str]
+            if onsets:
+                points_ = set(CpIndices.NAMES)
+                points_ = points_ - {"onset"}
+            else:
+                points_ = points
+            self.chpoints.plot(ax, t=self.t, y=self.y, points=points_)
             has_legend = True
         if onsets and self.chpoints and len(self.onsets):
             ax.plot(
                 self.t_onsets,
                 self.y[self.onsets],
                 "r+",
                 label=f"onset ({self.chpoints.alg})",
@@ -745,14 +853,17 @@
         if legend != "off" and has_legend:
             if legend == "outside":
                 ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
             else:
                 ax.legend()
         if title:
             ax.set(title=title)
+
+        ax.grid(True)
+
         return ax
 
     def to_hdf(self, group: h5py.Group) -> None:
         """Saves contents to a HDF5 file or a group thereof.
 
         :param group: :class:`h5py.File` or :class:`h5py.Group`
         """
```

### Comparing `bpwave-0.0.2/bpwave.egg-info/PKG-INFO` & `bpwave-0.0.3/bpwave.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpwave
-Version: 0.0.2
+Version: 0.0.3
 Summary: Blood pressure waveform processing toolbox
 Author-email: Répai Attila <repai.attila@hallgato.ppke.hu>
 Project-URL: Homepage, https://github.com/repat8/bpwave
 Project-URL: Issues, https://github.com/repat8/bpwave/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -119,14 +119,29 @@
     https://doi.org/10.13026/2hsy-t491.
 .. [PhysioNet] Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P. C.,
     Mark, R., ... & Stanley, H. E. (2000).
     PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research
     resource for complex physiologic signals. Circulation [Online]. 101 (23),
     pp. e215–e220.
 
+0.0.3 (2024-04-30)
+    Features:
+
+    * ``SignalReader`` base class and ``CsvReader``.
+    * ``Signal.plot``: grid on by default. New parameter ``t0``.
+    * ``to_csv``: simple CSV export
+    * ``ChPoints.plot``: plot independently of the containing signal.
+    * Slicing of ``ChPoints``, shifting indices with scalar (``+, -``)
+    * ``visu.plot_signal_slices``.
+
+    Fixes:
+
+    * ``Signal.__getitem__`` can no longer produce empty slices in ``Signal.slices``.
+    * ``Signal.slices`` validation error messages now contain the ``key``.
+
 0.0.2 (2024-02-27)
     Breaking changes:
 
     * ``Signal.copy``: arguments made keyword-only
 
     Features:
```

### Comparing `bpwave-0.0.2/pyproject.toml` & `bpwave-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bpwave-0.0.2/tests/test_cpindices.py` & `bpwave-0.0.3/tests/test_cpindices.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,35 +53,59 @@
         dicr_peak=170 - offset,
     )
 
 
 def test__cpindices__sub__out_of_range(cpindices_all_set: CpIndices) -> None:
     offset = 120
     assert cpindices_all_set - offset == CpIndices(
-        onset=-1,
+        onset=CpIndices.UNSET,
         sys_peak=0,
         refl_onset=140 - offset,
         refl_peak=150 - offset,
         dicr_notch=160 - offset,
         dicr_peak=170 - offset,
     )
 
 
 def test__cpindices__sub__unset(cpindices_with_unset: CpIndices) -> None:
     offset = 10
     assert cpindices_with_unset - offset == CpIndices(
         onset=100 - offset,
         sys_peak=120 - offset,
-        refl_onset=-1,
-        refl_peak=-1,
+        refl_onset=CpIndices.UNSET,
+        refl_peak=CpIndices.UNSET,
         dicr_notch=160 - offset,
         dicr_peak=170 - offset,
     )
 
 
+def test__cpindices__add__in_range(cpindices_all_set: CpIndices) -> None:
+    offset = 10
+    assert cpindices_all_set + offset == CpIndices(
+        onset=100 + offset,
+        sys_peak=120 + offset,
+        refl_onset=140 + offset,
+        refl_peak=150 + offset,
+        dicr_notch=160 + offset,
+        dicr_peak=170 + offset,
+    )
+
+
+def test__cpindices__add__unset(cpindices_with_unset: CpIndices) -> None:
+    offset = 10
+    assert cpindices_with_unset + offset == CpIndices(
+        onset=100 + offset,
+        sys_peak=120 + offset,
+        refl_onset=CpIndices.UNSET,
+        refl_peak=CpIndices.UNSET,
+        dicr_notch=160 + offset,
+        dicr_peak=170 + offset,
+    )
+
+
 def test__cpindices__without_unset(cpindices_with_unset: CpIndices) -> None:
     assert cpindices_with_unset.without_unset() == {
         "onset": 100,
         "sys_peak": 120,
         "dicr_notch": 160,
         "dicr_peak": 170,
     }
```

### Comparing `bpwave-0.0.2/tests/test_signal.py` & `bpwave-0.0.3/tests/test_signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,19 +176,24 @@
 
 @pytest.mark.human
 def test__signal__plot(simple_signal: Signal) -> None:
     with visu.figure(nrows=4, title="test__signal__plot", figsize=(5, 10)) as (
         _,
         axes,
     ):
+        axes = axes.ravel()
         simple_signal.plot(axes[0], title="all on")
         simple_signal.plot(axes[1], title="onsets off", onsets=False)
         simple_signal.plot(axes[2], title="points off", points=False)
         simple_signal.plot(
-            axes[3], title="filtered points", points={"sys_peak"}, onsets=False
+            axes[3],
+            title="filtered points, t0=10",
+            points={"sys_peak"},
+            onsets=False,
+            t0=10,
         )
     plt.show()
 
 
 def test__signal__hdf__t_from_fs_has_segmentation(
     simple_signal: Signal,
     out_folder: pl.Path,
@@ -203,7 +208,15 @@
     assert s_loaded.label == simple_signal.label
     assert s_loaded.unit == simple_signal.unit
     assert s_loaded.t_from_fs
     assert s_loaded.chpoints == simple_signal.chpoints
     assert s_loaded.marks == simple_signal.marks
     assert s_loaded.slices == simple_signal.slices
     assert s_loaded.meta == simple_signal.meta
+
+
+def test__signal__repr(simple_signal: Signal) -> None:
+    assert repr(simple_signal) == "<Signal of 9 values>"
+
+
+def test__signal__str(simple_signal: Signal) -> None:
+    assert str(simple_signal) == "<Signal of 9 values>"
```

### Comparing `bpwave-0.0.2/tests/test_signal_slicing.py` & `bpwave-0.0.3/tests/test_signal_slicing.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,26 @@
         version="0",
         indices=[
             CpIndices(onset=0, sys_peak=2),
         ],
     )
 
 
+def test__signal__getitem__empty_slice_removed() -> None:
+    s = Signal(
+        y=np.ones(30),
+        fs=30,
+        slices={"test": [slice(5, 10), slice(10, 15), slice(15, 20)]},
+    )
+    s2 = s[10:15]
+    assert s2.slices["test"] == [slice(0, 5)]
+    s2 = s[9:16]
+    assert s2.slices["test"] == [slice(0, 1), slice(1, 6), slice(6, 7)]
+
+
 def test__signal__by_t__start_stop(bp_signal: Signal) -> None:
     section = bp_signal.by_t[2.0:3.5]  # type: ignore[misc]
     assert np.isclose(section.t[0], 2.0, atol=1 / section.fs)
     assert np.isclose(section.t[-1], 3.5, atol=1 / section.fs)
 
 
 def test__signal__by_t__start(bp_signal: Signal) -> None:
```

