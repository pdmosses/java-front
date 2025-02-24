---
title: InterfaceDeclarations.sdf3
hide:
  - toc
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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/interfaces/InterfaceDeclarations_1_8" title="a definition with multiple references" data-urls="../AnnotationTypes.sdf3/#java/interfaces/InterfaceDeclarations line 6_3; ../Main.sdf3/#java/interfaces/InterfaceDeclarations line 6_3; ../../classes/ClassDeclarations.sdf3/#java/interfaces/InterfaceDeclarations line 17_3; ../../packages/TypeDeclarations.sdf3/#java/interfaces/InterfaceDeclarations line 8_3">java/interfaces/InterfaceDeclarations</button>

<span class="layout">// 9.1. Interface Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_7_3" title="a reference to a single-file definition">java/lexical/Modifiers</a>
  <a href="../../lexical/SemiColon.sdf3/#java/lexical/SemiColon_1_8" id="java/lexical/SemiColon_8_3" title="a reference to a single-file definition">java/lexical/SemiColon</a>
  <a href="../../classes/ClassDeclarations.sdf3/#java/classes/ClassDeclarations_1_8" id="java/classes/ClassDeclarations_9_3" title="a reference to a single-file definition">java/classes/ClassDeclarations</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_10_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_11_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>
  <a href="../ConstantDeclarations.sdf3/#java/interfaces/ConstantDeclarations_1_8" id="java/interfaces/ConstantDeclarations_12_3" title="a reference to a single-file definition">java/interfaces/ConstantDeclarations</a>
  <a href="../InterfaceMethodDeclarations.sdf3/#java/interfaces/InterfaceMethodDeclarations_1_8" id="java/interfaces/InterfaceMethodDeclarations_13_3" title="a reference to a single-file definition">java/interfaces/InterfaceMethodDeclarations</a>
  <a href="../AnnotationTypes.sdf3/#java/interfaces/AnnotationTypes_1_8" id="java/interfaces/AnnotationTypes_14_3" title="a reference to a single-file definition">java/interfaces/AnnotationTypes</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="InterfaceDeclaration_18_3" title="a definition with multiple references" data-urls="#InterfaceDeclaration line 46_32; ../AnnotationTypes.sdf3/#InterfaceDeclaration line 34_37; ../../classes/ClassDeclarations.sdf3/#InterfaceDeclaration line 66_28; ../../packages/TypeDeclarations.sdf3/#InterfaceDeclaration line 17_21">InterfaceDeclaration</button>
  <button class="modal-open" id="InterfaceModifier_19_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button>
  <a href="#ExtendsInterfaces_27_63" id="ExtendsInterfaces_20_3" title="a definition with a single reference">ExtendsInterfaces</a>
  <a href="#InterfaceMemberDeclaration_28_7" id="InterfaceMemberDeclaration_21_3" title="a definition with a single reference">InterfaceMemberDeclaration</a>

