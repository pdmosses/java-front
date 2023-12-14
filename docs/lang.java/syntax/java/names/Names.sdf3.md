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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/names/Names_1_8" title="Multi-file references" data-urls="../Main.sdf3/#java/names/Names_7_3 line 7; ../../classes/ConstructorDeclarations.sdf3/#java/names/Names_11_3 line 11; ../../expressions/ArrayAccess.sdf3/#java/names/Names_6_3 line 6; ../../expressions/AssignmentOperators.sdf3/#java/names/Names_8_3 line 8; ../../expressions/ClassInstanceCreation.sdf3/#java/names/Names_6_3 line 6; ../../expressions/Disambiguation.sdf3/#java/names/Names_13_3 line 13; ../../expressions/FieldAccess.sdf3/#java/names/Names_6_3 line 6; ../../expressions/MethodInvocation.sdf3/#java/names/Names_6_3 line 6; ../../expressions/MethodReference.sdf3/#java/names/Names_9_3 line 9; ../../expressions/Postfix.sdf3/#java/names/Names_6_3 line 6; ../../expressions/PrimaryExpressions.sdf3/#java/names/Names_7_3 line 7; ../../interfaces/Annotations.sdf3/#java/names/Names_6_3 line 6; ../../packages/ImportDeclarations.sdf3/#java/names/Names_6_3 line 6; ../../statements/Statements.sdf3/#java/names/Names_10_3 line 10">java/names/Names</button>

<span class="layout">// 6.5. Determining the Meaning of a Name</span>

