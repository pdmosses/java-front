---
title: CompilationUnits.sdf3
hide:
  - toc
---

# `CompilationUnits.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/packages/CompilationUnits.sdf3]

[pdmosses/java-front/lang.java/syntax/java/packages/CompilationUnits.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/packages/CompilationUnits.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/packages/CompilationUnits_61_91" id="java/packages/CompilationUnits_7_37" title="Referenced at ../Main.sdf3 line 6; ../../Test.sdf3 line 11; ../../../Java_StrategoMix.sdf3 line 4; ../../../metaborg-java.sdf3 line 9">java/packages/CompilationUnits</a>

<span class="layout">// 7.3. Compilation Units</span>

<span class="keyword">imports</span> 
  <a href="../PackageDeclarations.sdf3/#java/packages/PackageDeclarations_7_40" id="java/packages/PackageDeclarations_77_110" title="Defined at ../PackageDeclarations.sdf3 line 1">java/packages/PackageDeclarations</a>
  <a href="../ImportDeclarations.sdf3/#java/packages/ImportDeclarations_7_39" id="java/packages/ImportDeclarations_113_145" title="Defined at ../ImportDeclarations.sdf3 line 1">java/packages/ImportDeclarations</a>
  <a href="../TypeDeclarations.sdf3/#java/packages/TypeDeclarations_7_37" id="java/packages/TypeDeclarations_148_178" title="Defined at ../TypeDeclarations.sdf3 line 1">java/packages/TypeDeclarations</a>

<span class="keyword">context-free sorts</span>

  <a href="../../../Java_StrategoMix.sdf3/#CompilationUnit_397_412" id="CompilationUnit_202_217" title="Referenced at ../../../Java_StrategoMix.sdf3 line 22, 23, 24, 25; ../../../metaborg-java.sdf3 line 21">CompilationUnit</a>

<span class="keyword">context-free syntax</span>


  <a href="../../../Java_StrategoMix.sdf3/#CompilationUnit_397_412" id="CompilationUnit_243_258" title="Referenced at ../../../Java_StrategoMix.sdf3 line 22, 23, 24, 25; ../../../metaborg-java.sdf3 line 21">CompilationUnit</a>.<span class="cons_Constructor"><span id="CompilationUnit_259_274" title="Not referenced locally, nor via imports">CompilationUnit</span></span> = &lt;
  &lt;<a href="../PackageDeclarations.sdf3/#PackageDeclaration_162_180" id="PackageDeclaration_282_300" title="Defined at ../PackageDeclarations.sdf3 line 11, 15">PackageDeclaration</a>?&gt;
  
  &lt;{<a href="../ImportDeclarations.sdf3/#ImportDeclaration_147_164" id="ImportDeclaration_310_327" title="Defined at ../ImportDeclarations.sdf3 line 11, 15, 16, 17, 18">ImportDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
     
  &lt;{<a href="../TypeDeclarations.sdf3/#TypeDeclaration_205_220" id="TypeDeclaration_346_361" title="Defined at ../TypeDeclarations.sdf3 line 12, 16, 17, 18">TypeDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt; 
</code></pre></td></tr></tbody></table></div>