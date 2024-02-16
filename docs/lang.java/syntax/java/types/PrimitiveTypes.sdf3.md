---
title: PrimitiveTypes.sdf3
hide:
  - toc
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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/types/PrimitiveTypes_1_8" title="a definition with multiple references" data-urls="../Main.sdf3/#java/types/PrimitiveTypes line 6_3; ../ReferenceTypes.sdf3/#java/types/PrimitiveTypes line 7_3; ../../classes/FieldDeclarations.sdf3/#java/types/PrimitiveTypes line 9_3; ../../expressions/ArrayCreation.sdf3/#java/types/PrimitiveTypes line 7_3; ../../expressions/PrimaryExpressions.sdf3/#java/types/PrimitiveTypes line 8_3; ../../expressions/UnaryOperators.sdf3/#java/types/PrimitiveTypes line 6_3">java/types/PrimitiveTypes</button>

<span class="layout">// 4.2. Primitive Types and Values</span>

<span class="keyword">imports</span>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_6_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="PrimitiveType_10_3" title="a definition with multiple references" data-urls="../Main.sdf3/#PrimitiveType line 19_10; ../ReferenceTypes.sdf3/#PrimitiveType line 37_36; ../../expressions/ArrayCreation.sdf3/#PrimitiveType line 24_19; ../../expressions/UnaryOperators.sdf3/#PrimitiveType line 22_33">PrimitiveType</button>
  <button class="modal-open" id="NumericType_11_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>

<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="PrimitiveType_15_3" title="a definition with multiple references" data-urls="../Main.sdf3/#PrimitiveType line 19_10; ../ReferenceTypes.sdf3/#PrimitiveType line 37_36; ../../expressions/ArrayCreation.sdf3/#PrimitiveType line 24_19; ../../expressions/UnaryOperators.sdf3/#PrimitiveType line 22_33">PrimitiveType</button>.<span class="cons_Constructor"><span id="NumericType_15_17" title="a definition with no references">NumericType</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_15_34" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#NumericType_11_3" id="NumericType_15_53" title="a reference to a single-file definition">NumericType</a>&gt;&gt;
  <button class="modal-open" id="PrimitiveType_16_3" title="a definition with multiple references" data-urls="../Main.sdf3/#PrimitiveType line 19_10; ../ReferenceTypes.sdf3/#PrimitiveType line 37_36; ../../expressions/ArrayCreation.sdf3/#PrimitiveType line 24_19; ../../expressions/UnaryOperators.sdf3/#PrimitiveType line 22_33">PrimitiveType</button>.<span class="cons_Constructor"><span id="BooleanType_16_17" title="a definition with no references">BooleanType</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_16_34" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">boolean</span>&gt;
  <button class="modal-open" id="NumericType_17_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Byte_17_15" title="a definition with no references">Byte</span></span>   = &lt;<span class="cons_String">byte</span>&gt;
  <button class="modal-open" id="NumericType_18_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Short_18_15" title="a definition with no references">Short</span></span>  = &lt;<span class="cons_String">short</span>&gt;
  <button class="modal-open" id="NumericType_19_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Int_19_15" title="a definition with no references">Int</span></span>    = &lt;<span class="cons_String">int</span>&gt;
  <button class="modal-open" id="NumericType_20_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Long_20_15" title="a definition with no references">Long</span></span>   = &lt;<span class="cons_String">long</span>&gt;
  <button class="modal-open" id="NumericType_21_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Char_21_15" title="a definition with no references">Char</span></span>   = &lt;<span class="cons_String">char</span>&gt;
  <button class="modal-open" id="NumericType_22_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Float_22_15" title="a definition with no references">Float</span></span>  = &lt;<span class="cons_String">float</span>&gt;
  <button class="modal-open" id="NumericType_23_3" title="a definition with multiple references" data-urls="#NumericType line 15_53; ../../classes/FieldDeclarations.sdf3/#NumericType line 53_36; ../../expressions/PrimaryExpressions.sdf3/#NumericType line 24_44">NumericType</button>.<span class="cons_Constructor"><span id="Double_23_15" title="a definition with no references">Double</span></span> = &lt;<span class="cons_String">double</span>&gt;
  
  
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
