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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../metaborg-java.sdf3#java/Test_101_110" id="java/Test_7_16" title="Referenced at ../../metaborg-java.sdf3 line 8">java/Test</a>

<span class="layout">// The Java Language Specification</span>
<span class="layout">// Java SE 8 Edition</span>

<span class="keyword">imports</span>
  <a href="../Main.sdf3#java/Main_7_16" id="java/Main_85_94" title="Defined at ../Main.sdf3 line 1">java/Main</a>
  <a href="../lexical/Comments.sdf3#java/lexical/Comments_7_28" id="java/lexical/Comments_97_118" title="Defined at ../lexical/Comments.sdf3 line 1">java/lexical/Comments</a>
  <a href="../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_121_145" title="Defined at ../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../lexical/LineTerminators.sdf3#java/lexical/LineTerminators_7_35" id="java/lexical/LineTerminators_148_176" title="Defined at ../lexical/LineTerminators.sdf3 line 1">java/lexical/LineTerminators</a>
  <a href="../packages/CompilationUnits.sdf3#java/packages/CompilationUnits_7_37" id="java/packages/CompilationUnits_179_209" title="Defined at ../packages/CompilationUnits.sdf3 line 1">java/packages/CompilationUnits</a>

<span class="keyword">context-free sorts</span>

  <span id="Expectation_233_244" title="Not referenced locally, nor via imports">Expectation</span> <a href="#TestUnit_385_393" id="TestUnit_245_253" title="Referenced at line 26">TestUnit</a>

<span class="keyword">context-free syntax</span>

  <a href="#CompilationUnit_453_468" id="CompilationUnit_278_293" title="Referenced at line 32">CompilationUnit</a>.<span class="cons_Constructor"><span id="Test_294_298" title="Not referenced locally, nor via imports">Test</span></span> = &lt;
    <span class="cons_String">test;</span>
    &lt;{<a href="#TestUnit_245_253" id="TestUnit_319_327" title="Defined at line 15, 24, 30">TestUnit</a> <span class="cons_Lit">"\n"</span>}*&gt;
  &gt;

  <a href="#TestUnit_385_393" id="TestUnit_343_351" title="Referenced at line 26">TestUnit</a>.<span class="cons_Constructor"><span id="TestPkg_352_359" title="Not referenced locally, nor via imports">TestPkg</span></span> = &lt;
    <span class="cons_String">[</span>&lt;<a href="../lexical/Identifiers.sdf3#ID_164_166" id="ID_370_372" title="Defined at ../lexical/Identifiers.sdf3 line 19, 27, 28, 29, 30, 31">ID</a>&gt;<span class="cons_String">]</span> <span class="cons_String">{</span>
      &lt;{<a href="#TestUnit_245_253" id="TestUnit_385_393" title="Defined at line 15, 24, 30">TestUnit</a> <span class="cons_Lit">"\n"</span>}*&gt;
    <span class="cons_String">}</span>
  &gt;

  <a href="#TestUnit_385_393" id="TestUnit_415_423" title="Referenced at line 26">TestUnit</a>.<span class="cons_Constructor"><span id="TestFile_424_432" title="Not referenced locally, nor via imports">TestFile</span></span> = &lt;
    <span class="cons_String">[</span>&lt;<a href="../lexical/Identifiers.sdf3#ID_164_166" id="ID_443_445" title="Defined at ../lexical/Identifiers.sdf3 line 19, 27, 28, 29, 30, 31">ID</a>&gt;<span class="cons_String">]</span>
    &lt;<a href="#CompilationUnit_278_293" id="CompilationUnit_453_468" title="Defined at line 19">CompilationUnit</a>&gt;
  &gt;


</code></pre></td></tr></tbody></table></div>