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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/classes/ClassDeclarations_1_8" title="a definition with multiple references" data-urls="../ConstructorDeclarations.sdf3/#java/classes/ClassDeclarations line 6_3; ../EnumDeclarations.sdf3/#java/classes/ClassDeclarations line 7_3; ../Main.sdf3/#java/classes/ClassDeclarations line 6_3; ../MethodDeclarations.sdf3/#java/classes/ClassDeclarations line 7_3; ../../expressions/ClassInstanceCreation.sdf3/#java/classes/ClassDeclarations line 10_3; ../../interfaces/AnnotationTypes.sdf3/#java/classes/ClassDeclarations line 13_3; ../../interfaces/InterfaceDeclarations.sdf3/#java/classes/ClassDeclarations line 9_3; ../../packages/TypeDeclarations.sdf3/#java/classes/ClassDeclarations line 7_3; ../../statements/Blocks.sdf3/#java/classes/ClassDeclarations line 6_3">java/classes/ClassDeclarations</button>

<span class="layout">// 8.1. Class Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_7_3" title="a reference to a single-file definition">java/lexical/Modifiers</a>
  <a href="../../lexical/SemiColon.sdf3/#java/lexical/SemiColon_1_8" id="java/lexical/SemiColon_8_3" title="a reference to a single-file definition">java/lexical/SemiColon</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_9_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_10_3" title="a reference to a single-file definition">java/classes/FieldDeclarations</a>
  <a href="../MethodDeclarations.sdf3/#java/classes/MethodDeclarations_1_8" id="java/classes/MethodDeclarations_11_3" title="a reference to a single-file definition">java/classes/MethodDeclarations</a>
  <a href="../InstanceInitializers.sdf3/#java/classes/InstanceInitializers_1_8" id="java/classes/InstanceInitializers_12_3" title="a reference to a single-file definition">java/classes/InstanceInitializers</a>
  <a href="../StaticInitializers.sdf3/#java/classes/StaticInitializers_1_8" id="java/classes/StaticInitializers_13_3" title="a reference to a single-file definition">java/classes/StaticInitializers</a>
  <a href="../EnumDeclarations.sdf3/#java/classes/EnumDeclarations_1_8" id="java/classes/EnumDeclarations_14_3" title="a reference to a single-file definition">java/classes/EnumDeclarations</a>
  <a href="../ConstructorDeclarations.sdf3/#java/classes/ConstructorDeclarations_1_8" id="java/classes/ConstructorDeclarations_15_3" title="a reference to a single-file definition">java/classes/ConstructorDeclarations</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_16_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>
  <a href="../../interfaces/InterfaceDeclarations.sdf3/#java/interfaces/InterfaceDeclarations_1_8" id="java/interfaces/InterfaceDeclarations_17_3" title="a reference to a single-file definition">java/interfaces/InterfaceDeclarations</a>
  <a href="../../types/TypeVariable.sdf3/#java/types/TypeVariable_1_8" id="java/types/TypeVariable_18_3" title="a reference to a single-file definition">java/types/TypeVariable</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="ClassDeclaration_22_3" title="a definition with multiple references" data-urls="#ClassDeclaration line 65_28; ../../interfaces/AnnotationTypes.sdf3/#ClassDeclaration line 33_37; ../../interfaces/InterfaceDeclarations.sdf3/#ClassDeclaration line 45_32; ../../packages/TypeDeclarations.sdf3/#ClassDeclaration line 16_21; ../../statements/Blocks.sdf3/#ClassDeclaration line 22_22">ClassDeclaration</button>
  <a href="#NormalClassDeclaration_33_22" id="NormalClassDeclaration_23_3" title="a definition with a single reference">NormalClassDeclaration</a>
  <button class="modal-open" id="ClassModifier_24_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button>
  <button class="modal-open" id="TypeParameters_25_3" title="a definition with multiple references" data-urls="#TypeParameters line 37_37; ../ConstructorDeclarations.sdf3/#TypeParameters line 25_33; ../MethodDeclarations.sdf3/#TypeParameters line 37_4; ../../interfaces/InterfaceDeclarations.sdf3/#TypeParameters line 27_45">TypeParameters</button>
  <a href="#SuperClass_37_55" id="SuperClass_26_3" title="a definition with a single reference">SuperClass</a>
  <button class="modal-open" id="SuperInterfaces_27_3" title="a definition with multiple references" data-urls="#SuperInterfaces line 37_69; ../EnumDeclarations.sdf3/#SuperInterfaces line 21_37, 26_37">SuperInterfaces</button>
  <button class="modal-open" id="ClassBodyDeclaration_28_3" title="a definition with multiple references" data-urls="#ClassBodyDeclaration line 38_7; ../EnumDeclarations.sdf3/#ClassBodyDeclaration line 32_7, 38_45; ../../expressions/ClassInstanceCreation.sdf3/#ClassBodyDeclaration line 28_7">ClassBodyDeclaration</button>
  <a href="#ClassMemberDeclaration_58_26" id="ClassMemberDeclaration_29_3" title="a definition with a single reference">ClassMemberDeclaration</a>

