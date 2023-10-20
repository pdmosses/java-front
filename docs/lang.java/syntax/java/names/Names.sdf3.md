---
title: Names.sdf3
hide:
  - toc
---

# `Names.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/names/Names.sdf3]

[pdmosses/java-front/lang.java/syntax/java/names/Names.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/names/Names.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/names/Names_57_73" id="java/names/Names_7_23" title="Referenced at ../Main.sdf3 line 7; ../../classes/ConstructorDeclarations.sdf3 line 11; ../../expressions/ArrayAccess.sdf3 line 6; ../../expressions/AssignmentOperators.sdf3 line 8; ../../expressions/ClassInstanceCreation.sdf3 line 6; ../../expressions/Disambiguation.sdf3 line 13; ../../expressions/FieldAccess.sdf3 line 6; ../../expressions/MethodInvocation.sdf3 line 6; ../../expressions/MethodReference.sdf3 line 9; ../../expressions/Postfix.sdf3 line 6; ../../expressions/PrimaryExpressions.sdf3 line 7; ../../interfaces/Annotations.sdf3 line 6; ../../packages/ImportDeclarations.sdf3 line 6; ../../statements/Statements.sdf3 line 10">java/names/Names</a>

<span class="layout">// 6.5. Determining the Meaning of a Name</span>

<span class="keyword">imports</span> 
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_79_103" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  
<span class="keyword">context-free sorts</span>
  
  <a href="#PackageName_329_340" id="PackageName_131_142" title="Referenced at line 20">PackageName</a>
  <a href="../../expressions/FieldAccess.sdf3/#TypeName_359_367" id="TypeName_145_153" title="Referenced at ../../expressions/FieldAccess.sdf3 line 20; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 17; ../../expressions/PrimaryExpressions.sdf3 line 20, 23; ../../interfaces/Annotations.sdf3 line 19, 20, 21; ../../packages/ImportDeclarations.sdf3 line 15, 17, 18">TypeName</a>
  <a href="#PackageOrTypeName_433_450" id="PackageOrTypeName_156_173" title="Referenced at line 22, 24; ../../packages/ImportDeclarations.sdf3 line 16">PackageOrTypeName</a>
  <a href="../../expressions/AssignmentOperators.sdf3/#ExpressionName_915_929" id="ExpressionName_176_190" title="Referenced at ../../expressions/AssignmentOperators.sdf3 line 29; ../../expressions/Disambiguation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 22; ../../expressions/Postfix.sdf3 line 13; ../../statements/Statements.sdf3 line 57, 58, 59">ExpressionName</a>
  <a href="#AmbiguousName_653_666" id="AmbiguousName_193_206" title="Referenced at line 26, 28">AmbiguousName</a>
  <a href="../../expressions/MethodInvocation.sdf3/#MethodName_228_238" id="MethodName_209_219" title="Referenced at ../../expressions/MethodInvocation.sdf3 line 12">MethodName</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#PackageName_329_340" id="PackageName_246_257" title="Referenced at line 20">PackageName</a>.<span class="cons_Constructor"><span id="PackageName_258_269" title="Not referenced locally, nor via imports">PackageName</span></span>             = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_284_286" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#PackageName_329_340" id="PackageName_289_300" title="Referenced at line 20">PackageName</a>.<span class="cons_Constructor"><span id="PackageName_301_312" title="Not referenced locally, nor via imports">PackageName</span></span>             = &lt;&lt;<a href="#PackageName_131_142" id="PackageName_329_340" title="Defined at line 10, 19, 20">PackageName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_343_345" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="../../expressions/FieldAccess.sdf3/#TypeName_359_367" id="TypeName_350_358" title="Referenced at ../../expressions/FieldAccess.sdf3 line 20; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 17; ../../expressions/PrimaryExpressions.sdf3 line 20, 23; ../../interfaces/Annotations.sdf3 line 19, 20, 21; ../../packages/ImportDeclarations.sdf3 line 15, 17, 18">TypeName</a>.<span class="cons_Constructor"><span id="TypeName_359_367" title="Not referenced locally, nor via imports">TypeName</span></span>                   = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_388_390" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="../../expressions/FieldAccess.sdf3/#TypeName_359_367" id="TypeName_393_401" title="Referenced at ../../expressions/FieldAccess.sdf3 line 20; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 17; ../../expressions/PrimaryExpressions.sdf3 line 20, 23; ../../interfaces/Annotations.sdf3 line 19, 20, 21; ../../packages/ImportDeclarations.sdf3 line 15, 17, 18">TypeName</a>.<span class="cons_Constructor"><span id="TypeName_402_410" title="Not referenced locally, nor via imports">TypeName</span></span>                   = &lt;&lt;<a href="#PackageOrTypeName_156_173" id="PackageOrTypeName_433_450" title="Defined at line 12, 23, 24">PackageOrTypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_453_455" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#PackageOrTypeName_433_450" id="PackageOrTypeName_460_477" title="Referenced at line 22, 24; ../../packages/ImportDeclarations.sdf3 line 16">PackageOrTypeName</a>.<span class="cons_Constructor"><span id="PackageOrTypeName_478_495" title="Not referenced locally, nor via imports">PackageOrTypeName</span></span> = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_498_500" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#PackageOrTypeName_433_450" id="PackageOrTypeName_503_520" title="Referenced at line 22, 24; ../../packages/ImportDeclarations.sdf3 line 16">PackageOrTypeName</a>.<span class="cons_Constructor"><span id="PackageOrTypeName_521_538" title="Not referenced locally, nor via imports">PackageOrTypeName</span></span> = &lt;&lt;<a href="#PackageOrTypeName_156_173" id="PackageOrTypeName_543_560" title="Defined at line 12, 23, 24">PackageOrTypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_563_565" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="../../expressions/AssignmentOperators.sdf3/#ExpressionName_915_929" id="ExpressionName_570_584" title="Referenced at ../../expressions/AssignmentOperators.sdf3 line 29; ../../expressions/Disambiguation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 22; ../../expressions/Postfix.sdf3 line 13; ../../statements/Statements.sdf3 line 57, 58, 59">ExpressionName</a>.<span class="cons_Constructor"><span id="ExpressionName_585_599" title="Not referenced locally, nor via imports">ExpressionName</span></span>       = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_608_610" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="../../expressions/AssignmentOperators.sdf3/#ExpressionName_915_929" id="ExpressionName_613_627" title="Referenced at ../../expressions/AssignmentOperators.sdf3 line 29; ../../expressions/Disambiguation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 22; ../../expressions/Postfix.sdf3 line 13; ../../statements/Statements.sdf3 line 57, 58, 59">ExpressionName</a>.<span class="cons_Constructor"><span id="ExpressionName_628_642" title="Not referenced locally, nor via imports">ExpressionName</span></span>       = &lt;&lt;<a href="#AmbiguousName_193_206" id="AmbiguousName_653_666" title="Defined at line 14, 27, 28">AmbiguousName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_669_671" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#AmbiguousName_653_666" id="AmbiguousName_676_689" title="Referenced at line 26, 28">AmbiguousName</a>.<span class="cons_Constructor"><span id="AmbiguousName_690_703" title="Not referenced locally, nor via imports">AmbiguousName</span></span>         = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_714_716" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#AmbiguousName_653_666" id="AmbiguousName_719_732" title="Referenced at line 26, 28">AmbiguousName</a>.<span class="cons_Constructor"><span id="AmbiguousName_733_746" title="Not referenced locally, nor via imports">AmbiguousName</span></span>         = &lt;&lt;<a href="#AmbiguousName_193_206" id="AmbiguousName_759_772" title="Defined at line 14, 27, 28">AmbiguousName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_775_777" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="../../expressions/MethodInvocation.sdf3/#MethodName_228_238" id="MethodName_782_792" title="Referenced at ../../expressions/MethodInvocation.sdf3 line 12">MethodName</a>.<span class="cons_Constructor"><span id="MethodName_793_803" title="Not referenced locally, nor via imports">MethodName</span></span>               = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_820_822" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
</code></pre></td></tr></tbody></table></div>