<span class="keyword">context-free syntax</span>

  
  <button class="modal-open" id="InterfaceDeclaration_26_3" title="a definition with multiple references" data-urls="#InterfaceDeclaration line 46_32; ../AnnotationTypes.sdf3/#InterfaceDeclaration line 34_37; ../../classes/ClassDeclarations.sdf3/#InterfaceDeclaration line 66_28; ../../packages/TypeDeclarations.sdf3/#InterfaceDeclaration line 17_21">InterfaceDeclaration</button>.<span class="cons_Constructor"><span id="NormalInterface_26_24" title="a definition with no references">NormalInterface</span></span> = &lt;
  &lt;{<a href="#InterfaceModifier_19_3" id="InterfaceModifier_27_5" title="a reference to a single-file definition">InterfaceModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">interface</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_41" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="../../classes/ClassDeclarations.sdf3/#TypeParameters_25_3" id="TypeParameters_27_45" title="a reference to a single-file definition">TypeParameters</a>?&gt; &lt;<a href="#ExtendsInterfaces_20_3" id="ExtendsInterfaces_27_63" title="a reference to a single-file definition">ExtendsInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#InterfaceMemberDeclaration_21_3" id="InterfaceMemberDeclaration_28_7" title="a reference to a single-file definition">InterfaceMemberDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <button class="modal-open" id="InterfaceDeclaration_31_3" title="a definition with multiple references" data-urls="#InterfaceDeclaration line 46_32; ../AnnotationTypes.sdf3/#InterfaceDeclaration line 34_37; ../../classes/ClassDeclarations.sdf3/#InterfaceDeclaration line 66_28; ../../packages/TypeDeclarations.sdf3/#InterfaceDeclaration line 17_21">InterfaceDeclaration</button> = <a href="../AnnotationTypes.sdf3/#AnnotationTypeDeclaration_18_3" id="AnnotationTypeDeclaration_31_26" title="a reference to a single-file definition">AnnotationTypeDeclaration</a>
  
  <button class="modal-open" id="InterfaceModifier_33_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../Annotations.sdf3/#Annotation_12_3" id="Annotation_33_23" title="a reference to a single-file definition">Annotation</a>
  <button class="modal-open" id="InterfaceModifier_34_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_34_23" title="a reference to a single-file definition">Public</a>
  <button class="modal-open" id="InterfaceModifier_35_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Protected_13_3" id="Protected_35_23" title="a reference to a single-file definition">Protected</a>
  <button class="modal-open" id="InterfaceModifier_36_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Private_12_3" id="Private_36_23" title="a reference to a single-file definition">Private</a>
  <button class="modal-open" id="InterfaceModifier_37_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Abstract_8_3" id="Abstract_37_23" title="a reference to a single-file definition">Abstract</a>
  <button class="modal-open" id="InterfaceModifier_38_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_38_23" title="a reference to a single-file definition">Static</a>
  <button class="modal-open" id="InterfaceModifier_39_3" title="a definition with multiple references" data-urls="#InterfaceModifier line 27_5; ../AnnotationTypes.sdf3/#InterfaceModifier line 27_5">InterfaceModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Strictfp_16_3" id="Strictfp_39_23" title="a reference to a single-file definition">Strictfp</a>
  
  <a href="#ExtendsInterfaces_27_63" id="ExtendsInterfaces_41_3" title="a definition with a single reference">ExtendsInterfaces</a>.<span class="cons_Constructor"><span id="ExtendsInterfaces_41_21" title="a definition with no references">ExtendsInterfaces</span></span> = &lt;<span class="cons_String">extends</span> &lt;{<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_41_52" title="a reference to a single-file definition">ClassType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#InterfaceMemberDeclaration_28_7" id="InterfaceMemberDeclaration_43_3" title="a definition with a single reference">InterfaceMemberDeclaration</a> = <a href="../ConstantDeclarations.sdf3/#ConstantDeclaration_12_3" id="ConstantDeclaration_43_32" title="a reference to a single-file definition">ConstantDeclaration</a>
  <a href="#InterfaceMemberDeclaration_28_7" id="InterfaceMemberDeclaration_44_3" title="a definition with a single reference">InterfaceMemberDeclaration</a> = <a href="../InterfaceMethodDeclarations.sdf3/#InterfaceMethodDeclaration_12_3" id="InterfaceMethodDeclaration_44_32" title="a reference to a single-file definition">InterfaceMethodDeclaration</a>
  <a href="#InterfaceMemberDeclaration_28_7" id="InterfaceMemberDeclaration_45_3" title="a definition with a single reference">InterfaceMemberDeclaration</a> = <a href="../../classes/ClassDeclarations.sdf3/#ClassDeclaration_22_3" id="ClassDeclaration_45_32" title="a reference to a single-file definition">ClassDeclaration</a>
  <a href="#InterfaceMemberDeclaration_28_7" id="InterfaceMemberDeclaration_46_3" title="a definition with a single reference">InterfaceMemberDeclaration</a> = <a href="#InterfaceDeclaration_18_3" id="InterfaceDeclaration_46_32" title="a reference to a single-file definition">InterfaceDeclaration</a>
  <a href="#InterfaceMemberDeclaration_28_7" id="InterfaceMemberDeclaration_47_3" title="a definition with a single reference">InterfaceMemberDeclaration</a> = <a href="../../lexical/SemiColon.sdf3/#SemiColon_8_3" id="SemiColon_47_32" title="a reference to a single-file definition">SemiColon</a>
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
