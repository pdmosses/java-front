---
title: InterfaceDeclarations.sdf3
---

# `InterfaceDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/interfaces/InterfaceDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/interfaces/InterfaceDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/interfaces/InterfaceDeclarations.sdf3 "The source file on GitHub"

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
36
37
38
39
40
41
42
43
44
45
46
47
48
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../packages/TypeDeclarations.sdf3#java/interfaces/InterfaceDeclarations_144_181" id="java/interfaces/InterfaceDeclarations_7_44" title="Referenced at ../../packages/TypeDeclarations.sdf3 line 8">java/interfaces/InterfaceDeclarations</a>

<span class="layout">// 9.1. Interface Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_88_112" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_115_137" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../lexical/SemiColon.sdf3#java/lexical/SemiColon_7_29" id="java/lexical/SemiColon_140_162" title="Defined at ../../lexical/SemiColon.sdf3 line 1">java/lexical/SemiColon</a>
  <a href="../../classes/ClassDeclarations.sdf3#java/classes/ClassDeclarations_7_37" id="java/classes/ClassDeclarations_165_195" title="Defined at ../../classes/ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_198_223" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_226_253" title="Defined at ../Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../ConstantDeclarations.sdf3#java/interfaces/ConstantDeclarations_7_43" id="java/interfaces/ConstantDeclarations_256_292" title="Defined at ../ConstantDeclarations.sdf3 line 1">java/interfaces/ConstantDeclarations</a>
  <a href="../InterfaceMethodDeclarations.sdf3#java/interfaces/InterfaceMethodDeclarations_7_50" id="java/interfaces/InterfaceMethodDeclarations_295_338" title="Defined at ../InterfaceMethodDeclarations.sdf3 line 1">java/interfaces/InterfaceMethodDeclarations</a>
  <a href="../AnnotationTypes.sdf3#java/interfaces/AnnotationTypes_7_38" id="java/interfaces/AnnotationTypes_341_372" title="Defined at ../AnnotationTypes.sdf3 line 1">java/interfaces/AnnotationTypes</a>

<span class="keyword">context-free sorts</span>

  <a href="#InterfaceDeclaration_1220_1240" id="InterfaceDeclaration_396_416" title="Referenced at line 46; ../AnnotationTypes.sdf3 line 34; ../../classes/ClassDeclarations.sdf3 line 66; ../../packages/TypeDeclarations.sdf3 line 17">InterfaceDeclaration</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_419_436" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a>
  <a href="#ExtendsInterfaces_616_633" id="ExtendsInterfaces_439_456" title="Referenced at line 27">ExtendsInterfaces</a>
  <a href="#InterfaceMemberDeclaration_644_670" id="InterfaceMemberDeclaration_459_485" title="Referenced at line 28">InterfaceMemberDeclaration</a>

