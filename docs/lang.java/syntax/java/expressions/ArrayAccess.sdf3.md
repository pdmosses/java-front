---
title: ArrayAccess.sdf3
hide:
  - toc
---

# `ArrayAccess.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/ArrayAccess.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/ArrayAccess.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/ArrayAccess.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/ArrayAccess_1_8" title="a definition with multiple references" data-urls="../AssignmentOperators.sdf3/#java/expressions/ArrayAccess line 6_3; ../Disambiguation.sdf3/#java/expressions/ArrayAccess line 8_3; ../Main.sdf3/#java/expressions/ArrayAccess line 11_3">java/expressions/ArrayAccess</button>

<span class="layout">// 15.10.3. Array Access Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../ArrayCreation.sdf3/#java/expressions/ArrayCreation_1_8" id="java/expressions/ArrayCreation_7_3" title="a reference to a single-file definition">java/expressions/ArrayCreation</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="ArrayAccess_11_3" title="a definition with multiple references" data-urls="#ArrayAccess line 15_16, 21_3; ../AssignmentOperators.sdf3/#ArrayAccess line 31_9; ../Disambiguation.sdf3/#ArrayAccess line 56_5">ArrayAccess</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Expression_15_3" title="a definition with multiple references" data-urls="#Expression line 17_31, 17_44">Expression</button> = <a href="#ArrayAccess_11_3" id="ArrayAccess_15_16" title="a reference to a single-file definition">ArrayAccess</a>
  
  <button class="modal-open" id="ArrayAccess_17_3" title="a definition with multiple references" data-urls="#ArrayAccess line 15_16, 21_3; ../AssignmentOperators.sdf3/#ArrayAccess line 31_9; ../Disambiguation.sdf3/#ArrayAccess line 56_5">ArrayAccess</button>.<span class="cons_Constructor"><button class="modal-open" id="ArrayAccess_17_15" title="a definition with multiple references" data-urls="#ArrayAccess line 21_15; ../Disambiguation.sdf3/#ArrayAccess line 56_17">ArrayAccess</button></span> = &lt;&lt;<a href="#Expression_15_3" id="Expression_17_31" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">[</span>&lt;<a href="#Expression_15_3" id="Expression_17_44" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">]</span>&gt;
  
<span class="keyword">context-free priorities</span>

  <a href="#ArrayAccess_11_3" id="ArrayAccess_21_3" title="a reference to a single-file definition">ArrayAccess</a>.<span class="cons_Constructor"><a href="#ArrayAccess_17_15" id="ArrayAccess_21_15" title="a reference to a single-file definition">ArrayAccess</a></span> &lt;0&gt; . &gt; <button class="modal-open" id="Expression_21_35" title="a definition with multiple references" data-urls="#Expression line 17_31, 17_44">Expression</button> = <a href="../ArrayCreation.sdf3/#ArrayCreationExpression_13_3" id="ArrayCreationExpression_21_48" title="a reference to a single-file definition">ArrayCreationExpression</a>
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
