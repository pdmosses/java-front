---
title: ConstantDeclarations.sdf3
hide:
  - toc
---

# `ConstantDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/interfaces/ConstantDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/interfaces/ConstantDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/interfaces/ConstantDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/interfaces/ConstantDeclarations_215_251" id="java/interfaces/ConstantDeclarations_7_43" title="Referenced at ../Main.sdf3 line 10">java/interfaces/ConstantDeclarations</a>

<span class="layout">// 9.3. Field (Constant) Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Modifiers.sdf3#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_94_116" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../classes/FieldDeclarations.sdf3#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_119_149" title="Defined at ../../classes/FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_152_179" title="Defined at ../Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../AnnotationTypes.sdf3#ConstantDeclaration_789_808" id="ConstantDeclaration_203_222" title="Referenced at ../AnnotationTypes.sdf3 line 32; ../InterfaceDeclarations.sdf3 line 43">ConstantDeclaration</a>
  <a href="#ConstantModifier_309_325" id="ConstantModifier_225_241" title="Referenced at line 18">ConstantModifier</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../AnnotationTypes.sdf3#ConstantDeclaration_789_808" id="ConstantDeclaration_268_287" title="Referenced at ../AnnotationTypes.sdf3 line 32; ../InterfaceDeclarations.sdf3 line 43">ConstantDeclaration</a>.<span class="cons_Constructor"><span id="ConstantDecl_288_300" title="Not referenced locally, nor via imports">ConstantDecl</span></span> = &lt;
  &lt;{<a href="#ConstantModifier_225_241" id="ConstantModifier_309_325" title="Defined at line 13, 20, 21, 22, 23">ConstantModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#UnannType_403_412" id="UnannType_334_343" title="Defined at ../../classes/FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="../../classes/FieldDeclarations.sdf3#VarDecl_355_362" id="VarDecl_347_354" title="Defined at ../../classes/FieldDeclarations.sdf3 line 19, 33, 34">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#ConstantModifier_309_325" id="ConstantModifier_369_385" title="Referenced at line 18">ConstantModifier</a> = <a href="../Annotations.sdf3#Annotation_158_168" id="Annotation_388_398" title="Defined at ../Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#ConstantModifier_309_325" id="ConstantModifier_401_417" title="Referenced at line 18">ConstantModifier</a> = <a href="../../lexical/Modifiers.sdf3#Public_201_207" id="Public_420_426" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#ConstantModifier_309_325" id="ConstantModifier_429_445" title="Referenced at line 18">ConstantModifier</a> = <a href="../../lexical/Modifiers.sdf3#Static_210_216" id="Static_448_454" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#ConstantModifier_309_325" id="ConstantModifier_457_473" title="Referenced at line 18">ConstantModifier</a> = <a href="../../lexical/Modifiers.sdf3#Final_162_167" id="Final_476_481" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
</code></pre></td></tr></tbody></table></div>