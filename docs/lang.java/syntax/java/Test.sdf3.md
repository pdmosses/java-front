---
title: Test.sdf3
hide:
  - toc
---

# `Test.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/Test.sdf3]

[pdmosses/java-front/lang.java/syntax/java/Test.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/Test.sdf3 "The source file on GitHub"

<div class="sdf3"><table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span></span>1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../metaborg-java.sdf3/#java/Test_8_3" id="java/Test_1_8" title="a definition with a single reference">java/Test</a>

<span class="layout">// The Java Language Specification</span>
<span class="layout">// Java SE 8 Edition</span>

<span class="keyword">imports</span>
  <a href="../Main.sdf3/#java/Main_1_8" id="java/Main_7_3" title="a reference to a single-file definition">java/Main</a>
  <a href="../lexical/Comments.sdf3/#java/lexical/Comments_1_8" id="java/lexical/Comments_8_3" title="a reference to a single-file definition">java/lexical/Comments</a>
  <a href="../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_9_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../lexical/LineTerminators.sdf3/#java/lexical/LineTerminators_1_8" id="java/lexical/LineTerminators_10_3" title="a reference to a single-file definition">java/lexical/LineTerminators</a>
  <a href="../packages/CompilationUnits.sdf3/#java/packages/CompilationUnits_1_8" id="java/packages/CompilationUnits_11_3" title="a reference to a single-file definition">java/packages/CompilationUnits</a>

<span class="keyword">context-free sorts</span>

  <span id="Expectation_15_3" title="a definition with no references">Expectation</span> <button class="modal-open" id="TestUnit_15_15" title="a definition with multiple references" data-urls="#TestUnit line 21_7, 26_9">TestUnit</button>

<span class="keyword">context-free syntax</span>

  <a href="#CompilationUnit_32_6" id="CompilationUnit_19_3" title="a definition with a single reference">CompilationUnit</a>.<span class="cons_Constructor"><span id="Test_19_19" title="a definition with no references">Test</span></span> = &lt;
    <span class="cons_String">test;</span>
    &lt;{<a href="#TestUnit_15_15" id="TestUnit_21_7" title="a reference to a single-file definition">TestUnit</a> <span class="cons_Lit">"\n"</span>}*&gt;
  &gt;

  <button class="modal-open" id="TestUnit_24_3" title="a definition with multiple references" data-urls="#TestUnit line 21_7, 26_9">TestUnit</button>.<span class="cons_Constructor"><span id="TestPkg_24_12" title="a definition with no references">TestPkg</span></span> = &lt;
    <span class="cons_String">[</span>&lt;<a href="../lexical/Identifiers.sdf3/#ID_19_3" id="ID_25_7" title="a reference to a single-file definition">ID</a>&gt;<span class="cons_String">]</span> <span class="cons_String">{</span>
      &lt;{<a href="#TestUnit_15_15" id="TestUnit_26_9" title="a reference to a single-file definition">TestUnit</a> <span class="cons_Lit">"\n"</span>}*&gt;
    <span class="cons_String">}</span>
  &gt;

  <button class="modal-open" id="TestUnit_30_3" title="a definition with multiple references" data-urls="#TestUnit line 21_7, 26_9">TestUnit</button>.<span class="cons_Constructor"><span id="TestFile_30_12" title="a definition with no references">TestFile</span></span> = &lt;
    <span class="cons_String">[</span>&lt;<a href="../lexical/Identifiers.sdf3/#ID_19_3" id="ID_31_7" title="a reference to a single-file definition">ID</a>&gt;<span class="cons_String">]</span>
    &lt;<a href="#CompilationUnit_19_3" id="CompilationUnit_32_6" title="a reference to a single-file definition">CompilationUnit</a>&gt;
  &gt;


</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
