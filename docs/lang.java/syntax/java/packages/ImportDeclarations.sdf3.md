---
title: ImportDeclarations.sdf3
---

# `ImportDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/packages/ImportDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/packages/ImportDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/packages/ImportDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/packages/ImportDeclarations_94_126" id="java/packages/ImportDeclarations_7_39" title="Referenced at ../Main.sdf3 line 7">java/packages/ImportDeclarations</a>

<span class="layout">// 7.5. Import Declarations</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_80_96" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_99_123" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>

<span class="keyword">context-free sorts</span>

  <a href="../CompilationUnits.sdf3#ImportDeclaration_310_327" id="ImportDeclaration_147_164" title="Referenced at ../CompilationUnits.sdf3 line 20">ImportDeclaration</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../CompilationUnits.sdf3#ImportDeclaration_310_327" id="ImportDeclaration_191_208" title="Referenced at ../CompilationUnits.sdf3 line 20">ImportDeclaration</a>.<span class="cons_Constructor"><span id="SingleTypeImport_209_225" title="Not referenced locally, nor via imports">SingleTypeImport</span></span>     = &lt;<span class="cons_String">import</span> &lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_241_249" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">;</span>&gt;
  <a href="../CompilationUnits.sdf3#ImportDeclaration_310_327" id="ImportDeclaration_255_272" title="Referenced at ../CompilationUnits.sdf3 line 20">ImportDeclaration</a>.<span class="cons_Constructor"><span id="TypeImportOnDemand_273_291" title="Not referenced locally, nor via imports">TypeImportOnDemand</span></span>   = &lt;<span class="cons_String">import</span> &lt;<a href="../../names/Names.sdf3#PackageOrTypeName_156_173" id="PackageOrTypeName_305_322" title="Defined at ../../names/Names.sdf3 line 12, 23, 24">PackageOrTypeName</a>&gt;<span class="cons_String">.*;</span>&gt;
  <a href="../CompilationUnits.sdf3#ImportDeclaration_310_327" id="ImportDeclaration_330_347" title="Referenced at ../CompilationUnits.sdf3 line 20">ImportDeclaration</a>.<span class="cons_Constructor"><span id="SingleStaticImport_348_366" title="Not referenced locally, nor via imports">SingleStaticImport</span></span>   = &lt;<span class="cons_String">import</span> <span class="cons_String">static</span> &lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_387_395" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_398_400" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">;</span>&gt;
  <a href="../CompilationUnits.sdf3#ImportDeclaration_310_327" id="ImportDeclaration_406_423" title="Referenced at ../CompilationUnits.sdf3 line 20">ImportDeclaration</a>.<span class="cons_Constructor"><span id="StaticImportOnDemand_424_444" title="Not referenced locally, nor via imports">StaticImportOnDemand</span></span> = &lt;<span class="cons_String">import</span> <span class="cons_String">static</span> &lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_463_471" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">.*;</span>&gt;  

<span class="keyword">template options</span>
  <span class="keyword">tokenize</span> : ".;" 
</code></pre></td></tr></tbody></table></div>