---
title: ArrayInitializers.sdf3
---

# `ArrayInitializers.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/arrays/ArrayInitializers.sdf3]

[pdmosses/java-front/lang.java/syntax/java/arrays/ArrayInitializers.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/arrays/ArrayInitializers.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../expressions/ArrayCreation.sdf3#java/arrays/ArrayInitializers_175_204" id="java/arrays/ArrayInitializers_7_36" title="Referenced at ../../expressions/ArrayCreation.sdf3 line 9">java/arrays/ArrayInitializers</a>

<span class="layout">// 10.6. Array Initializers</span>

<span class="keyword">imports</span>
  <a href="../../classes/FieldDeclarations.sdf3#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_77_107" title="Defined at ../../classes/FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  
<span class="keyword">context-free sorts</span>

  <a href="../../classes/FieldDeclarations.sdf3#ArrayInitializer_863_879" id="ArrayInitializer_133_149" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 37; ../../expressions/ArrayCreation.sdf3 line 21">ArrayInitializer</a>
  
<span class="keyword">context-free syntax</span>
  
  <a href="../../classes/FieldDeclarations.sdf3#ArrayInitializer_863_879" id="ArrayInitializer_178_194" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 37; ../../expressions/ArrayCreation.sdf3 line 21">ArrayInitializer</a>.<span class="cons_Constructor"><span id="ArrayInit_195_204" title="Not referenced locally, nor via imports">ArrayInit</span></span>      = &lt;<span class="cons_String">{</span>&lt;{<a href="../../classes/FieldDeclarations.sdf3#VariableInitializer_365_384" id="VariableInitializer_216_235" title="Defined at ../../classes/FieldDeclarations.sdf3 line 20, 36, 37">VariableInitializer</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">}</span>&gt;
  <a href="../../classes/FieldDeclarations.sdf3#ArrayInitializer_863_879" id="ArrayInitializer_247_263" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 37; ../../expressions/ArrayCreation.sdf3 line 21">ArrayInitializer</a>.<span class="cons_Constructor"><span id="ArrayInitComma_264_278" title="Not referenced locally, nor via imports">ArrayInitComma</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="../../classes/FieldDeclarations.sdf3#VariableInitializer_365_384" id="VariableInitializer_285_304" title="Defined at ../../classes/FieldDeclarations.sdf3 line 20, 36, 37">VariableInitializer</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> <span class="cons_String">}</span>&gt;
</code></pre></td></tr></tbody></table></div>