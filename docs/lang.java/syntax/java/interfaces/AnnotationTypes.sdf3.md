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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/interfaces/AnnotationTypes_1_8" title="a definition with multiple references" data-urls="../InterfaceDeclarations.sdf3/#java/interfaces/AnnotationTypes line 14_3; ../Main.sdf3/#java/interfaces/AnnotationTypes line 8_3">java/interfaces/AnnotationTypes</button>

<span class="layout">// 9.6. Annotation Types</span>

<span class="keyword">imports</span>
  <a href="../InterfaceDeclarations.sdf3/#java/interfaces/InterfaceDeclarations_1_8" id="java/interfaces/InterfaceDeclarations_6_3" title="a reference to a single-file definition">java/interfaces/InterfaceDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_8_3" title="a reference to a single-file definition">java/lexical/Modifiers</a>
  <a href="../../lexical/SemiColon.sdf3/#java/lexical/SemiColon_1_8" id="java/lexical/SemiColon_9_3" title="a reference to a single-file definition">java/lexical/SemiColon</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_10_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../../classes/FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_11_3" title="a reference to a single-file definition">java/classes/FieldDeclarations</a>
  <a href="../ConstantDeclarations.sdf3/#java/interfaces/ConstantDeclarations_1_8" id="java/interfaces/ConstantDeclarations_12_3" title="a reference to a single-file definition">java/interfaces/ConstantDeclarations</a>
  <a href="../../classes/ClassDeclarations.sdf3/#java/classes/ClassDeclarations_1_8" id="java/classes/ClassDeclarations_13_3" title="a reference to a single-file definition">java/classes/ClassDeclarations</a>
  <a href="../Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_14_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../InterfaceDeclarations.sdf3/#AnnotationTypeDeclaration_31_26" id="AnnotationTypeDeclaration_18_3" title="a definition with a single reference">AnnotationTypeDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_28_7" id="AnnotationTypeMemberDeclaration_19_3" title="a definition with a single reference">AnnotationTypeMemberDeclaration</a>
  <a href="#AnnotationTypeElementDeclaration_31_37" id="AnnotationTypeElementDeclaration_20_3" title="a definition with a single reference">AnnotationTypeElementDeclaration</a>
  <a href="#AnnotationTypeElementModifier_38_5" id="AnnotationTypeElementModifier_21_3" title="a definition with a single reference">AnnotationTypeElementModifier</a>
  <a href="#DefaultValue_38_83" id="DefaultValue_22_3" title="a definition with a single reference">DefaultValue</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../InterfaceDeclarations.sdf3/#AnnotationTypeDeclaration_31_26" id="AnnotationTypeDeclaration_26_3" title="a definition with a single reference">AnnotationTypeDeclaration</a>.<span class="cons_Constructor"><span id="AnnoDec_26_29" title="a definition with no references">AnnoDec</span></span> = &lt;
  &lt;{<a href="../InterfaceDeclarations.sdf3/#InterfaceModifier_19_3" id="InterfaceModifier_27_5" title="a reference to a single-file definition">InterfaceModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">@interface</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_42" title="a reference to a single-file definition">Id</a>&gt; <span class="cons_String">{</span>
    &lt;{<a href="#AnnotationTypeMemberDeclaration_19_3" id="AnnotationTypeMemberDeclaration_28_7" title="a reference to a single-file definition">AnnotationTypeMemberDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#AnnotationTypeMemberDeclaration_28_7" id="AnnotationTypeMemberDeclaration_31_3" title="a definition with a single reference">AnnotationTypeMemberDeclaration</a> = <a href="#AnnotationTypeElementDeclaration_20_3" id="AnnotationTypeElementDeclaration_31_37" title="a reference to a single-file definition">AnnotationTypeElementDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_28_7" id="AnnotationTypeMemberDeclaration_32_3" title="a definition with a single reference">AnnotationTypeMemberDeclaration</a> = <a href="../ConstantDeclarations.sdf3/#ConstantDeclaration_12_3" id="ConstantDeclaration_32_37" title="a reference to a single-file definition">ConstantDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_28_7" id="AnnotationTypeMemberDeclaration_33_3" title="a definition with a single reference">AnnotationTypeMemberDeclaration</a> = <a href="../../classes/ClassDeclarations.sdf3/#ClassDeclaration_22_3" id="ClassDeclaration_33_37" title="a reference to a single-file definition">ClassDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_28_7" id="AnnotationTypeMemberDeclaration_34_3" title="a definition with a single reference">AnnotationTypeMemberDeclaration</a> = <a href="../InterfaceDeclarations.sdf3/#InterfaceDeclaration_18_3" id="InterfaceDeclaration_34_37" title="a reference to a single-file definition">InterfaceDeclaration</a>
  <a href="#AnnotationTypeMemberDeclaration_28_7" id="AnnotationTypeMemberDeclaration_35_3" title="a definition with a single reference">AnnotationTypeMemberDeclaration</a> = <a href="../../lexical/SemiColon.sdf3/#SemiColon_8_3" id="SemiColon_35_37" title="a reference to a single-file definition">SemiColon</a>
  
  <a href="#AnnotationTypeElementDeclaration_31_37" id="AnnotationTypeElementDeclaration_37_3" title="a definition with a single reference">AnnotationTypeElementDeclaration</a>.<span class="cons_Constructor"><span id="AnnotationTypeElementDecl_37_36" title="a definition with no references">AnnotationTypeElementDecl</span></span> = &lt;
  &lt;{<a href="#AnnotationTypeElementModifier_21_3" id="AnnotationTypeElementModifier_38_5" title="a reference to a single-file definition">AnnotationTypeElementModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_38_43" title="a reference to a single-file definition">UnannType</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_38_55" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">()</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDimsEmpty_18_3" id="AnnotatedDimsEmpty_38_62" title="a reference to a single-file definition">AnnotatedDimsEmpty</a>&gt; &lt;<a href="#DefaultValue_22_3" id="DefaultValue_38_83" title="a reference to a single-file definition">DefaultValue</a>?&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#AnnotationTypeElementModifier_38_5" id="AnnotationTypeElementModifier_40_3" title="a definition with a single reference">AnnotationTypeElementModifier</a> = <a href="../Annotations.sdf3/#Annotation_12_3" id="Annotation_40_35" title="a reference to a single-file definition">Annotation</a>
  <a href="#AnnotationTypeElementModifier_38_5" id="AnnotationTypeElementModifier_41_3" title="a definition with a single reference">AnnotationTypeElementModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_41_35" title="a reference to a single-file definition">Public</a>
  <a href="#AnnotationTypeElementModifier_38_5" id="AnnotationTypeElementModifier_42_3" title="a definition with a single reference">AnnotationTypeElementModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Abstract_8_3" id="Abstract_42_35" title="a reference to a single-file definition">Abstract</a>
  
  <a href="#DefaultValue_38_83" id="DefaultValue_44_3" title="a definition with a single reference">DefaultValue</a>.<span class="cons_Constructor"><span id="DefaultVal_44_16" title="a definition with no references">DefaultVal</span></span> = &lt;<span class="cons_String">default</span> &lt;<a href="../Annotations.sdf3/#ElementValue_14_3" id="ElementValue_44_39" title="a reference to a single-file definition">ElementValue</a>&gt;&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
