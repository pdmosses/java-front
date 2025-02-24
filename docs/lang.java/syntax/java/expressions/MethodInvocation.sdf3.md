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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/MethodInvocation_1_8" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#java/expressions/MethodInvocation line 10_3; ../Main.sdf3/#java/expressions/MethodInvocation line 12_3">java/expressions/MethodInvocation</button>

<span class="layout">// 15.12. Method Invocation Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../types/ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_8_3" title="a reference to a single-file definition">java/types/ParameterizedTypes</a>
  
<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="Expression_12_3" title="a definition with multiple references" data-urls="#Expression line 12_48, 16_34, 16_70, 17_63, 18_74">Expression</button>.<span class="cons_Constructor"><span id="Invoke_12_14" title="a definition with no references">Invoke</span></span>          = &lt;&lt;<a href="../../names/Names.sdf3/#MethodName_15_3" id="MethodName_12_34" title="a reference to a single-file definition">MethodName</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_12_3" id="Expression_12_48" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
<span class="layout">//  ambiguous with Expression?</span>
<span class="layout">//  Expression.InvokeQTypeName = &lt;&lt;TypeName&gt;.&lt;TypeArguments?&gt; &lt;Id&gt;(&lt;{Expression ", "}*&gt;)&gt;</span>
<span class="layout">//  Expression.InvokeQExpName  = &lt;&lt;ExpressionName&gt;.&lt;TypeArguments?&gt; &lt;Id&gt;(&lt;{Expression ", "}*&gt;)&gt;</span>
  <button class="modal-open" id="Expression_16_3" title="a definition with multiple references" data-urls="#Expression line 12_48, 16_34, 16_70, 17_63, 18_74">Expression</button>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#InvokeQExp_58_16" id="InvokeQExp_16_14" title="a definition with a single reference">InvokeQExp</a></span>      = &lt;&lt;<a href="#Expression_12_3" id="Expression_16_34" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_16_47" title="a reference to a single-file definition">TypeArguments</a>?&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_16_64" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_12_3" id="Expression_16_70" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <button class="modal-open" id="Expression_17_3" title="a definition with multiple references" data-urls="#Expression line 12_48, 16_34, 16_70, 17_63, 18_74">Expression</button>.<span class="cons_Constructor"><span id="InvokeSuper_17_14" title="a definition with no references">InvokeSuper</span></span>     = &lt;<span class="cons_String">super.</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_17_40" title="a reference to a single-file definition">TypeArguments</a>?&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_17_57" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_12_3" id="Expression_17_63" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <button class="modal-open" id="Expression_18_3" title="a definition with multiple references" data-urls="#Expression line 12_48, 16_34, 16_70, 17_63, 18_74">Expression</button>.<span class="cons_Constructor"><span id="InvokeQSuper_18_14" title="a definition with no references">InvokeQSuper</span></span>    = &lt;&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_18_34" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">.super.</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_18_51" title="a reference to a single-file definition">TypeArguments</a>?&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_18_68" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_12_3" id="Expression_18_74" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
