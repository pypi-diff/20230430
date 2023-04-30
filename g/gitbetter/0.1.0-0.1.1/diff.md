# Comparing `tmp/gitbetter-0.1.0.tar.gz` & `tmp/gitbetter-0.1.1.tar.gz`

## Comparing `gitbetter-0.1.0.tar` & `gitbetter-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.1.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.1.0/docs/index.html
--rw-r--r--   0        0        0    55575 2020-02-02 00:00:00.000000 gitbetter-0.1.0/docs/search.js
--rw-r--r--   0        0        0   130318 2020-02-02 00:00:00.000000 gitbetter-0.1.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   227629 2020-02-02 00:00:00.000000 gitbetter-0.1.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.1.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 gitbetter-0.1.0/src/gitbetter/git.py
--rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 gitbetter-0.1.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 gitbetter-0.1.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 gitbetter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 gitbetter-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/index.html
+-rw-r--r--   0        0        0    55399 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/search.js
+-rw-r--r--   0        0        0   130318 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   227735 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.1.1/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 gitbetter-0.1.1/src/gitbetter/git.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 gitbetter-0.1.1/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 gitbetter-0.1.1/README.md
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 gitbetter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 gitbetter-0.1.1/PKG-INFO
```

### Comparing `gitbetter-0.1.0/docs/gitbetter.html` & `gitbetter-0.1.1/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.0/docs/search.js` & `gitbetter-0.1.1/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -939,15 +939,15 @@
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.recurse_files",
         "modulename": "gitbetter.gitbetter",
         "qualname": "recurse_files",
         "kind": "function",
         "doc": "<p></p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">filenames</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]</span>:</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">filenames</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.files_postparser",
         "modulename": "gitbetter.gitbetter",
         "qualname": "files_postparser",
         "kind": "function",
         "doc": "<p></p>\n",
```

### Comparing `gitbetter-0.1.0/docs/gitbetter/git.html` & `gitbetter-0.1.1/docs/gitbetter/git.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.0/docs/gitbetter/gitbetter.html` & `gitbetter-0.1.1/docs/gitbetter/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -239,23 +239,23 @@
 </span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
 </span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
 </span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
 </span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">]:</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">filenames</span><span class="p">:</span>
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
 </span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">))</span>
 </span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
 </span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;WARNING: Could not find any files with name </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">])</span>
 </span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span>
 </span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">return</span> <span class="n">files</span>
 </span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
 </span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
 </span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="k">def</span> <span class="nf">files_postparser</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
 </span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">:</span>
@@ -569,29 +569,29 @@
 
                 </section>
                 <section id="recurse_files">
                             <input id="recurse_files-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">recurse_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span> <span class="o">|</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]</span>:</span></span>
+        <span class="name">recurse_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="recurse_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#recurse_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="recurse_files-80"><a href="#recurse_files-80"><span class="linenos">80</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">]:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="recurse_files-80"><a href="#recurse_files-80"><span class="linenos">80</span></a><span class="k">def</span> <span class="nf">recurse_files</span><span class="p">(</span><span class="n">filenames</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="recurse_files-81"><a href="#recurse_files-81"><span class="linenos">81</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="recurse_files-82"><a href="#recurse_files-82"><span class="linenos">82</span></a>    <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">filenames</span><span class="p">:</span>
 </span><span id="recurse_files-83"><a href="#recurse_files-83"><span class="linenos">83</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
 </span><span id="recurse_files-84"><a href="#recurse_files-84"><span class="linenos">84</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">))</span>
 </span><span id="recurse_files-85"><a href="#recurse_files-85"><span class="linenos">85</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
 </span><span id="recurse_files-86"><a href="#recurse_files-86"><span class="linenos">86</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;WARNING: Could not find any files with name </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="recurse_files-87"><a href="#recurse_files-87"><span class="linenos">87</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="recurse_files-88"><a href="#recurse_files-88"><span class="linenos">88</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="recurse_files-88"><a href="#recurse_files-88"><span class="linenos">88</span></a>                <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">])</span>
 </span><span id="recurse_files-89"><a href="#recurse_files-89"><span class="linenos">89</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="recurse_files-90"><a href="#recurse_files-90"><span class="linenos">90</span></a>            <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span>
 </span><span id="recurse_files-91"><a href="#recurse_files-91"><span class="linenos">91</span></a>    <span class="k">return</span> <span class="n">files</span>
 </span></pre></div>
