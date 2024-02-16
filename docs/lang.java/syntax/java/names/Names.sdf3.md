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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/names/Names_1_8" title="a definition with multiple references" data-urls="../Main.sdf3/#java/names/Names line 7_3; ../../classes/ConstructorDeclarations.sdf3/#java/names/Names line 11_3; ../../expressions/ArrayAccess.sdf3/#java/names/Names line 6_3; ../../expressions/AssignmentOperators.sdf3/#java/names/Names line 8_3; ../../expressions/ClassInstanceCreation.sdf3/#java/names/Names line 6_3; ../../expressions/Disambiguation.sdf3/#java/names/Names line 13_3; ../../expressions/FieldAccess.sdf3/#java/names/Names line 6_3; ../../expressions/MethodInvocation.sdf3/#java/names/Names line 6_3; ../../expressions/MethodReference.sdf3/#java/names/Names line 9_3; ../../expressions/Postfix.sdf3/#java/names/Names line 6_3; ../../expressions/PrimaryExpressions.sdf3/#java/names/Names line 7_3; ../../interfaces/Annotations.sdf3/#java/names/Names line 6_3; ../../packages/ImportDeclarations.sdf3/#java/names/Names line 6_3; ../../statements/Statements.sdf3/#java/names/Names line 10_3">java/names/Names</button>

<span class="layout">// 6.5. Determining the Meaning of a Name</span>

