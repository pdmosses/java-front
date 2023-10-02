---
title: MethodInvocation.sdf3
hide:
  - toc
---

# `MethodInvocation.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/MethodInvocation.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/MethodInvocation.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/MethodInvocation.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/MethodInvocation_243_276" id="java/expressions/MethodInvocation_7_40" title="Referenced at ../Main.sdf3 line 12">java/expressions/MethodInvocation</a>

<span class="layout">// 15.12. Method Invocation Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_93_109" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_112_136" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../types/ParameterizedTypes.sdf3#java/types/ParameterizedTypes_7_36" id="java/types/ParameterizedTypes_139_168" title="Defined at ../../types/ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  
<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_726_736" id="Expression_197_207" title="Referenced at line 18">Expression</a>.<span class="cons_Constructor"><span id="Invoke_208_214" title="Not referenced locally, nor via imports">Invoke</span></span>          = &lt;&lt;<a href="../../names/Names.sdf3#MethodName_209_219" id="MethodName_228_238" title="Defined at ../../names/Names.sdf3 line 15, 29">MethodName</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_197_207" id="Expression_242_252" title="Defined at line 12, 16, 17, 18">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
<span class="layout">//  ambiguous with Expression?</span>
<span class="layout">//  Expression.InvokeQTypeName = &lt;&lt;TypeName&gt;.&lt;TypeArguments?&gt; &lt;Id&gt;(&lt;{Expression ", "}*&gt;)&gt;</span>
<span class="layout">//  Expression.InvokeQExpName  = &lt;&lt;ExpressionName&gt;.&lt;TypeArguments?&gt; &lt;Id&gt;(&lt;{Expression ", "}*&gt;)&gt;</span>
  <a href="#Expression_726_736" id="Expression_482_492" title="Referenced at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#InvokeQExp_1172_1182" id="InvokeQExp_493_503" title="Referenced at ../Disambiguation.sdf3 line 58">InvokeQExp</a></span>      = &lt;&lt;<a href="#Expression_197_207" id="Expression_513_523" title="Defined at line 12, 16, 17, 18">Expression</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_526_539" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_543_545" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_197_207" id="Expression_549_559" title="Defined at line 12, 16, 17, 18">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <a href="#Expression_726_736" id="Expression_572_582" title="Referenced at line 18">Expression</a>.<span class="cons_Constructor"><span id="InvokeSuper_583_594" title="Not referenced locally, nor via imports">InvokeSuper</span></span>     = &lt;<span class="cons_String">super.</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_609_622" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_626_628" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_197_207" id="Expression_632_642" title="Defined at line 12, 16, 17, 18">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <a href="#Expression_726_736" id="Expression_655_665" title="Referenced at line 18">Expression</a>.<span class="cons_Constructor"><span id="InvokeQSuper_666_678" title="Not referenced locally, nor via imports">InvokeQSuper</span></span>    = &lt;&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_686_694" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">.super.</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_703_716" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_720_722" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_197_207" id="Expression_726_736" title="Defined at line 12, 16, 17, 18">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
</code></pre></td></tr></tbody></table></div>