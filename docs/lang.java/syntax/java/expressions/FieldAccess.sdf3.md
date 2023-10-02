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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/FieldAccess_181_209" id="java/expressions/FieldAccess_7_35" title="Referenced at ../Main.sdf3 line 10">java/expressions/FieldAccess</a>

<span class="layout">// 15.11. Field Access Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_83_99" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_102_126" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../Main.sdf3#java/expressions/Main_7_28" id="java/expressions/Main_129_150" title="Defined at ../Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="#FieldAccess_225_236" id="FieldAccess_174_185" title="Referenced at line 16; ../AssignmentOperators.sdf3 line 30; ../Disambiguation.sdf3 line 57">FieldAccess</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_270_280" id="Expression_212_222" title="Referenced at line 18">Expression</a> = <a href="#FieldAccess_174_185" id="FieldAccess_225_236" title="Defined at line 12, 18, 19, 20">FieldAccess</a>
  
  <a href="#FieldAccess_225_236" id="FieldAccess_242_253" title="Referenced at line 16; ../AssignmentOperators.sdf3 line 30; ../Disambiguation.sdf3 line 57">FieldAccess</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Field_1150_1155" id="Field_254_259" title="Referenced at ../Disambiguation.sdf3 line 57">Field</a></span>       = &lt;&lt;<a href="#Expression_212_222" id="Expression_270_280" title="Defined at line 16">Expression</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_283_285" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#FieldAccess_225_236" id="FieldAccess_290_301" title="Referenced at line 16; ../AssignmentOperators.sdf3 line 30; ../Disambiguation.sdf3 line 57">FieldAccess</a>.<span class="cons_Constructor"><span id="SuperField_302_312" title="Not referenced locally, nor via imports">SuperField</span></span>  = &lt;<span class="cons_String">super.</span>&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_324_326" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#FieldAccess_225_236" id="FieldAccess_331_342" title="Referenced at line 16; ../AssignmentOperators.sdf3 line 30; ../Disambiguation.sdf3 line 57">FieldAccess</a>.<span class="cons_Constructor"><span id="QSuperField_343_354" title="Not referenced locally, nor via imports">QSuperField</span></span> = &lt;&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_359_367" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">.super.</span>&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_376_378" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;


<span class="keyword">template options</span>
  
  <span class="keyword">tokenize</span> : "."
  
  
</code></pre></td></tr></tbody></table></div>