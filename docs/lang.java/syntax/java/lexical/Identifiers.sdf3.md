---
title: Identifiers.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../types/TypeVariable.sdf3#java/lexical/Identifiers_94_118" id="java/lexical/Identifiers_7_31" title="Referenced at ../../types/TypeVariable.sdf3 line 7">java/lexical/Identifiers</a>

<span class="layout">// 3.8. Identifiers</span>

<span class="keyword">imports</span>

  <a href="../Keywords.sdf3#java/lexical/Keywords_7_28" id="java/lexical/Keywords_65_86" title="Defined at ../Keywords.sdf3 line 1">java/lexical/Keywords</a>

<span class="keyword">lexical start-symbols</span>
  
  <a href="#ID_164_166" id="ID_115_117" title="Defined at line 19, 27, 28, 29, 30, 31">ID</a>

<span class="keyword">context-free sorts</span>

  <a href="../../classes/ClassDeclarations.sdf3#Id_848_850" id="Id_141_143" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 37; ../../classes/ConstructorDeclarations.sdf3 line 25; ../../classes/EnumDeclarations.sdf3 line 35; ../../classes/FieldDeclarations.sdf3 line 60; ../../classes/MethodDeclarations.sdf3 line 59; ../../expressions/ClassInstanceCreation.sdf3 line 31; ../../expressions/FieldAccess.sdf3 line 20; ../../expressions/LambdaExpressions.sdf3 line 21; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 17; ../../interfaces/Annotations.sdf3 line 23; ../../interfaces/AnnotationTypes.sdf3 line 38; ../../interfaces/InterfaceDeclarations.sdf3 line 27; ../../names/Names.sdf3 line 29; ../../packages/ImportDeclarations.sdf3 line 17; ../../packages/PackageDeclarations.sdf3 line 15; ../../statements/Statements.sdf3 line 87; ../../types/ReferenceTypes.sdf3 line 35; ../../types/TypeVariable.sdf3 line 17">Id</a>

<span class="keyword">lexical sorts</span>
  
  <a href="#ID_375_377" id="ID_164_166" title="Referenced at line 35; ../../Test.sdf3 line 31">ID</a>

<span class="keyword">context-free syntax</span>

  <a href="../../classes/ClassDeclarations.sdf3#Id_848_850" id="Id_191_193" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 37; ../../classes/ConstructorDeclarations.sdf3 line 25; ../../classes/EnumDeclarations.sdf3 line 35; ../../classes/FieldDeclarations.sdf3 line 60; ../../classes/MethodDeclarations.sdf3 line 59; ../../expressions/ClassInstanceCreation.sdf3 line 31; ../../expressions/FieldAccess.sdf3 line 20; ../../expressions/LambdaExpressions.sdf3 line 21; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 17; ../../interfaces/Annotations.sdf3 line 23; ../../interfaces/AnnotationTypes.sdf3 line 38; ../../interfaces/InterfaceDeclarations.sdf3 line 27; ../../names/Names.sdf3 line 29; ../../packages/ImportDeclarations.sdf3 line 17; ../../packages/PackageDeclarations.sdf3 line 15; ../../statements/Statements.sdf3 line 87; ../../types/ReferenceTypes.sdf3 line 35; ../../types/TypeVariable.sdf3 line 17">Id</a>.<span class="cons_Constructor"><span id="Id_194_196" title="Not referenced locally, nor via imports">Id</span></span> = <a href="#ID_164_166" id="ID_199_201" title="Defined at line 19, 27, 28, 29, 30, 31">ID</a>

<span class="keyword">lexical syntax</span>

  <a href="#ID_375_377" id="ID_221_223" title="Referenced at line 35; ../../Test.sdf3 line 31">ID</a> = [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span>\_\$] [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]*
  <a href="#ID_375_377" id="ID_258_260" title="Referenced at line 35; ../../Test.sdf3 line 31">ID</a> = <a href="../Keywords.sdf3#Keyword_66_73" id="Keyword_263_270" title="Defined at ../Keywords.sdf3 line 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56">Keyword</a> {<span class="keyword">reject</span>}
  <a href="#ID_375_377" id="ID_282_284" title="Referenced at line 35; ../../Test.sdf3 line 31">ID</a> = <span class="cons_Lit">"true"</span> {<span class="keyword">reject</span>}
  <a href="#ID_375_377" id="ID_305_307" title="Referenced at line 35; ../../Test.sdf3 line 31">ID</a> = <span class="cons_Lit">"false"</span> {<span class="keyword">reject</span>}
  <a href="#ID_375_377" id="ID_329_331" title="Referenced at line 35; ../../Test.sdf3 line 31">ID</a> = <span class="cons_Lit">"null"</span> {<span class="keyword">reject</span>}

<span class="keyword">lexical restrictions</span>

  <a href="#ID_164_166" id="ID_375_377" title="Defined at line 19, 27, 28, 29, 30, 31">ID</a> -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]
</code></pre></td></tr></tbody></table></div>