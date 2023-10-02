---
title: ClassDeclarations.sdf3
hide:
  - toc
---

# `ClassDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/classes/ClassDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/classes/ClassDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/classes/ClassDeclarations.sdf3 "The source file on GitHub"

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
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../statements/Blocks.sdf3#java/classes/ClassDeclarations_58_88" id="java/classes/ClassDeclarations_7_37" title="Referenced at ../../statements/Blocks.sdf3 line 6">java/classes/ClassDeclarations</a>

<span class="layout">// 8.1. Class Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_77_101" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_104_126" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../lexical/SemiColon.sdf3#java/lexical/SemiColon_7_29" id="java/lexical/SemiColon_129_151" title="Defined at ../../lexical/SemiColon.sdf3 line 1">java/lexical/SemiColon</a>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_154_179" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../FieldDeclarations.sdf3#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_182_212" title="Defined at ../FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../MethodDeclarations.sdf3#java/classes/MethodDeclarations_7_38" id="java/classes/MethodDeclarations_215_246" title="Defined at ../MethodDeclarations.sdf3 line 1">java/classes/MethodDeclarations</a>
  <a href="../InstanceInitializers.sdf3#java/classes/InstanceInitializers_7_40" id="java/classes/InstanceInitializers_249_282" title="Defined at ../InstanceInitializers.sdf3 line 1">java/classes/InstanceInitializers</a>
  <a href="../StaticInitializers.sdf3#java/classes/StaticInitializers_7_38" id="java/classes/StaticInitializers_285_316" title="Defined at ../StaticInitializers.sdf3 line 1">java/classes/StaticInitializers</a>
  <a href="../EnumDeclarations.sdf3#java/classes/EnumDeclarations_7_36" id="java/classes/EnumDeclarations_319_348" title="Defined at ../EnumDeclarations.sdf3 line 1">java/classes/EnumDeclarations</a>
  <a href="../ConstructorDeclarations.sdf3#java/classes/ConstructorDeclarations_7_43" id="java/classes/ConstructorDeclarations_351_387" title="Defined at ../ConstructorDeclarations.sdf3 line 1">java/classes/ConstructorDeclarations</a>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_390_417" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../interfaces/InterfaceDeclarations.sdf3#java/interfaces/InterfaceDeclarations_7_44" id="java/interfaces/InterfaceDeclarations_420_457" title="Defined at ../../interfaces/InterfaceDeclarations.sdf3 line 1">java/interfaces/InterfaceDeclarations</a>
  <a href="../../types/TypeVariable.sdf3#java/types/TypeVariable_7_30" id="java/types/TypeVariable_460_483" title="Defined at ../../types/TypeVariable.sdf3 line 1">java/types/TypeVariable</a>