<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="ClassDeclaration_33_3" title="a definition with multiple references" data-urls="#ClassDeclaration line 65_28; ../../interfaces/AnnotationTypes.sdf3/#ClassDeclaration line 33_37; ../../interfaces/InterfaceDeclarations.sdf3/#ClassDeclaration line 45_32; ../../packages/TypeDeclarations.sdf3/#ClassDeclaration line 16_21; ../../statements/Blocks.sdf3/#ClassDeclaration line 22_22">ClassDeclaration</button> = <a href="#NormalClassDeclaration_23_3" id="NormalClassDeclaration_33_22" title="a reference to a single-file definition">NormalClassDeclaration</a>
  <button class="modal-open" id="ClassDeclaration_34_3" title="a definition with multiple references" data-urls="#ClassDeclaration line 65_28; ../../interfaces/AnnotationTypes.sdf3/#ClassDeclaration line 33_37; ../../interfaces/InterfaceDeclarations.sdf3/#ClassDeclaration line 45_32; ../../packages/TypeDeclarations.sdf3/#ClassDeclaration line 16_21; ../../statements/Blocks.sdf3/#ClassDeclaration line 22_22">ClassDeclaration</button>  = <a href="../EnumDeclarations.sdf3/#EnumDeclaration_13_3" id="EnumDeclaration_34_23" title="a reference to a single-file definition">EnumDeclaration</a>
  
  <a href="#NormalClassDeclaration_33_22" id="NormalClassDeclaration_36_3" title="a definition with a single reference">NormalClassDeclaration</a>.<span class="cons_Constructor"><span id="ClassDeclaration_36_26" title="a definition with no references">ClassDeclaration</span></span> = &lt;
  &lt;{<a href="#ClassModifier_24_3" id="ClassModifier_37_5" title="a reference to a single-file definition">ClassModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">class</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_37_33" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="#TypeParameters_25_3" id="TypeParameters_37_37" title="a reference to a single-file definition">TypeParameters</a>?&gt; &lt;<a href="#SuperClass_26_3" id="SuperClass_37_55" title="a reference to a single-file definition">SuperClass</a>?&gt; &lt;<a href="#SuperInterfaces_27_3" id="SuperInterfaces_37_69" title="a reference to a single-file definition">SuperInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#ClassBodyDeclaration_28_3" id="ClassBodyDeclaration_38_7" title="a reference to a single-file definition">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <button class="modal-open" id="ClassModifier_41_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_41_19" title="a reference to a single-file definition">Annotation</a>
  <button class="modal-open" id="ClassModifier_42_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_42_19" title="a reference to a single-file definition">Public</a>
  <button class="modal-open" id="ClassModifier_43_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Protected_13_3" id="Protected_43_19" title="a reference to a single-file definition">Protected</a>
  <button class="modal-open" id="ClassModifier_44_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Private_12_3" id="Private_44_19" title="a reference to a single-file definition">Private</a>
  <button class="modal-open" id="ClassModifier_45_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Abstract_8_3" id="Abstract_45_19" title="a reference to a single-file definition">Abstract</a>
  <button class="modal-open" id="ClassModifier_46_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_46_19" title="a reference to a single-file definition">Static</a>
  <button class="modal-open" id="ClassModifier_47_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_47_19" title="a reference to a single-file definition">Final</a>
  <button class="modal-open" id="ClassModifier_48_3" title="a definition with multiple references" data-urls="#ClassModifier line 37_5; ../EnumDeclarations.sdf3/#ClassModifier line 21_5, 26_5">ClassModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Strictfp_16_3" id="Strictfp_48_19" title="a reference to a single-file definition">Strictfp</a>
  
  <button class="modal-open" id="TypeParameters_50_3" title="a definition with multiple references" data-urls="#TypeParameters line 37_37; ../ConstructorDeclarations.sdf3/#TypeParameters line 25_33; ../MethodDeclarations.sdf3/#TypeParameters line 37_4; ../../interfaces/InterfaceDeclarations.sdf3/#TypeParameters line 27_45">TypeParameters</button>.<span class="cons_Constructor"><span id="TypeParameters_50_18" title="a definition with no references">TypeParameters</span></span>               = [<span class="cons_String">&lt;</span>[{<a href="../../types/TypeVariable.sdf3/#TypeParameter_12_3" id="TypeParameter_50_53" title="a reference to a single-file definition">TypeParameter</a> <span class="cons_Lit">","</span>}+]<span class="cons_String">&gt;</span>]

  <span class="layout">// TypeParameter is already defined in 4.4 / java/types/TypeVariable</span>

  <a href="#SuperClass_37_55" id="SuperClass_54_3" title="a definition with a single reference">SuperClass</a>.<span class="cons_Constructor"><span id="SuperClass_54_14" title="a definition with no references">SuperClass</span></span> = &lt;<span class="cons_String">extends</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_54_37" title="a reference to a single-file definition">ClassType</a>&gt;&gt;
  
  <button class="modal-open" id="SuperInterfaces_56_3" title="a definition with multiple references" data-urls="#SuperInterfaces line 37_69; ../EnumDeclarations.sdf3/#SuperInterfaces line 21_37, 26_37">SuperInterfaces</button>.<span class="cons_Constructor"><span id="SuperInterface_56_19" title="a definition with no references">SuperInterface</span></span> = &lt;<span class="cons_String">implements</span> &lt;{<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_56_50" title="a reference to a single-file definition">ClassType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <button class="modal-open" id="ClassBodyDeclaration_58_3" title="a definition with multiple references" data-urls="#ClassBodyDeclaration line 38_7; ../EnumDeclarations.sdf3/#ClassBodyDeclaration line 32_7, 38_45; ../../expressions/ClassInstanceCreation.sdf3/#ClassBodyDeclaration line 28_7">ClassBodyDeclaration</button> = <a href="#ClassMemberDeclaration_29_3" id="ClassMemberDeclaration_58_26" title="a reference to a single-file definition">ClassMemberDeclaration</a>
  <button class="modal-open" id="ClassBodyDeclaration_59_3" title="a definition with multiple references" data-urls="#ClassBodyDeclaration line 38_7; ../EnumDeclarations.sdf3/#ClassBodyDeclaration line 32_7, 38_45; ../../expressions/ClassInstanceCreation.sdf3/#ClassBodyDeclaration line 28_7">ClassBodyDeclaration</button>  = <a href="../InstanceInitializers.sdf3/#InstanceInitializer_10_3" id="InstanceInitializer_59_27" title="a reference to a single-file definition">InstanceInitializer</a>
  <button class="modal-open" id="ClassBodyDeclaration_60_3" title="a definition with multiple references" data-urls="#ClassBodyDeclaration line 38_7; ../EnumDeclarations.sdf3/#ClassBodyDeclaration line 32_7, 38_45; ../../expressions/ClassInstanceCreation.sdf3/#ClassBodyDeclaration line 28_7">ClassBodyDeclaration</button>  = <a href="../StaticInitializers.sdf3/#StaticInitializer_10_3" id="StaticInitializer_60_27" title="a reference to a single-file definition">StaticInitializer</a>
  <button class="modal-open" id="ClassBodyDeclaration_61_3" title="a definition with multiple references" data-urls="#ClassBodyDeclaration line 38_7; ../EnumDeclarations.sdf3/#ClassBodyDeclaration line 32_7, 38_45; ../../expressions/ClassInstanceCreation.sdf3/#ClassBodyDeclaration line 28_7">ClassBodyDeclaration</button>  = <a href="../ConstructorDeclarations.sdf3/#ConstructorDeclaration_18_3" id="ConstructorDeclaration_61_27" title="a reference to a single-file definition">ConstructorDeclaration</a>
  
  <a href="#ClassMemberDeclaration_58_26" id="ClassMemberDeclaration_63_3" title="a definition with a single reference">ClassMemberDeclaration</a> = <a href="../FieldDeclarations.sdf3/#FieldDeclaration_17_3" id="FieldDeclaration_63_28" title="a reference to a single-file definition">FieldDeclaration</a>
  <a href="#ClassMemberDeclaration_58_26" id="ClassMemberDeclaration_64_3" title="a definition with a single reference">ClassMemberDeclaration</a> = <a href="../MethodDeclarations.sdf3/#MethodDeclaration_15_3" id="MethodDeclaration_64_28" title="a reference to a single-file definition">MethodDeclaration</a>
  <a href="#ClassMemberDeclaration_58_26" id="ClassMemberDeclaration_65_3" title="a definition with a single reference">ClassMemberDeclaration</a> = <a href="#ClassDeclaration_22_3" id="ClassDeclaration_65_28" title="a reference to a single-file definition">ClassDeclaration</a>
  <a href="#ClassMemberDeclaration_58_26" id="ClassMemberDeclaration_66_3" title="a definition with a single reference">ClassMemberDeclaration</a> = <a href="../../interfaces/InterfaceDeclarations.sdf3/#InterfaceDeclaration_18_3" id="InterfaceDeclaration_66_28" title="a reference to a single-file definition">InterfaceDeclaration</a>
  <a href="#ClassMemberDeclaration_58_26" id="ClassMemberDeclaration_67_3" title="a definition with a single reference">ClassMemberDeclaration</a> = <a href="../../lexical/SemiColon.sdf3/#SemiColon_8_3" id="SemiColon_67_28" title="a reference to a single-file definition">SemiColon</a>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
