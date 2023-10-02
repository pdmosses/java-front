---
title: AnnotationTypes.sdf3
hide:
  - toc
---

# `AnnotationTypes.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/interfaces/AnnotationTypes.sdf3]

[pdmosses/java-front/lang.java/syntax/java/interfaces/AnnotationTypes.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/interfaces/AnnotationTypes.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/interfaces/AnnotationTypes_151_182" id="java/interfaces/AnnotationTypes_7_38" title="Referenced at ../Main.sdf3 line 8">java/interfaces/AnnotationTypes</a>

<span class="layout">// 9.6. Annotation Types</span>

<span class="keyword">imports</span>
  <a href="../InterfaceDeclarations.sdf3#java/interfaces/InterfaceDeclarations_7_44" id="java/interfaces/InterfaceDeclarations_76_113" title="Defined at ../InterfaceDeclarations.sdf3 line 1">java/interfaces/InterfaceDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_116_140" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_143_165" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../lexical/SemiColon.sdf3#java/lexical/SemiColon_7_29" id="java/lexical/SemiColon_168_190" title="Defined at ../../lexical/SemiColon.sdf3 line 1">java/lexical/SemiColon</a>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_193_218" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../classes/FieldDeclarations.sdf3#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_221_251" title="Defined at ../../classes/FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../ConstantDeclarations.sdf3#java/interfaces/ConstantDeclarations_7_43" id="java/interfaces/ConstantDeclarations_254_290" title="Defined at ../ConstantDeclarations.sdf3 line 1">java/interfaces/ConstantDeclarations</a>
  <a href="../../classes/ClassDeclarations.sdf3#java/classes/ClassDeclarations_7_37" id="java/classes/ClassDeclarations_293_323" title="Defined at ../../classes/ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_326_353" title="Defined at ../Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../InterfaceDeclarations.sdf3#AnnotationTypeDeclaration_712_737" id="AnnotationTypeDeclaration_377_402" title="Referenced at ../InterfaceDeclarations.sdf3 line 31">AnnotationTypeDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_636_667" id="AnnotationTypeMemberDeclaration_405_436" title="Referenced at line 28">AnnotationTypeMemberDeclaration</a>
  <a href="#AnnotationTypeElementDeclaration_720_752" id="AnnotationTypeElementDeclaration_439_471" title="Referenced at line 31">AnnotationTypeElementDeclaration</a>
  <a href="#AnnotationTypeElementModifier_1037_1066" id="AnnotationTypeElementModifier_474_503" title="Referenced at line 38">AnnotationTypeElementModifier</a>
  <a href="#DefaultValue_1115_1127" id="DefaultValue_506_518" title="Referenced at line 38">DefaultValue</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../InterfaceDeclarations.sdf3#AnnotationTypeDeclaration_712_737" id="AnnotationTypeDeclaration_545_570" title="Referenced at ../InterfaceDeclarations.sdf3 line 31">AnnotationTypeDeclaration</a>.<span class="cons_Constructor"><span id="AnnoDec_571_578" title="Not referenced locally, nor via imports">AnnoDec</span></span> = &lt;
  &lt;{<a href="../InterfaceDeclarations.sdf3#InterfaceModifier_419_436" id="InterfaceModifier_587_604" title="Defined at ../InterfaceDeclarations.sdf3 line 19, 33, 34, 35, 36, 37, 38, 39">InterfaceModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">@interface</span> &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_624_626" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; <span class="cons_String">{</span>
    &lt;{<a href="#AnnotationTypeMemberDeclaration_405_436" id="AnnotationTypeMemberDeclaration_636_667" title="Defined at line 19, 31, 32, 33, 34, 35">AnnotationTypeMemberDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#AnnotationTypeMemberDeclaration_636_667" id="AnnotationTypeMemberDeclaration_686_717" title="Referenced at line 28">AnnotationTypeMemberDeclaration</a> = <a href="#AnnotationTypeElementDeclaration_439_471" id="AnnotationTypeElementDeclaration_720_752" title="Defined at line 20, 37">AnnotationTypeElementDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_636_667" id="AnnotationTypeMemberDeclaration_755_786" title="Referenced at line 28">AnnotationTypeMemberDeclaration</a> = <a href="../ConstantDeclarations.sdf3#ConstantDeclaration_203_222" id="ConstantDeclaration_789_808" title="Defined at ../ConstantDeclarations.sdf3 line 12, 17">ConstantDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_636_667" id="AnnotationTypeMemberDeclaration_811_842" title="Referenced at line 28">AnnotationTypeMemberDeclaration</a> = <a href="../../classes/ClassDeclarations.sdf3#ClassDeclaration_507_523" id="ClassDeclaration_845_861" title="Defined at ../../classes/ClassDeclarations.sdf3 line 22, 33, 34">ClassDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_636_667" id="AnnotationTypeMemberDeclaration_864_895" title="Referenced at line 28">AnnotationTypeMemberDeclaration</a> = <a href="../InterfaceDeclarations.sdf3#InterfaceDeclaration_396_416" id="InterfaceDeclaration_898_918" title="Defined at ../InterfaceDeclarations.sdf3 line 18, 26, 31">InterfaceDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_636_667" id="AnnotationTypeMemberDeclaration_921_952" title="Referenced at line 28">AnnotationTypeMemberDeclaration</a> = <a href="../../lexical/SemiColon.sdf3#SemiColon_132_141" id="SemiColon_955_964" title="Defined at ../../lexical/SemiColon.sdf3 line 8, 12">SemiColon</a>
  
  <a href="#AnnotationTypeElementDeclaration_720_752" id="AnnotationTypeElementDeclaration_970_1002" title="Referenced at line 31">AnnotationTypeElementDeclaration</a>.<span class="cons_Constructor"><span id="AnnotationTypeElementDecl_1003_1028" title="Not referenced locally, nor via imports">AnnotationTypeElementDecl</span></span> = &lt;
  &lt;{<a href="#AnnotationTypeElementModifier_474_503" id="AnnotationTypeElementModifier_1037_1066" title="Defined at line 21, 40, 41, 42">AnnotationTypeElementModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#UnannType_403_412" id="UnannType_1075_1084" title="Defined at ../../classes/FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_1087_1089" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">()</span> &lt;<a href="../../types/ReferenceTypes.sdf3#AnnotatedDimsEmpty_289_307" id="AnnotatedDimsEmpty_1094_1112" title="Defined at ../../types/ReferenceTypes.sdf3 line 18, 40">AnnotatedDimsEmpty</a>&gt; &lt;<a href="#DefaultValue_506_518" id="DefaultValue_1115_1127" title="Defined at line 22, 44">DefaultValue</a>?&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#AnnotationTypeElementModifier_1037_1066" id="AnnotationTypeElementModifier_1137_1166" title="Referenced at line 38">AnnotationTypeElementModifier</a> = <a href="../Annotations.sdf3#Annotation_158_168" id="Annotation_1169_1179" title="Defined at ../Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#AnnotationTypeElementModifier_1037_1066" id="AnnotationTypeElementModifier_1182_1211" title="Referenced at line 38">AnnotationTypeElementModifier</a> = <a href="../../lexical/Modifiers.sdf3#Public_201_207" id="Public_1214_1220" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#AnnotationTypeElementModifier_1037_1066" id="AnnotationTypeElementModifier_1223_1252" title="Referenced at line 38">AnnotationTypeElementModifier</a> = <a href="../../lexical/Modifiers.sdf3#Abstract_141_149" id="Abstract_1255_1263" title="Defined at ../../lexical/Modifiers.sdf3 line 8, 23">Abstract</a>
  
  <a href="#DefaultValue_1115_1127" id="DefaultValue_1269_1281" title="Referenced at line 38">DefaultValue</a>.<span class="cons_Constructor"><span id="DefaultVal_1282_1292" title="Not referenced locally, nor via imports">DefaultVal</span></span> = &lt;<span class="cons_String">default</span> &lt;<a href="../Annotations.sdf3#ElementValue_190_202" id="ElementValue_1305_1317" title="Defined at ../Annotations.sdf3 line 14, 24, 25, 26">ElementValue</a>&gt;&gt;
</code></pre></td></tr></tbody></table></div>