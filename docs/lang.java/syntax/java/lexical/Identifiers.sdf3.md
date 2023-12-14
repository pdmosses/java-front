---
title: Identifiers.sdf3
hide:
  - toc
---

# `Identifiers.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/Identifiers.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/Identifiers.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/Identifiers.sdf3 "The source file on GitHub"

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
34
35
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Identifiers_1_8" title="Multi-file references" data-urls="../Main.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../Test.sdf3/#java/lexical/Identifiers_9_3 line 9; ../../classes/ClassDeclarations.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../classes/ConstructorDeclarations.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../classes/EnumDeclarations.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../classes/FieldDeclarations.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../classes/MethodDeclarations.sdf3/#java/lexical/Identifiers_8_3 line 8; ../../expressions/ClassInstanceCreation.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../expressions/FieldAccess.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../expressions/LambdaExpressions.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../expressions/MethodInvocation.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../expressions/MethodReference.sdf3/#java/lexical/Identifiers_8_3 line 8; ../../interfaces/Annotations.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../interfaces/AnnotationTypes.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../interfaces/InterfaceDeclarations.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../names/Names.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../packages/ImportDeclarations.sdf3/#java/lexical/Identifiers_7_3 line 7; ../../packages/PackageDeclarations.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../statements/Statements.sdf3/#java/lexical/Identifiers_8_3 line 8; ../../types/ReferenceTypes.sdf3/#java/lexical/Identifiers_6_3 line 6; ../../types/TypeVariable.sdf3/#java/lexical/Identifiers_7_3 line 7">java/lexical/Identifiers</button>

<span class="layout">// 3.8. Identifiers</span>

<span class="keyword">imports</span>

  <a href="../Keywords.sdf3/#java/lexical/Keywords_1_8" id="java/lexical/Keywords_7_3" title="Defined at ../Keywords.sdf3 line 1">java/lexical/Keywords</a>

<span class="keyword">lexical start-symbols</span>
  
  <a href="#ID_19_3" id="ID_11_3" title="Defined at line 19, 27, 28, 29, 30, 31">ID</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Id_15_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Id_37_33 line 37; ../../classes/ConstructorDeclarations.sdf3/#Id_25_51 line 25; ../../classes/EnumDeclarations.sdf3/#Id_21_32 line 21, 26, 31, 35; ../../classes/FieldDeclarations.sdf3/#Id_31_33 line 31, 32, 59, 60; ../../classes/MethodDeclarations.sdf3/#Id_34_13 line 34, 37, 59; ../../expressions/ClassInstanceCreation.sdf3/#Id_24_45 line 24, 27, 31; ../../expressions/FieldAccess.sdf3/#Id_18_44 line 18, 19, 20; ../../expressions/LambdaExpressions.sdf3/#Id_19_42 line 19, 21; ../../expressions/MethodInvocation.sdf3/#Id_16_64 line 16, 17, 18; ../../expressions/MethodReference.sdf3/#Id_14_73 line 14, 15, 16, 17; ../../interfaces/Annotations.sdf3/#Id_23_36 line 23; ../../interfaces/AnnotationTypes.sdf3/#Id_27_42 line 27, 38; ../../interfaces/InterfaceDeclarations.sdf3/#Id_27_41 line 27; ../../names/Names.sdf3/#Id_19_41 line 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29; ../../packages/ImportDeclarations.sdf3/#Id_17_71 line 17; ../../packages/PackageDeclarations.sdf3/#Id_15_74 line 15; ../../statements/Statements.sdf3/#Id_34_25 line 34, 84, 87; ../../types/ReferenceTypes.sdf3/#Id_26_64 line 26, 27, 35; ../../types/TypeVariable.sdf3/#Id_16_62 line 16, 17">Id</button>

<span class="keyword">lexical sorts</span>
  
  <button class="modal-open" id="ID_19_3" title="Multi-file references" data-urls="#ID_11_3 line 11, 23, 35; ../../Test.sdf3/#ID_25_7 line 25, 31">ID</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Id_23_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Id_37_33 line 37; ../../classes/ConstructorDeclarations.sdf3/#Id_25_51 line 25; ../../classes/EnumDeclarations.sdf3/#Id_21_32 line 21, 26, 31, 35; ../../classes/FieldDeclarations.sdf3/#Id_31_33 line 31, 32, 59, 60; ../../classes/MethodDeclarations.sdf3/#Id_34_13 line 34, 37, 59; ../../expressions/ClassInstanceCreation.sdf3/#Id_24_45 line 24, 27, 31; ../../expressions/FieldAccess.sdf3/#Id_18_44 line 18, 19, 20; ../../expressions/LambdaExpressions.sdf3/#Id_19_42 line 19, 21; ../../expressions/MethodInvocation.sdf3/#Id_16_64 line 16, 17, 18; ../../expressions/MethodReference.sdf3/#Id_14_73 line 14, 15, 16, 17; ../../interfaces/Annotations.sdf3/#Id_23_36 line 23; ../../interfaces/AnnotationTypes.sdf3/#Id_27_42 line 27, 38; ../../interfaces/InterfaceDeclarations.sdf3/#Id_27_41 line 27; ../../names/Names.sdf3/#Id_19_41 line 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29; ../../packages/ImportDeclarations.sdf3/#Id_17_71 line 17; ../../packages/PackageDeclarations.sdf3/#Id_15_74 line 15; ../../statements/Statements.sdf3/#Id_34_25 line 34, 84, 87; ../../types/ReferenceTypes.sdf3/#Id_26_64 line 26, 27, 35; ../../types/TypeVariable.sdf3/#Id_16_62 line 16, 17">Id</button>.<span class="cons_Constructor"><span id="Id_23_6" title="Not referenced">Id</span></span> = <a href="#ID_19_3" id="ID_23_11" title="Defined at line 19, 27, 28, 29, 30, 31">ID</a>

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="ID_27_3" title="Multi-file references" data-urls="#ID_11_3 line 11, 23, 35; ../../Test.sdf3/#ID_25_7 line 25, 31">ID</button> = [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span>\_\$] [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]*
  <button class="modal-open" id="ID_28_3" title="Multi-file references" data-urls="#ID_11_3 line 11, 23, 35; ../../Test.sdf3/#ID_25_7 line 25, 31">ID</button> = <a href="../Keywords.sdf3/#Keyword_7_3" id="Keyword_28_8" title="Defined at ../Keywords.sdf3 line 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56">Keyword</a> {<span class="keyword">reject</span>}
  <button class="modal-open" id="ID_29_3" title="Multi-file references" data-urls="#ID_11_3 line 11, 23, 35; ../../Test.sdf3/#ID_25_7 line 25, 31">ID</button> = <span class="cons_Lit">"true"</span> {<span class="keyword">reject</span>}
  <button class="modal-open" id="ID_30_3" title="Multi-file references" data-urls="#ID_11_3 line 11, 23, 35; ../../Test.sdf3/#ID_25_7 line 25, 31">ID</button> = <span class="cons_Lit">"false"</span> {<span class="keyword">reject</span>}
  <button class="modal-open" id="ID_31_3" title="Multi-file references" data-urls="#ID_11_3 line 11, 23, 35; ../../Test.sdf3/#ID_25_7 line 25, 31">ID</button> = <span class="cons_Lit">"null"</span> {<span class="keyword">reject</span>}

<span class="keyword">lexical restrictions</span>

  <a href="#ID_19_3" id="ID_35_3" title="Defined at line 19, 27, 28, 29, 30, 31">ID</a> -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
