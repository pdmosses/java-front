---
title: PrimitiveTypes.sdf3
---

# `PrimitiveTypes.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/types/PrimitiveTypes.sdf3]

[pdmosses/java-front/lang.java/syntax/java/types/PrimitiveTypes.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/types/PrimitiveTypes.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../ReferenceTypes.sdf3#java/types/PrimitiveTypes_107_132" id="java/types/PrimitiveTypes_7_32" title="Referenced at ../ReferenceTypes.sdf3 line 7">java/types/PrimitiveTypes</a>

<span class="layout">// 4.2. Primitive Types and Values</span>

<span class="keyword">imports</span>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_80_107" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../../expressions/ArrayCreation.sdf3#PrimitiveType_581_594" id="PrimitiveType_131_144" title="Referenced at ../../expressions/ArrayCreation.sdf3 line 24; ../../expressions/UnaryOperators.sdf3 line 22; ../Main.sdf3 line 19; ../ReferenceTypes.sdf3 line 37">PrimitiveType</a>
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_147_158" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../../expressions/ArrayCreation.sdf3#PrimitiveType_581_594" id="PrimitiveType_185_198" title="Referenced at ../../expressions/ArrayCreation.sdf3 line 24; ../../expressions/UnaryOperators.sdf3 line 22; ../Main.sdf3 line 19; ../ReferenceTypes.sdf3 line 37">PrimitiveType</a>.<span class="cons_Constructor"><span id="NumericType_199_210" title="Not referenced locally, nor via imports">NumericType</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_216_226" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#NumericType_147_158" id="NumericType_235_246" title="Defined at line 11, 17, 18, 19, 20, 21, 22, 23">NumericType</a>&gt;&gt;
  <a href="../../expressions/ArrayCreation.sdf3#PrimitiveType_581_594" id="PrimitiveType_251_264" title="Referenced at ../../expressions/ArrayCreation.sdf3 line 24; ../../expressions/UnaryOperators.sdf3 line 22; ../Main.sdf3 line 19; ../ReferenceTypes.sdf3 line 37">PrimitiveType</a>.<span class="cons_Constructor"><span id="BooleanType_265_276" title="Not referenced locally, nor via imports">BooleanType</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_282_292" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">boolean</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_311_322" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Byte_323_327" title="Not referenced locally, nor via imports">Byte</span></span>   = &lt;<span class="cons_String">byte</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_341_352" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Short_353_358" title="Not referenced locally, nor via imports">Short</span></span>  = &lt;<span class="cons_String">short</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_372_383" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Int_384_387" title="Not referenced locally, nor via imports">Int</span></span>    = &lt;<span class="cons_String">int</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_401_412" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Long_413_417" title="Not referenced locally, nor via imports">Long</span></span>   = &lt;<span class="cons_String">long</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_431_442" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Char_443_447" title="Not referenced locally, nor via imports">Char</span></span>   = &lt;<span class="cons_String">char</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_461_472" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Float_473_478" title="Not referenced locally, nor via imports">Float</span></span>  = &lt;<span class="cons_String">float</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#NumericType_1227_1238" id="NumericType_492_503" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 53; ../../expressions/PrimaryExpressions.sdf3 line 24; line 15">NumericType</a>.<span class="cons_Constructor"><span id="Double_504_510" title="Not referenced locally, nor via imports">Double</span></span> = &lt;<span class="cons_String">double</span>&gt;
  
  
  
  
</code></pre></td></tr></tbody></table></div>