<span class="keyword">context-free sorts</span>

  <a href="#ClassDeclaration_1737_1753" id="ClassDeclaration_507_523" title="Referenced at line 65; ../../interfaces/AnnotationTypes.sdf3 line 33; ../../interfaces/InterfaceDeclarations.sdf3 line 45; ../../packages/TypeDeclarations.sdf3 line 16; ../../statements/Blocks.sdf3 line 22">ClassDeclaration</a>
  <a href="#NormalClassDeclaration_706_728" id="NormalClassDeclaration_526_548" title="Referenced at line 33">NormalClassDeclaration</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_551_564" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a>
  <a href="#TypeParameters_852_866" id="TypeParameters_567_581" title="Referenced at line 37; ../ConstructorDeclarations.sdf3 line 25; ../MethodDeclarations.sdf3 line 37; ../../interfaces/InterfaceDeclarations.sdf3 line 27">TypeParameters</a>
  <a href="#SuperClass_870_880" id="SuperClass_584_594" title="Referenced at line 37">SuperClass</a>
  <a href="#SuperInterfaces_884_899" id="SuperInterfaces_597_612" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">SuperInterfaces</a>
  <a href="#ClassBodyDeclaration_910_930" id="ClassBodyDeclaration_615_635" title="Referenced at line 38; ../EnumDeclarations.sdf3 line 38; ../../expressions/ClassInstanceCreation.sdf3 line 28">ClassBodyDeclaration</a>
  <a href="#ClassMemberDeclaration_1456_1478" id="ClassMemberDeclaration_638_660" title="Referenced at line 58">ClassMemberDeclaration</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#ClassDeclaration_1737_1753" id="ClassDeclaration_687_703" title="Referenced at line 65; ../../interfaces/AnnotationTypes.sdf3 line 33; ../../interfaces/InterfaceDeclarations.sdf3 line 45; ../../packages/TypeDeclarations.sdf3 line 16; ../../statements/Blocks.sdf3 line 22">ClassDeclaration</a> = <a href="#NormalClassDeclaration_526_548" id="NormalClassDeclaration_706_728" title="Defined at line 23, 36">NormalClassDeclaration</a>
  <a href="#ClassDeclaration_1737_1753" id="ClassDeclaration_731_747" title="Referenced at line 65; ../../interfaces/AnnotationTypes.sdf3 line 33; ../../interfaces/InterfaceDeclarations.sdf3 line 45; ../../packages/TypeDeclarations.sdf3 line 16; ../../statements/Blocks.sdf3 line 22">ClassDeclaration</a>  = <a href="../EnumDeclarations.sdf3#EnumDeclaration_203_218" id="EnumDeclaration_751_766" title="Defined at ../EnumDeclarations.sdf3 line 13, 20, 25">EnumDeclaration</a>
  
  <a href="#NormalClassDeclaration_706_728" id="NormalClassDeclaration_772_794" title="Referenced at line 33">NormalClassDeclaration</a>.<span class="cons_Constructor"><span id="ClassDeclaration_795_811" title="Not referenced locally, nor via imports">ClassDeclaration</span></span> = &lt;
  &lt;{<a href="#ClassModifier_551_564" id="ClassModifier_820_833" title="Defined at line 24, 41, 42, 43, 44, 45, 46, 47, 48">ClassModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">class</span> &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_848_850" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="#TypeParameters_567_581" id="TypeParameters_852_866" title="Defined at line 25, 50">TypeParameters</a>?&gt; &lt;<a href="#SuperClass_584_594" id="SuperClass_870_880" title="Defined at line 26, 54">SuperClass</a>?&gt; &lt;<a href="#SuperInterfaces_597_612" id="SuperInterfaces_884_899" title="Defined at line 27, 56">SuperInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#ClassBodyDeclaration_615_635" id="ClassBodyDeclaration_910_930" title="Defined at line 28, 58, 59, 60, 61">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#ClassModifier_820_833" id="ClassModifier_949_962" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_965_975" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_978_991" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Public_201_207" id="Public_994_1000" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_1003_1016" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Protected_189_198" id="Protected_1019_1028" title="Defined at ../../lexical/Modifiers.sdf3 line 13, 28">Protected</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_1031_1044" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Private_179_186" id="Private_1047_1054" title="Defined at ../../lexical/Modifiers.sdf3 line 12, 27">Private</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_1057_1070" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Abstract_141_149" id="Abstract_1073_1081" title="Defined at ../../lexical/Modifiers.sdf3 line 8, 23">Abstract</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_1084_1097" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Static_210_216" id="Static_1100_1106" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_1109_1122" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Final_162_167" id="Final_1125_1130" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  <a href="#ClassModifier_820_833" id="ClassModifier_1133_1146" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">ClassModifier</a> = <a href="../../lexical/Modifiers.sdf3#Strictfp_219_227" id="Strictfp_1149_1157" title="Defined at ../../lexical/Modifiers.sdf3 line 16, 31">Strictfp</a>
  
  <a href="#TypeParameters_852_866" id="TypeParameters_1163_1177" title="Referenced at line 37; ../ConstructorDeclarations.sdf3 line 25; ../MethodDeclarations.sdf3 line 37; ../../interfaces/InterfaceDeclarations.sdf3 line 27">TypeParameters</a>.<span class="cons_Constructor"><span id="TypeParameters_1178_1192" title="Not referenced locally, nor via imports">TypeParameters</span></span>               = [<span class="cons_String">&lt;</span>[{<a href="../../types/TypeVariable.sdf3#TypeParameter_172_185" id="TypeParameter_1213_1226" title="Defined at ../../types/TypeVariable.sdf3 line 12, 16, 17">TypeParameter</a> <span class="cons_Lit">","</span>}+]<span class="cons_String">&gt;</span>]

  <span class="layout">// TypeParameter is already defined in 4.4 / java/types/TypeVariable</span>

  <a href="#SuperClass_870_880" id="SuperClass_1311_1321" title="Referenced at line 37">SuperClass</a>.<span class="cons_Constructor"><span id="SuperClass_1322_1332" title="Not referenced locally, nor via imports">SuperClass</span></span> = &lt;<span class="cons_String">extends</span> &lt;<a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_1345_1354" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>&gt;&gt;
  
  <a href="#SuperInterfaces_884_899" id="SuperInterfaces_1362_1377" title="Referenced at line 37; ../EnumDeclarations.sdf3 line 26">SuperInterfaces</a>.<span class="cons_Constructor"><span id="SuperInterface_1378_1392" title="Not referenced locally, nor via imports">SuperInterface</span></span> = &lt;<span class="cons_String">implements</span> &lt;{<a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_1409_1418" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#ClassBodyDeclaration_910_930" id="ClassBodyDeclaration_1433_1453" title="Referenced at line 38; ../EnumDeclarations.sdf3 line 38; ../../expressions/ClassInstanceCreation.sdf3 line 28">ClassBodyDeclaration</a> = <a href="#ClassMemberDeclaration_638_660" id="ClassMemberDeclaration_1456_1478" title="Defined at line 29, 63, 64, 65, 66, 67">ClassMemberDeclaration</a>
  <a href="#ClassBodyDeclaration_910_930" id="ClassBodyDeclaration_1481_1501" title="Referenced at line 38; ../EnumDeclarations.sdf3 line 38; ../../expressions/ClassInstanceCreation.sdf3 line 28">ClassBodyDeclaration</a>  = <a href="../InstanceInitializers.sdf3#InstanceInitializer_129_148" id="InstanceInitializer_1505_1524" title="Defined at ../InstanceInitializers.sdf3 line 10, 14">InstanceInitializer</a>
  <a href="#ClassBodyDeclaration_910_930" id="ClassBodyDeclaration_1527_1547" title="Referenced at line 38; ../EnumDeclarations.sdf3 line 38; ../../expressions/ClassInstanceCreation.sdf3 line 28">ClassBodyDeclaration</a>  = <a href="../StaticInitializers.sdf3#StaticInitializer_127_144" id="StaticInitializer_1551_1568" title="Defined at ../StaticInitializers.sdf3 line 10, 14">StaticInitializer</a>
  <a href="#ClassBodyDeclaration_910_930" id="ClassBodyDeclaration_1571_1591" title="Referenced at line 38; ../EnumDeclarations.sdf3 line 38; ../../expressions/ClassInstanceCreation.sdf3 line 28">ClassBodyDeclaration</a>  = <a href="../ConstructorDeclarations.sdf3#ConstructorDeclaration_359_381" id="ConstructorDeclaration_1595_1617" title="Defined at ../ConstructorDeclarations.sdf3 line 18, 24">ConstructorDeclaration</a>
  
  <a href="#ClassMemberDeclaration_1456_1478" id="ClassMemberDeclaration_1623_1645" title="Referenced at line 58">ClassMemberDeclaration</a> = <a href="../FieldDeclarations.sdf3#FieldDeclaration_324_340" id="FieldDeclaration_1648_1664" title="Defined at ../FieldDeclarations.sdf3 line 17, 30">FieldDeclaration</a>
  <a href="#ClassMemberDeclaration_1456_1478" id="ClassMemberDeclaration_1667_1689" title="Referenced at line 58">ClassMemberDeclaration</a> = <a href="../MethodDeclarations.sdf3#MethodDeclaration_300_317" id="MethodDeclaration_1692_1709" title="Defined at ../MethodDeclarations.sdf3 line 15, 30">MethodDeclaration</a>
  <a href="#ClassMemberDeclaration_1456_1478" id="ClassMemberDeclaration_1712_1734" title="Referenced at line 58">ClassMemberDeclaration</a> = <a href="#ClassDeclaration_507_523" id="ClassDeclaration_1737_1753" title="Defined at line 22, 33, 34">ClassDeclaration</a>
  <a href="#ClassMemberDeclaration_1456_1478" id="ClassMemberDeclaration_1756_1778" title="Referenced at line 58">ClassMemberDeclaration</a> = <a href="../../interfaces/InterfaceDeclarations.sdf3#InterfaceDeclaration_396_416" id="InterfaceDeclaration_1781_1801" title="Defined at ../../interfaces/InterfaceDeclarations.sdf3 line 18, 26, 31">InterfaceDeclaration</a>
  <a href="#ClassMemberDeclaration_1456_1478" id="ClassMemberDeclaration_1804_1826" title="Referenced at line 58">ClassMemberDeclaration</a> = <a href="../../lexical/SemiColon.sdf3#SemiColon_132_141" id="SemiColon_1829_1838" title="Defined at ../../lexical/SemiColon.sdf3 line 8, 12">SemiColon</a>
</code></pre></td></tr></tbody></table></div>