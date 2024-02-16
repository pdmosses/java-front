---
title: PrimaryExpressions.sdf3
hide:
  - toc
---

# `PrimaryExpressions.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/PrimaryExpressions.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/PrimaryExpressions.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/PrimaryExpressions.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/expressions/PrimaryExpressions_7_3" id="java/expressions/PrimaryExpressions_1_8" title="a definition with a single reference">java/expressions/PrimaryExpressions</a>

<span class="layout">// 15.8. Primary Expressions</span>

<span class="keyword">imports</span>
  <a href="../../literals/Main.sdf3/#java/literals/Main_1_8" id="java/literals/Main_6_3" title="a reference to a single-file definition">java/literals/Main</a>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_7_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../types/PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_8_3" title="a reference to a single-file definition">java/types/PrimitiveTypes</a>
  
<span class="keyword">context-free sorts</span>

  <a href="#ClassLiteral_18_16" id="ClassLiteral_12_3" title="a definition with a single reference">ClassLiteral</a>
  <button class="modal-open" id="Dims_13_3" title="a definition with multiple references" data-urls="#Dims line 23_54, 24_57, 25_51">Dims</button>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_21_19" id="Expression_17_3" title="a definition with a single reference">Expression</a> = <a href="../../literals/Main.sdf3/#Literal_15_3" id="Literal_17_16" title="a reference to a single-file definition">Literal</a>
  <a href="#Expression_21_19" id="Expression_18_3" title="a definition with a single reference">Expression</a> = <a href="#ClassLiteral_12_3" id="ClassLiteral_18_16" title="a reference to a single-file definition">ClassLiteral</a>
  <a href="#Expression_21_19" id="Expression_19_3" title="a definition with a single reference">Expression</a>.<span class="cons_Constructor"><span id="This_19_14" title="a definition with no references">This</span></span> = <span class="cons_Lit">"this"</span>
  <a href="#Expression_21_19" id="Expression_20_3" title="a definition with a single reference">Expression</a>.<span class="cons_Constructor"><span id="QThis_20_14" title="a definition with no references">QThis</span></span> = &lt;&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_20_24" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">.this</span>&gt;
  <a href="#Expression_21_19" id="Expression_21_3" title="a definition with a single reference">Expression</a> = &lt;<span class="cons_String">(</span>&lt;<a href="#Expression_17_3" id="Expression_21_19" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span>&gt; {<span class="keyword">bracket</span>}
  
  <a href="#ClassLiteral_18_16" id="ClassLiteral_23_3" title="a definition with a single reference">ClassLiteral</a>.<span class="cons_Constructor"><span id="TypeNameClassLiteral_23_16" title="a definition with no references">TypeNameClassLiteral</span></span>    = &lt;&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_23_44" title="a reference to a single-file definition">TypeName</a>&gt;&lt;<a href="#Dims_13_3" id="Dims_23_54" title="a reference to a single-file definition">Dims</a>*&gt;<span class="cons_String">.class</span>&gt;
  <a href="#ClassLiteral_18_16" id="ClassLiteral_24_3" title="a definition with a single reference">ClassLiteral</a>.<span class="cons_Constructor"><span id="NumericTypeClassLiteral_24_16" title="a definition with no references">NumericTypeClassLiteral</span></span> = &lt;&lt;<a href="../../types/PrimitiveTypes.sdf3/#NumericType_11_3" id="NumericType_24_44" title="a reference to a single-file definition">NumericType</a>&gt;&lt;<a href="#Dims_13_3" id="Dims_24_57" title="a reference to a single-file definition">Dims</a>*&gt;<span class="cons_String">.class</span>&gt;
  <a href="#ClassLiteral_18_16" id="ClassLiteral_25_3" title="a definition with a single reference">ClassLiteral</a>.<span class="cons_Constructor"><span id="BooleanClassLiteral_25_16" title="a definition with no references">BooleanClassLiteral</span></span>     = &lt;<span class="cons_String">boolean</span>&lt;<a href="#Dims_13_3" id="Dims_25_51" title="a reference to a single-file definition">Dims</a>*&gt;<span class="cons_String">.class</span>&gt;
  <a href="#ClassLiteral_18_16" id="ClassLiteral_26_3" title="a definition with a single reference">ClassLiteral</a>.<span class="cons_Constructor"><span id="VoidClassLiteral_26_16" title="a definition with no references">VoidClassLiteral</span></span>        = &lt;<span class="cons_String">void.class</span>&gt;
  
  <button class="modal-open" id="Dims_28_3" title="a definition with multiple references" data-urls="#Dims line 23_54, 24_57, 25_51">Dims</button>.<span class="cons_Constructor"><span id="Dimension_28_8" title="a definition with no references">Dimension</span></span> = &lt;<span class="cons_String">[]</span>&gt;

<span class="keyword">template options</span>

  <span class="keyword">tokenize</span> : ".["
  
  

  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
