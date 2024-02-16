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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Identifiers_1_8" title="a definition with multiple references" data-urls="../Main.sdf3/#java/lexical/Identifiers line 7_3; ../../Test.sdf3/#java/lexical/Identifiers line 9_3; ../../classes/ClassDeclarations.sdf3/#java/lexical/Identifiers line 6_3; ../../classes/ConstructorDeclarations.sdf3/#java/lexical/Identifiers line 7_3; ../../classes/EnumDeclarations.sdf3/#java/lexical/Identifiers line 6_3; ../../classes/FieldDeclarations.sdf3/#java/lexical/Identifiers line 6_3; ../../classes/MethodDeclarations.sdf3/#java/lexical/Identifiers line 8_3; ../../expressions/ClassInstanceCreation.sdf3/#java/lexical/Identifiers line 7_3; ../../expressions/FieldAccess.sdf3/#java/lexical/Identifiers line 7_3; ../../expressions/LambdaExpressions.sdf3/#java/lexical/Identifiers line 7_3; ../../expressions/MethodInvocation.sdf3/#java/lexical/Identifiers line 7_3; ../../expressions/MethodReference.sdf3/#java/lexical/Identifiers line 8_3; ../../interfaces/Annotations.sdf3/#java/lexical/Identifiers line 7_3; ../../interfaces/AnnotationTypes.sdf3/#java/lexical/Identifiers line 7_3; ../../interfaces/InterfaceDeclarations.sdf3/#java/lexical/Identifiers line 6_3; ../../names/Names.sdf3/#java/lexical/Identifiers line 6_3; ../../packages/ImportDeclarations.sdf3/#java/lexical/Identifiers line 7_3; ../../packages/PackageDeclarations.sdf3/#java/lexical/Identifiers line 6_3; ../../statements/Statements.sdf3/#java/lexical/Identifiers line 8_3; ../../types/ReferenceTypes.sdf3/#java/lexical/Identifiers line 6_3; ../../types/TypeVariable.sdf3/#java/lexical/Identifiers line 7_3">java/lexical/Identifiers</button>

<span class="layout">// 3.8. Identifiers</span>

<span class="keyword">imports</span>

  <a href="../Keywords.sdf3/#java/lexical/Keywords_1_8" id="java/lexical/Keywords_7_3" title="a reference to a single-file definition">java/lexical/Keywords</a>

<span class="keyword">lexical start-symbols</span>
  
  <a href="#ID_19_3" id="ID_11_3" title="a reference to a single-file definition">ID</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Id_15_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Id line 37_33; ../../classes/ConstructorDeclarations.sdf3/#Id line 25_51; ../../classes/EnumDeclarations.sdf3/#Id line 21_32, 26_32, 31_24, 35_24; ../../classes/FieldDeclarations.sdf3/#Id line 31_33, 32_35, 59_54, 60_91; ../../classes/MethodDeclarations.sdf3/#Id line 34_13, 37_50, 59_71; ../../expressions/ClassInstanceCreation.sdf3/#Id line 24_45, 27_45, 31_52; ../../expressions/FieldAccess.sdf3/#Id line 18_44, 19_37, 20_48; ../../expressions/LambdaExpressions.sdf3/#Id line 19_42, 21_46; ../../expressions/MethodInvocation.sdf3/#Id line 16_64, 17_57, 18_68; ../../expressions/MethodReference.sdf3/#Id line 14_73, 15_70, 16_63, 17_74; ../../interfaces/Annotations.sdf3/#Id line 23_36; ../../interfaces/AnnotationTypes.sdf3/#Id line 27_42, 38_55; ../../interfaces/InterfaceDeclarations.sdf3/#Id line 27_41; ../../names/Names.sdf3/#Id line 19_41, 20_57, 21_41, 22_63, 23_41, 24_63, 25_41, 26_59, 27_41, 28_59, 29_41; ../../packages/ImportDeclarations.sdf3/#Id line 17_71; ../../packages/PackageDeclarations.sdf3/#Id line 15_74; ../../statements/Statements.sdf3/#Id line 34_25, 84_29, 87_35; ../../types/ReferenceTypes.sdf3/#Id line 26_64, 27_76, 35_48; ../../types/TypeVariable.sdf3/#Id line 16_62, 17_62">Id</button>

