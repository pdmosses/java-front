---
title: FieldAccess.sdf3
hide:
  - toc
---

# `FieldAccess.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/FieldAccess.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/FieldAccess.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/FieldAccess.sdf3 "The source file on GitHub"

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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/FieldAccess_1_8" title="a definition with multiple references" data-urls="../AssignmentOperators.sdf3/#java/expressions/FieldAccess line 7_3; ../Disambiguation.sdf3/#java/expressions/FieldAccess line 9_3; ../Main.sdf3/#java/expressions/FieldAccess line 10_3">java/expressions/FieldAccess</button>

<span class="layout">// 15.11. Field Access Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_8_3" title="a reference to a single-file definition">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="FieldAccess_12_3" title="a definition with multiple references" data-urls="#FieldAccess line 16_16; ../AssignmentOperators.sdf3/#FieldAccess line 30_9; ../Disambiguation.sdf3/#FieldAccess line 17_3, 57_5">FieldAccess</button>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_18_31" id="Expression_16_3" title="a definition with a single reference">Expression</a> = <a href="#FieldAccess_12_3" id="FieldAccess_16_16" title="a reference to a single-file definition">FieldAccess</a>
  
  <button class="modal-open" id="FieldAccess_18_3" title="a definition with multiple references" data-urls="#FieldAccess line 16_16; ../AssignmentOperators.sdf3/#FieldAccess line 30_9; ../Disambiguation.sdf3/#FieldAccess line 17_3, 57_5">FieldAccess</button>.<span class="cons_Constructor"><button class="modal-open" id="Field_18_15" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#Field line 17_15, 57_17">Field</button></span>       = &lt;&lt;<a href="#Expression_16_3" id="Expression_18_31" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_18_44" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="FieldAccess_19_3" title="a definition with multiple references" data-urls="#FieldAccess line 16_16; ../AssignmentOperators.sdf3/#FieldAccess line 30_9; ../Disambiguation.sdf3/#FieldAccess line 17_3, 57_5">FieldAccess</button>.<span class="cons_Constructor"><span id="SuperField_19_15" title="a definition with no references">SuperField</span></span>  = &lt;<span class="cons_String">super.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_19_37" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="FieldAccess_20_3" title="a definition with multiple references" data-urls="#FieldAccess line 16_16; ../AssignmentOperators.sdf3/#FieldAccess line 30_9; ../Disambiguation.sdf3/#FieldAccess line 17_3, 57_5">FieldAccess</button>.<span class="cons_Constructor"><span id="QSuperField_20_15" title="a definition with no references">QSuperField</span></span> = &lt;&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_20_31" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">.super.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_20_48" title="a reference to a single-file definition">Id</a>&gt;&gt;


<span class="keyword">template options</span>
  
  <span class="keyword">tokenize</span> : "."
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
