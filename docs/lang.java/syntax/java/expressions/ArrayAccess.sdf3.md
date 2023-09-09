---
title: ArrayAccess.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/ArrayAccess_212_240" id="java/expressions/ArrayAccess_7_35" title="Referenced at ../Main.sdf3 line 11">java/expressions/ArrayAccess</a>

<span class="layout">// 15.10.3. Array Access Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_85_101" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../ArrayCreation.sdf3#java/expressions/ArrayCreation_7_37" id="java/expressions/ArrayCreation_104_134" title="Defined at ../ArrayCreation.sdf3 line 1">java/expressions/ArrayCreation</a>

<span class="keyword">context-free sorts</span>

  <a href="#ArrayAccess_309_320" id="ArrayAccess_158_169" title="Referenced at line 21; ../AssignmentOperators.sdf3 line 31; ../Disambiguation.sdf3 line 56">ArrayAccess</a>

<span class="keyword">context-free syntax</span>

  <a href="#Expression_265_275" id="Expression_194_204" title="Referenced at line 17">Expression</a> = <a href="#ArrayAccess_158_169" id="ArrayAccess_207_218" title="Defined at line 11, 17">ArrayAccess</a>
  
  <a href="#ArrayAccess_309_320" id="ArrayAccess_224_235" title="Referenced at line 21; ../AssignmentOperators.sdf3 line 31; ../Disambiguation.sdf3 line 56">ArrayAccess</a>.<span class="cons_Constructor"><a href="#ArrayAccess_321_332" id="ArrayAccess_236_247" title="Referenced at line 21; ../Disambiguation.sdf3 line 56">ArrayAccess</a></span> = &lt;&lt;<a href="#Expression_194_204" id="Expression_252_262" title="Defined at line 15, 21">Expression</a>&gt;<span class="cons_String">[</span>&lt;<a href="#Expression_194_204" id="Expression_265_275" title="Defined at line 15, 21">Expression</a>&gt;<span class="cons_String">]</span>&gt;
  
<span class="keyword">context-free priorities</span>

  <a href="#ArrayAccess_158_169" id="ArrayAccess_309_320" title="Defined at line 11, 17">ArrayAccess</a>.<span class="cons_Constructor"><a href="#ArrayAccess_236_247" id="ArrayAccess_321_332" title="Defined at line 17">ArrayAccess</a></span> &lt;0&gt; . &gt; <a href="#Expression_265_275" id="Expression_341_351" title="Referenced at line 17">Expression</a> = <a href="../ArrayCreation.sdf3#ArrayCreationExpression_228_251" id="ArrayCreationExpression_354_377" title="Defined at ../ArrayCreation.sdf3 line 13, 20, 21">ArrayCreationExpression</a>
  
</code></pre></td></tr></tbody></table></div>