<span class="keyword">imports</span> 
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  
<span class="keyword">context-free sorts</span>
  
  <a href="#PackageName_20_43" id="PackageName_10_3" title="a definition with a single reference">PackageName</a>
  <button class="modal-open" id="TypeName_11_3" title="a definition with multiple references" data-urls="../../expressions/FieldAccess.sdf3/#TypeName line 20_31; ../../expressions/MethodInvocation.sdf3/#TypeName line 18_34; ../../expressions/MethodReference.sdf3/#TypeName line 17_40; ../../expressions/PrimaryExpressions.sdf3/#TypeName line 20_24, 23_44; ../../interfaces/Annotations.sdf3/#TypeName line 19_24, 20_30, 21_34; ../../packages/ImportDeclarations.sdf3/#TypeName line 15_53, 17_60, 18_60">TypeName</button>
  <button class="modal-open" id="PackageOrTypeName_12_3" title="a definition with multiple references" data-urls="#PackageOrTypeName line 22_43, 24_43; ../../packages/ImportDeclarations.sdf3/#PackageOrTypeName line 16_53">PackageOrTypeName</button>
  <button class="modal-open" id="ExpressionName_13_3" title="a definition with multiple references" data-urls="../../expressions/AssignmentOperators.sdf3/#ExpressionName line 29_9; ../../expressions/Disambiguation.sdf3/#ExpressionName line 18_16; ../../expressions/MethodReference.sdf3/#ExpressionName line 22_49; ../../expressions/Postfix.sdf3/#ExpressionName line 13_16; ../../statements/Statements.sdf3/#ExpressionName line 57_15, 57_34, 58_15, 58_34, 58_53, 59_15, 59_34, 59_53, 59_72">ExpressionName</button>
  <button class="modal-open" id="AmbiguousName_14_3" title="a definition with multiple references" data-urls="#AmbiguousName line 26_43, 28_43">AmbiguousName</button>
  <a href="../../expressions/MethodInvocation.sdf3/#MethodName_12_34" id="MethodName_15_3" title="a definition with a single reference">MethodName</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#PackageName_20_43" id="PackageName_19_3" title="a definition with a single reference">PackageName</a>.<span class="cons_Constructor"><span id="PackageName_19_15" title="a definition with no references">PackageName</span></span>             = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_19_41" title="a reference to a single-file definition">Id</a>
  <a href="#PackageName_20_43" id="PackageName_20_3" title="a definition with a single reference">PackageName</a>.<span class="cons_Constructor"><span id="PackageName_20_15" title="a definition with no references">PackageName</span></span>             = &lt;&lt;<a href="#PackageName_10_3" id="PackageName_20_43" title="a reference to a single-file definition">PackageName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_20_57" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="TypeName_21_3" title="a definition with multiple references" data-urls="../../expressions/FieldAccess.sdf3/#TypeName line 20_31; ../../expressions/MethodInvocation.sdf3/#TypeName line 18_34; ../../expressions/MethodReference.sdf3/#TypeName line 17_40; ../../expressions/PrimaryExpressions.sdf3/#TypeName line 20_24, 23_44; ../../interfaces/Annotations.sdf3/#TypeName line 19_24, 20_30, 21_34; ../../packages/ImportDeclarations.sdf3/#TypeName line 15_53, 17_60, 18_60">TypeName</button>.<span class="cons_Constructor"><span id="TypeName_21_12" title="a definition with no references">TypeName</span></span>                   = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_21_41" title="a reference to a single-file definition">Id</a>
  <button class="modal-open" id="TypeName_22_3" title="a definition with multiple references" data-urls="../../expressions/FieldAccess.sdf3/#TypeName line 20_31; ../../expressions/MethodInvocation.sdf3/#TypeName line 18_34; ../../expressions/MethodReference.sdf3/#TypeName line 17_40; ../../expressions/PrimaryExpressions.sdf3/#TypeName line 20_24, 23_44; ../../interfaces/Annotations.sdf3/#TypeName line 19_24, 20_30, 21_34; ../../packages/ImportDeclarations.sdf3/#TypeName line 15_53, 17_60, 18_60">TypeName</button>.<span class="cons_Constructor"><span id="TypeName_22_12" title="a definition with no references">TypeName</span></span>                   = &lt;&lt;<a href="#PackageOrTypeName_12_3" id="PackageOrTypeName_22_43" title="a reference to a single-file definition">PackageOrTypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_22_63" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="PackageOrTypeName_23_3" title="a definition with multiple references" data-urls="#PackageOrTypeName line 22_43, 24_43; ../../packages/ImportDeclarations.sdf3/#PackageOrTypeName line 16_53">PackageOrTypeName</button>.<span class="cons_Constructor"><span id="PackageOrTypeName_23_21" title="a definition with no references">PackageOrTypeName</span></span> = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_23_41" title="a reference to a single-file definition">Id</a>
  <button class="modal-open" id="PackageOrTypeName_24_3" title="a definition with multiple references" data-urls="#PackageOrTypeName line 22_43, 24_43; ../../packages/ImportDeclarations.sdf3/#PackageOrTypeName line 16_53">PackageOrTypeName</button>.<span class="cons_Constructor"><span id="PackageOrTypeName_24_21" title="a definition with no references">PackageOrTypeName</span></span> = &lt;&lt;<a href="#PackageOrTypeName_12_3" id="PackageOrTypeName_24_43" title="a reference to a single-file definition">PackageOrTypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_24_63" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="ExpressionName_25_3" title="a definition with multiple references" data-urls="../../expressions/AssignmentOperators.sdf3/#ExpressionName line 29_9; ../../expressions/Disambiguation.sdf3/#ExpressionName line 18_16; ../../expressions/MethodReference.sdf3/#ExpressionName line 22_49; ../../expressions/Postfix.sdf3/#ExpressionName line 13_16; ../../statements/Statements.sdf3/#ExpressionName line 57_15, 57_34, 58_15, 58_34, 58_53, 59_15, 59_34, 59_53, 59_72">ExpressionName</button>.<span class="cons_Constructor"><span id="ExpressionName_25_18" title="a definition with no references">ExpressionName</span></span>       = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_25_41" title="a reference to a single-file definition">Id</a>
  <button class="modal-open" id="ExpressionName_26_3" title="a definition with multiple references" data-urls="../../expressions/AssignmentOperators.sdf3/#ExpressionName line 29_9; ../../expressions/Disambiguation.sdf3/#ExpressionName line 18_16; ../../expressions/MethodReference.sdf3/#ExpressionName line 22_49; ../../expressions/Postfix.sdf3/#ExpressionName line 13_16; ../../statements/Statements.sdf3/#ExpressionName line 57_15, 57_34, 58_15, 58_34, 58_53, 59_15, 59_34, 59_53, 59_72">ExpressionName</button>.<span class="cons_Constructor"><span id="ExpressionName_26_18" title="a definition with no references">ExpressionName</span></span>       = &lt;&lt;<a href="#AmbiguousName_14_3" id="AmbiguousName_26_43" title="a reference to a single-file definition">AmbiguousName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_26_59" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="AmbiguousName_27_3" title="a definition with multiple references" data-urls="#AmbiguousName line 26_43, 28_43">AmbiguousName</button>.<span class="cons_Constructor"><span id="AmbiguousName_27_17" title="a definition with no references">AmbiguousName</span></span>         = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_41" title="a reference to a single-file definition">Id</a>
  <button class="modal-open" id="AmbiguousName_28_3" title="a definition with multiple references" data-urls="#AmbiguousName line 26_43, 28_43">AmbiguousName</button>.<span class="cons_Constructor"><span id="AmbiguousName_28_17" title="a definition with no references">AmbiguousName</span></span>         = &lt;&lt;<a href="#AmbiguousName_14_3" id="AmbiguousName_28_43" title="a reference to a single-file definition">AmbiguousName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_28_59" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <a href="../../expressions/MethodInvocation.sdf3/#MethodName_12_34" id="MethodName_29_3" title="a definition with a single reference">MethodName</a>.<span class="cons_Constructor"><span id="MethodName_29_14" title="a definition with no references">MethodName</span></span>               = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_29_41" title="a reference to a single-file definition">Id</a>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
