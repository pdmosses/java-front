---
title: InterfaceMethodDeclarations.sdf3
hide:
  - toc
---

# `InterfaceMethodDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/interfaces/InterfaceMethodDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/interfaces/InterfaceMethodDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/interfaces/InterfaceMethodDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../InterfaceDeclarations.sdf3/#java/interfaces/InterfaceMethodDeclarations_295_338" id="java/interfaces/InterfaceMethodDeclarations_7_50" title="Referenced at ../InterfaceDeclarations.sdf3 line 13; ../Main.sdf3 line 7">java/interfaces/InterfaceMethodDeclarations</a>

<span class="layout">// 9.4. Method Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_91_113" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_7_38" id="java/classes/MethodDeclarations_116_147" title="Defined at ../../classes/MethodDeclarations.sdf3 line 1">java/classes/MethodDeclarations</a>
  <a href="../Annotations.sdf3/#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_150_177" title="Defined at ../Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../InterfaceDeclarations.sdf3/#InterfaceMethodDeclaration_1114_1140" id="InterfaceMethodDeclaration_201_227" title="Referenced at ../InterfaceDeclarations.sdf3 line 44">InterfaceMethodDeclaration</a>
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_230_253" title="Referenced at line 18">InterfaceMethodModifier</a> 

<span class="keyword">context-free syntax</span>
  
  <a href="../InterfaceDeclarations.sdf3/#InterfaceMethodDeclaration_1114_1140" id="InterfaceMethodDeclaration_281_307" title="Referenced at ../InterfaceDeclarations.sdf3 line 44">InterfaceMethodDeclaration</a>.<span class="cons_Constructor"><span id="AbstractMethodDec_308_325" title="Not referenced locally, nor via imports">AbstractMethodDec</span></span> = &lt;
  &lt;{<a href="#InterfaceMethodModifier_230_253" id="InterfaceMethodModifier_334_357" title="Defined at line 13, 20, 21, 22, 23, 24, 25">InterfaceMethodModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/MethodDeclarations.sdf3/#MethodHeader_320_332" id="MethodHeader_366_378" title="Defined at ../../classes/MethodDeclarations.sdf3 line 16, 33, 36">MethodHeader</a>&gt; &lt;<a href="../../classes/MethodDeclarations.sdf3/#MethodBody_386_396" id="MethodBody_381_391" title="Defined at ../../classes/MethodDeclarations.sdf3 line 21, 56, 57">MethodBody</a>&gt;&gt;
  
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_399_422" title="Referenced at line 18">InterfaceMethodModifier</a> = <a href="../Annotations.sdf3/#Annotation_158_168" id="Annotation_425_435" title="Defined at ../Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_438_461" title="Referenced at line 18">InterfaceMethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_201_207" id="Public_464_470" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_473_496" title="Referenced at line 18">InterfaceMethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Abstract_141_149" id="Abstract_499_507" title="Defined at ../../lexical/Modifiers.sdf3 line 8, 23">Abstract</a>
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_510_533" title="Referenced at line 18">InterfaceMethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Default_152_159" id="Default_536_543" title="Defined at ../../lexical/Modifiers.sdf3 line 9, 24">Default</a>
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_546_569" title="Referenced at line 18">InterfaceMethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_210_216" id="Static_572_578" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#InterfaceMethodModifier_334_357" id="InterfaceMethodModifier_581_604" title="Referenced at line 18">InterfaceMethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Strictfp_219_227" id="Strictfp_607_615" title="Defined at ../../lexical/Modifiers.sdf3 line 16, 31">Strictfp</a>
</code></pre></td></tr></tbody></table></div>