<span class="keyword">context-free syntax</span>

  
  <a href="#InterfaceDeclaration_1220_1240" id="InterfaceDeclaration_513_533" title="Referenced at line 46; ../AnnotationTypes.sdf3 line 34; ../../classes/ClassDeclarations.sdf3 line 66; ../../packages/TypeDeclarations.sdf3 line 17">InterfaceDeclaration</a>.<span class="cons_Constructor"><span id="NormalInterface_534_549" title="Not referenced locally, nor via imports">NormalInterface</span></span> = &lt;
  &lt;{<a href="#InterfaceModifier_419_436" id="InterfaceModifier_558_575" title="Defined at line 19, 33, 34, 35, 36, 37, 38, 39">InterfaceModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">interface</span> &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_594_596" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../classes/ClassDeclarations.sdf3#TypeParameters_567_581" id="TypeParameters_598_612" title="Defined at ../../classes/ClassDeclarations.sdf3 line 25, 50">TypeParameters</a>?&gt; &lt;<a href="#ExtendsInterfaces_439_456" id="ExtendsInterfaces_616_633" title="Defined at line 20, 41">ExtendsInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#InterfaceMemberDeclaration_459_485" id="InterfaceMemberDeclaration_644_670" title="Defined at line 21, 43, 44, 45, 46, 47">InterfaceMemberDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#InterfaceDeclaration_1220_1240" id="InterfaceDeclaration_689_709" title="Referenced at line 46; ../AnnotationTypes.sdf3 line 34; ../../classes/ClassDeclarations.sdf3 line 66; ../../packages/TypeDeclarations.sdf3 line 17">InterfaceDeclaration</a> = <a href="../AnnotationTypes.sdf3#AnnotationTypeDeclaration_377_402" id="AnnotationTypeDeclaration_712_737" title="Defined at ../AnnotationTypes.sdf3 line 18, 26">AnnotationTypeDeclaration</a>
  
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_743_760" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../Annotations.sdf3#Annotation_158_168" id="Annotation_763_773" title="Defined at ../Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_776_793" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../../lexical/Modifiers.sdf3#Public_201_207" id="Public_796_802" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_805_822" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../../lexical/Modifiers.sdf3#Protected_189_198" id="Protected_825_834" title="Defined at ../../lexical/Modifiers.sdf3 line 13, 28">Protected</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_837_854" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../../lexical/Modifiers.sdf3#Private_179_186" id="Private_857_864" title="Defined at ../../lexical/Modifiers.sdf3 line 12, 27">Private</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_867_884" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../../lexical/Modifiers.sdf3#Abstract_141_149" id="Abstract_887_895" title="Defined at ../../lexical/Modifiers.sdf3 line 8, 23">Abstract</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_898_915" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../../lexical/Modifiers.sdf3#Static_210_216" id="Static_918_924" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#InterfaceModifier_558_575" id="InterfaceModifier_927_944" title="Referenced at line 27; ../AnnotationTypes.sdf3 line 27">InterfaceModifier</a> = <a href="../../lexical/Modifiers.sdf3#Strictfp_219_227" id="Strictfp_947_955" title="Defined at ../../lexical/Modifiers.sdf3 line 16, 31">Strictfp</a>
  
  <a href="#ExtendsInterfaces_616_633" id="ExtendsInterfaces_961_978" title="Referenced at line 27">ExtendsInterfaces</a>.<span class="cons_Constructor"><span id="ExtendsInterfaces_979_996" title="Not referenced locally, nor via imports">ExtendsInterfaces</span></span> = &lt;<span class="cons_String">extends</span> &lt;{<a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_1010_1019" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#InterfaceMemberDeclaration_644_670" id="InterfaceMemberDeclaration_1034_1060" title="Referenced at line 28">InterfaceMemberDeclaration</a> = <a href="../ConstantDeclarations.sdf3#ConstantDeclaration_203_222" id="ConstantDeclaration_1063_1082" title="Defined at ../ConstantDeclarations.sdf3 line 12, 17">ConstantDeclaration</a>
  <a href="#InterfaceMemberDeclaration_644_670" id="InterfaceMemberDeclaration_1085_1111" title="Referenced at line 28">InterfaceMemberDeclaration</a> = <a href="../InterfaceMethodDeclarations.sdf3#InterfaceMethodDeclaration_201_227" id="InterfaceMethodDeclaration_1114_1140" title="Defined at ../InterfaceMethodDeclarations.sdf3 line 12, 17">InterfaceMethodDeclaration</a>
  <a href="#InterfaceMemberDeclaration_644_670" id="InterfaceMemberDeclaration_1143_1169" title="Referenced at line 28">InterfaceMemberDeclaration</a> = <a href="../../classes/ClassDeclarations.sdf3#ClassDeclaration_507_523" id="ClassDeclaration_1172_1188" title="Defined at ../../classes/ClassDeclarations.sdf3 line 22, 33, 34">ClassDeclaration</a>
  <a href="#InterfaceMemberDeclaration_644_670" id="InterfaceMemberDeclaration_1191_1217" title="Referenced at line 28">InterfaceMemberDeclaration</a> = <a href="#InterfaceDeclaration_396_416" id="InterfaceDeclaration_1220_1240" title="Defined at line 18, 26, 31">InterfaceDeclaration</a>
  <a href="#InterfaceMemberDeclaration_644_670" id="InterfaceMemberDeclaration_1243_1269" title="Referenced at line 28">InterfaceMemberDeclaration</a> = <a href="../../lexical/SemiColon.sdf3#SemiColon_132_141" id="SemiColon_1272_1281" title="Defined at ../../lexical/SemiColon.sdf3 line 8, 12">SemiColon</a>
  
</code></pre></td></tr></tbody></table></div>