```

#### html2text {}

```diff
@@ -127,24 +127,24 @@
 _73        help=""" Delete the remote and remote-tracking branches along with
 the local branch.
 _74        By default only the local branch is deleted.""",
 _75    )
 _76    return parser
 _77
 _78
-_79def recurse_files(filenames: list[str]) -> list[str | Pathier]:
+_79def recurse_files(filenames: list[str]) -> list[str]:
 _80    files = []
 _81    for filename in filenames:
 _82        if not Pathier(filename).exists():
 _83            results = list(Pathier.cwd().rglob(f"{filename}"))
 _84            if not results:
 _85                print(f"WARNING: Could not find any files with name
 {filename}")
 _86            else:
-_87                files.extend(results)
+_87                files.extend([str(result) for result in results])
 _88        else:
 _89            files.append(filename)
 _90    return files
 _91
 _92
 _93def files_postparser(args: Namespace) -> Namespace:
 _94    if args.recursive:
@@ -406,26 +406,25 @@
 73        action="store_true",
 74        help=""" Delete the remote and remote-tracking branches along with
 the local branch.
 75        By default only the local branch is deleted.""",
 76    )
 77    return parser
   ⁰
-def recurse_files(filenames: list[str]) -> list[str | pathier.pathier.Pathier]:
-View Source
-80def recurse_files(filenames: list[str]) -> list[str | Pathier]:
+def recurse_files(filenames: list[str]) -> list[str]: View Source
+80def recurse_files(filenames: list[str]) -> list[str]:
 81    files = []
 82    for filename in filenames:
 83        if not Pathier(filename).exists():
 84            results = list(Pathier.cwd().rglob(f"{filename}"))
 85            if not results:
 86                print(f"WARNING: Could not find any files with name
 {filename}")
 87            else:
-88                files.extend(results)
+88                files.extend([str(result) for result in results])
 89        else:
 90            files.append(filename)
 91    return files
   ⁰
 def files_postparser(args: argshell.argshell.Namespace) -
 > argshell.argshell.Namespace: View Source
 94def files_postparser(args: Namespace) -> Namespace:
```

### Comparing `gitbetter-0.1.0/src/gitbetter/git.py` & `gitbetter-0.1.1/src/gitbetter/git.py`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.0/src/gitbetter/gitbetter.py` & `gitbetter-0.1.1/src/gitbetter/gitbetter.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,23 +72,23 @@
         action="store_true",
         help=""" Delete the remote and remote-tracking branches along with the local branch.
         By default only the local branch is deleted.""",
     )
     return parser
 
 
-def recurse_files(filenames: list[str]) -> list[str | Pathier]:
+def recurse_files(filenames: list[str]) -> list[str]:
     files = []
     for filename in filenames:
         if not Pathier(filename).exists():
             results = list(Pathier.cwd().rglob(f"{filename}"))
             if not results:
                 print(f"WARNING: Could not find any files with name {filename}")
             else:
-                files.extend(results)
+                files.extend([str(result) for result in results])
         else:
             files.append(filename)
     return files
 
 
 def files_postparser(args: Namespace) -> Namespace:
     if args.recursive:
```

### Comparing `gitbetter-0.1.0/LICENSE.txt` & `gitbetter-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.0/README.md` & `gitbetter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.0/pyproject.toml` & `gitbetter-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,66 +5,66 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e31 2e30 220d  rsion = "0.1.0".
+000000b0: 7273 696f 6e20 3d20 2230 2e31 2e31 220d  rsion = "0.1.1".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
-000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
-000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
-000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
-00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
-00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
-00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords = 
-00000130: 5b22 6769 7422 2c20 2273 6865 6c6c 222c  ["git", "shell",
-00000140: 2022 636c 6922 2c20 2274 6572 6d69 6e61   "cli", "termina
-00000150: 6c22 2c20 2263 6f6d 6d69 7422 5d0d 0a63  l", "commit"]..c
-00000160: 6c61 7373 6966 6965 7273 203d 205b 0d0a  lassifiers = [..
-00000170: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
-00000180: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000190: 686f 6e20 3a3a 2033 222c 0d0a 2020 2020  hon :: 3",..    
-000001a0: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
-000001b0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000001c0: 4c69 6365 6e73 6522 2c0d 0a20 2020 2022  License",..    "
-000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001f0: 6e74 222c 0d0a 2020 2020 5d0d 0a0d 0a5b  nt",..    ]....[
-00000200: 5b70 726f 6a65 6374 2e61 7574 686f 7273  [project.authors
-00000210: 5d5d 0d0a 6e61 6d65 203d 2022 4d61 7474  ]]..name = "Matt
-00000220: 204d 616e 6573 220d 0a65 6d61 696c 203d   Manes"..email =
-00000230: 2022 6d61 7474 6d61 6e65 7340 706d 2e6d   "mattmanes@pm.m
-00000240: 6522 0d0a 0d0a 5b70 726f 6a65 6374 2e75  e"....[project.u
-00000250: 726c 735d 0d0a 2248 6f6d 6570 6167 6522  rls].."Homepage"
-00000260: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-00000270: 7562 2e63 6f6d 2f6d 6174 742d 6d61 6e65  ub.com/matt-mane
-00000280: 732f 6769 7462 6574 7465 7222 0d0a 2244  s/gitbetter".."D
-00000290: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
-000002a0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000002b0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f67  com/matt-manes/g
-000002c0: 6974 6265 7474 6572 2f74 7265 652f 6d61  itbetter/tree/ma
-000002d0: 696e 2f64 6f63 7322 0d0a 2253 6f75 7263  in/docs".."Sourc
-000002e0: 6520 636f 6465 2220 3d20 2268 7474 7073  e code" = "https
-000002f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
-00000300: 7474 2d6d 616e 6573 2f67 6974 6265 7474  tt-manes/gitbett
-00000310: 6572 2f74 7265 652f 6d61 696e 2f73 7263  er/tree/main/src
-00000320: 2f67 6974 6265 7474 6572 220d 0a0d 0a5b  /gitbetter"....[
-00000330: 746f 6f6c 2e70 7974 6573 742e 696e 695f  tool.pytest.ini_
-00000340: 6f70 7469 6f6e 735d 0d0a 6164 646f 7074  options]..addopt
-00000350: 7320 3d20 5b0d 0a20 2020 2022 2d2d 696d  s = [..    "--im
-00000360: 706f 7274 2d6d 6f64 653d 696d 706f 7274  port-mode=import
-00000370: 6c69 6222 2c0d 0a20 2020 205d 0d0a 7079  lib",..    ]..py
-00000380: 7468 6f6e 7061 7468 203d 2022 7372 6322  thonpath = "src"
-00000390: 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463 682e  ....[tool.hatch.
-000003a0: 6275 696c 642e 7461 7267 6574 732e 7364  build.targets.sd
-000003b0: 6973 745d 0d0a 6578 636c 7564 6520 3d20  ist]..exclude = 
-000003c0: 5b0d 0a20 2020 2022 2e63 6f76 6572 6167  [..    ".coverag
-000003d0: 6522 2c0d 0a20 2020 2022 2e70 7974 6573  e",..    ".pytes
-000003e0: 745f 6361 6368 6522 2c0d 0a20 2020 2022  t_cache",..    "
-000003f0: 2e76 7363 6f64 6522 2c0d 0a20 2020 2022  .vscode",..    "
-00000400: 7465 7374 7322 2c0d 0a20 2020 2022 2e67  tests",..    ".g
-00000410: 6974 6967 6e6f 7265 220d 0a20 2020 205d  itignore"..    ]
-00000420: 0d0a 5b70 726f 6a65 6374 2e73 6372 6970  ..[project.scrip
-00000430: 7473 5d0d 0a67 6974 6265 7474 6572 203d  ts]..gitbetter =
-00000440: 2022 6769 7462 6574 7465 722e 6769 7462   "gitbetter.gitb
-00000450: 6574 7465 723a 6d61 696e 220d 0a         etter:main"..
+000000d0: 203d 2022 3e3d 332e 3922 0d0a 6465 7065   = ">=3.9"..depe
+000000e0: 6e64 656e 6369 6573 203d 205b 2261 7267  ndencies = ["arg
+000000f0: 7368 656c 6c22 2c20 2270 6174 6869 6572  shell", "pathier
+00000100: 222c 2022 7079 7465 7374 225d 0d0a 7265  ", "pytest"]..re
+00000110: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
+00000120: 6422 0d0a 6b65 7977 6f72 6473 203d 205b  d"..keywords = [
+00000130: 2267 6974 222c 2022 7368 656c 6c22 2c20  "git", "shell", 
+00000140: 2263 6c69 222c 2022 7465 726d 696e 616c  "cli", "terminal
+00000150: 222c 2022 636f 6d6d 6974 225d 0d0a 636c  ", "commit"]..cl
+00000160: 6173 7369 6669 6572 7320 3d20 5b0d 0a20  assifiers = [.. 
+00000170: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+00000180: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000190: 6f6e 203a 3a20 3322 2c0d 0a20 2020 2022  on :: 3",..    "
+000001a0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001b0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001c0: 6963 656e 7365 222c 0d0a 2020 2020 224f  icense",..    "O
+000001d0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001e0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000001f0: 7422 2c0d 0a20 2020 205d 0d0a 0d0a 5b5b  t",..    ]....[[
+00000200: 7072 6f6a 6563 742e 6175 7468 6f72 735d  project.authors]
+00000210: 5d0d 0a6e 616d 6520 3d20 224d 6174 7420  ]..name = "Matt 
+00000220: 4d61 6e65 7322 0d0a 656d 6169 6c20 3d20  Manes"..email = 
+00000230: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
+00000240: 220d 0a0d 0a5b 7072 6f6a 6563 742e 7572  "....[project.ur
+00000250: 6c73 5d0d 0a22 486f 6d65 7061 6765 2220  ls].."Homepage" 
+00000260: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+00000270: 622e 636f 6d2f 6d61 7474 2d6d 616e 6573  b.com/matt-manes
+00000280: 2f67 6974 6265 7474 6572 220d 0a22 446f  /gitbetter".."Do
+00000290: 6375 6d65 6e74 6174 696f 6e22 203d 2022  cumentation" = "
+000002a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002b0: 6f6d 2f6d 6174 742d 6d61 6e65 732f 6769  om/matt-manes/gi
+000002c0: 7462 6574 7465 722f 7472 6565 2f6d 6169  tbetter/tree/mai
+000002d0: 6e2f 646f 6373 220d 0a22 536f 7572 6365  n/docs".."Source
+000002e0: 2063 6f64 6522 203d 2022 6874 7470 733a   code" = "https:
+000002f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+00000300: 742d 6d61 6e65 732f 6769 7462 6574 7465  t-manes/gitbette
+00000310: 722f 7472 6565 2f6d 6169 6e2f 7372 632f  r/tree/main/src/
+00000320: 6769 7462 6574 7465 7222 0d0a 0d0a 5b74  gitbetter"....[t
+00000330: 6f6f 6c2e 7079 7465 7374 2e69 6e69 5f6f  ool.pytest.ini_o
+00000340: 7074 696f 6e73 5d0d 0a61 6464 6f70 7473  ptions]..addopts
+00000350: 203d 205b 0d0a 2020 2020 222d 2d69 6d70   = [..    "--imp
+00000360: 6f72 742d 6d6f 6465 3d69 6d70 6f72 746c  ort-mode=importl
+00000370: 6962 222c 0d0a 2020 2020 5d0d 0a70 7974  ib",..    ]..pyt
+00000380: 686f 6e70 6174 6820 3d20 2273 7263 220d  honpath = "src".
+00000390: 0a0d 0a5b 746f 6f6c 2e68 6174 6368 2e62  ...[tool.hatch.b
+000003a0: 7569 6c64 2e74 6172 6765 7473 2e73 6469  uild.targets.sdi
+000003b0: 7374 5d0d 0a65 7863 6c75 6465 203d 205b  st]..exclude = [
+000003c0: 0d0a 2020 2020 222e 636f 7665 7261 6765  ..    ".coverage
+000003d0: 222c 0d0a 2020 2020 222e 7079 7465 7374  ",..    ".pytest
+000003e0: 5f63 6163 6865 222c 0d0a 2020 2020 222e  _cache",..    ".
+000003f0: 7673 636f 6465 222c 0d0a 2020 2020 2274  vscode",..    "t
+00000400: 6573 7473 222c 0d0a 2020 2020 222e 6769  ests",..    ".gi
+00000410: 7469 676e 6f72 6522 0d0a 2020 2020 5d0d  tignore"..    ].
+00000420: 0a5b 7072 6f6a 6563 742e 7363 7269 7074  .[project.script
+00000430: 735d 0d0a 6769 7462 6574 7465 7220 3d20  s]..gitbetter = 
+00000440: 2267 6974 6265 7474 6572 2e67 6974 6265  "gitbetter.gitbe
+00000450: 7474 6572 3a6d 6169 6e22 0d0a            tter:main"..
```

### Comparing `gitbetter-0.1.0/PKG-INFO` & `gitbetter-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: argshell
 Requires-Dist: pathier
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # gitbetter
```