<span class="keyword">imports</span> 
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  
<span class="keyword">context-free sorts</span>
  
  <a href="#PackageName_20_43" id="PackageName_10_3" title="Referenced at line 20">PackageName</a>
  <button class="modal-open" id="TypeName_11_3" title="Multi-file references" data-urls="../../expressions/FieldAccess.sdf3/#TypeName_20_31 line 20; ../../expressions/MethodInvocation.sdf3/#TypeName_18_34 line 18; ../../expressions/MethodReference.sdf3/#TypeName_17_40 line 17; ../../expressions/PrimaryExpressions.sdf3/#TypeName_20_24 line 20, 23; ../../interfaces/Annotations.sdf3/#TypeName_19_24 line 19, 20, 21; ../../packages/ImportDeclarations.sdf3/#TypeName_15_53 line 15, 17, 18">TypeName</button>
  <button class="modal-open" id="PackageOrTypeName_12_3" title="Multi-file references" data-urls="#PackageOrTypeName_22_43 line 22, 24; ../../packages/ImportDeclarations.sdf3/#PackageOrTypeName_16_53 line 16">PackageOrTypeName</button>
  <button class="modal-open" id="ExpressionName_13_3" title="Multi-file references" data-urls="../../expressions/AssignmentOperators.sdf3/#ExpressionName_29_9 line 29; ../../expressions/Disambiguation.sdf3/#ExpressionName_18_16 line 18; ../../expressions/MethodReference.sdf3/#ExpressionName_22_49 line 22; ../../expressions/Postfix.sdf3/#ExpressionName_13_16 line 13; ../../statements/Statements.sdf3/#ExpressionName_57_15 line 57, 58, 59">ExpressionName</button>
  <a href="#AmbiguousName_26_43" id="AmbiguousName_14_3" title="Referenced at line 26, 28">AmbiguousName</a>
  <a href="../../expressions/MethodInvocation.sdf3/#MethodName_12_34" id="MethodName_15_3" title="Referenced at ../../expressions/MethodInvocation.sdf3 line 12">MethodName</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#PackageName_20_43" id="PackageName_19_3" title="Referenced at line 20">PackageName</a>.<span class="cons_Constructor"><span id="PackageName_19_15" title="Not referenced">PackageName</span></span>             = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_19_41" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#PackageName_20_43" id="PackageName_20_3" title="Referenced at line 20">PackageName</a>.<span class="cons_Constructor"><span id="PackageName_20_15" title="Not referenced">PackageName</span></span>             = &lt;&lt;<a href="#PackageName_10_3" id="PackageName_20_43" title="Defined at line 10, 19, 20">PackageName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_20_57" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <button class="modal-open" id="TypeName_21_3" title="Multi-file references" data-urls="../../expressions/FieldAccess.sdf3/#TypeName_20_31 line 20; ../../expressions/MethodInvocation.sdf3/#TypeName_18_34 line 18; ../../expressions/MethodReference.sdf3/#TypeName_17_40 line 17; ../../expressions/PrimaryExpressions.sdf3/#TypeName_20_24 line 20, 23; ../../interfaces/Annotations.sdf3/#TypeName_19_24 line 19, 20, 21; ../../packages/ImportDeclarations.sdf3/#TypeName_15_53 line 15, 17, 18">TypeName</button>.<span class="cons_Constructor"><span id="TypeName_21_12" title="Not referenced">TypeName</span></span>                   = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_21_41" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <button class="modal-open" id="TypeName_22_3" title="Multi-file references" data-urls="../../expressions/FieldAccess.sdf3/#TypeName_20_31 line 20; ../../expressions/MethodInvocation.sdf3/#TypeName_18_34 line 18; ../../expressions/MethodReference.sdf3/#TypeName_17_40 line 17; ../../expressions/PrimaryExpressions.sdf3/#TypeName_20_24 line 20, 23; ../../interfaces/Annotations.sdf3/#TypeName_19_24 line 19, 20, 21; ../../packages/ImportDeclarations.sdf3/#TypeName_15_53 line 15, 17, 18">TypeName</button>.<span class="cons_Constructor"><span id="TypeName_22_12" title="Not referenced">TypeName</span></span>                   = &lt;&lt;<a href="#PackageOrTypeName_12_3" id="PackageOrTypeName_22_43" title="Defined at line 12, 23, 24">PackageOrTypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_22_63" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <button class="modal-open" id="PackageOrTypeName_23_3" title="Multi-file references" data-urls="#PackageOrTypeName_22_43 line 22, 24; ../../packages/ImportDeclarations.sdf3/#PackageOrTypeName_16_53 line 16">PackageOrTypeName</button>.<span class="cons_Constructor"><span id="PackageOrTypeName_23_21" title="Not referenced">PackageOrTypeName</span></span> = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_23_41" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <button class="modal-open" id="PackageOrTypeName_24_3" title="Multi-file references" data-urls="#PackageOrTypeName_22_43 line 22, 24; ../../packages/ImportDeclarations.sdf3/#PackageOrTypeName_16_53 line 16">PackageOrTypeName</button>.<span class="cons_Constructor"><span id="PackageOrTypeName_24_21" title="Not referenced">PackageOrTypeName</span></span> = &lt;&lt;<a href="#PackageOrTypeName_12_3" id="PackageOrTypeName_24_43" title="Defined at line 12, 23, 24">PackageOrTypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_24_63" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <button class="modal-open" id="ExpressionName_25_3" title="Multi-file references" data-urls="../../expressions/AssignmentOperators.sdf3/#ExpressionName_29_9 line 29; ../../expressions/Disambiguation.sdf3/#ExpressionName_18_16 line 18; ../../expressions/MethodReference.sdf3/#ExpressionName_22_49 line 22; ../../expressions/Postfix.sdf3/#ExpressionName_13_16 line 13; ../../statements/Statements.sdf3/#ExpressionName_57_15 line 57, 58, 59">ExpressionName</button>.<span class="cons_Constructor"><span id="ExpressionName_25_18" title="Not referenced">ExpressionName</span></span>       = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_25_41" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <button class="modal-open" id="ExpressionName_26_3" title="Multi-file references" data-urls="../../expressions/AssignmentOperators.sdf3/#ExpressionName_29_9 line 29; ../../expressions/Disambiguation.sdf3/#ExpressionName_18_16 line 18; ../../expressions/MethodReference.sdf3/#ExpressionName_22_49 line 22; ../../expressions/Postfix.sdf3/#ExpressionName_13_16 line 13; ../../statements/Statements.sdf3/#ExpressionName_57_15 line 57, 58, 59">ExpressionName</button>.<span class="cons_Constructor"><span id="ExpressionName_26_18" title="Not referenced">ExpressionName</span></span>       = &lt;&lt;<a href="#AmbiguousName_14_3" id="AmbiguousName_26_43" title="Defined at line 14, 27, 28">AmbiguousName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_26_59" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#AmbiguousName_26_43" id="AmbiguousName_27_3" title="Referenced at line 26, 28">AmbiguousName</a>.<span class="cons_Constructor"><span id="AmbiguousName_27_17" title="Not referenced">AmbiguousName</span></span>         = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_41" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#AmbiguousName_26_43" id="AmbiguousName_28_3" title="Referenced at line 26, 28">AmbiguousName</a>.<span class="cons_Constructor"><span id="AmbiguousName_28_17" title="Not referenced">AmbiguousName</span></span>         = &lt;&lt;<a href="#AmbiguousName_14_3" id="AmbiguousName_28_43" title="Defined at line 14, 27, 28">AmbiguousName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_28_59" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="../../expressions/MethodInvocation.sdf3/#MethodName_12_34" id="MethodName_29_3" title="Referenced at ../../expressions/MethodInvocation.sdf3 line 12">MethodName</a>.<span class="cons_Constructor"><span id="MethodName_29_14" title="Not referenced">MethodName</span></span>               = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_29_41" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