<span class="keyword">lexical sorts</span>
  
  <button class="modal-open" id="ID_19_3" title="a definition with multiple references" data-urls="#ID line 11_3, 23_11, 35_3; ../../Test.sdf3/#ID line 25_7, 31_7">ID</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Id_23_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Id line 37_33; ../../classes/ConstructorDeclarations.sdf3/#Id line 25_51; ../../classes/EnumDeclarations.sdf3/#Id line 21_32, 26_32, 31_24, 35_24; ../../classes/FieldDeclarations.sdf3/#Id line 31_33, 32_35, 59_54, 60_91; ../../classes/MethodDeclarations.sdf3/#Id line 34_13, 37_50, 59_71; ../../expressions/ClassInstanceCreation.sdf3/#Id line 24_45, 27_45, 31_52; ../../expressions/FieldAccess.sdf3/#Id line 18_44, 19_37, 20_48; ../../expressions/LambdaExpressions.sdf3/#Id line 19_42, 21_46; ../../expressions/MethodInvocation.sdf3/#Id line 16_64, 17_57, 18_68; ../../expressions/MethodReference.sdf3/#Id line 14_73, 15_70, 16_63, 17_74; ../../interfaces/Annotations.sdf3/#Id line 23_36; ../../interfaces/AnnotationTypes.sdf3/#Id line 27_42, 38_55; ../../interfaces/InterfaceDeclarations.sdf3/#Id line 27_41; ../../names/Names.sdf3/#Id line 19_41, 20_57, 21_41, 22_63, 23_41, 24_63, 25_41, 26_59, 27_41, 28_59, 29_41; ../../packages/ImportDeclarations.sdf3/#Id line 17_71; ../../packages/PackageDeclarations.sdf3/#Id line 15_74; ../../statements/Statements.sdf3/#Id line 34_25, 84_29, 87_35; ../../types/ReferenceTypes.sdf3/#Id line 26_64, 27_76, 35_48; ../../types/TypeVariable.sdf3/#Id line 16_62, 17_62">Id</button>.<span class="cons_Constructor"><span id="Id_23_6" title="a definition with no references">Id</span></span> = <a href="#ID_19_3" id="ID_23_11" title="a reference to a single-file definition">ID</a>

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="ID_27_3" title="a definition with multiple references" data-urls="#ID line 11_3, 23_11, 35_3; ../../Test.sdf3/#ID line 25_7, 31_7">ID</button> = [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span>\_\$] [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]*
  <button class="modal-open" id="ID_28_3" title="a definition with multiple references" data-urls="#ID line 11_3, 23_11, 35_3; ../../Test.sdf3/#ID line 25_7, 31_7">ID</button> = <a href="../Keywords.sdf3/#Keyword_7_3" id="Keyword_28_8" title="a reference to a single-file definition">Keyword</a> {<span class="keyword">reject</span>}
  <button class="modal-open" id="ID_29_3" title="a definition with multiple references" data-urls="#ID line 11_3, 23_11, 35_3; ../../Test.sdf3/#ID line 25_7, 31_7">ID</button> = <span class="cons_Lit">"true"</span> {<span class="keyword">reject</span>}
  <button class="modal-open" id="ID_30_3" title="a definition with multiple references" data-urls="#ID line 11_3, 23_11, 35_3; ../../Test.sdf3/#ID line 25_7, 31_7">ID</button> = <span class="cons_Lit">"false"</span> {<span class="keyword">reject</span>}
  <button class="modal-open" id="ID_31_3" title="a definition with multiple references" data-urls="#ID line 11_3, 23_11, 35_3; ../../Test.sdf3/#ID line 25_7, 31_7">ID</button> = <span class="cons_Lit">"null"</span> {<span class="keyword">reject</span>}

<span class="keyword">lexical restrictions</span>

  <a href="#ID_19_3" id="ID_35_3" title="a reference to a single-file definition">ID</a> -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
