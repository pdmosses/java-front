---
title: EnumDeclarations.sdf3
hide:
  - toc
---

# `EnumDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/classes/EnumDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/classes/EnumDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/classes/EnumDeclarations.sdf3 "The source file on GitHub"

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
37
38
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../ClassDeclarations.sdf3/#java/classes/EnumDeclarations_319_348" id="java/classes/EnumDeclarations_7_36" title="Referenced at ../ClassDeclarations.sdf3 line 14; ../Main.sdf3 line 9">java/classes/EnumDeclarations</a>

<span class="layout">// 8.9. Enum Types</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_68_92" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../ClassDeclarations.sdf3/#java/classes/ClassDeclarations_7_37" id="java/classes/ClassDeclarations_95_125" title="Defined at ../ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_128_155" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_7_28" id="java/expressions/Main_158_179" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#EnumDeclaration_751_766" id="EnumDeclaration_203_218" title="Referenced at ../ClassDeclarations.sdf3 line 34">EnumDeclaration</a>
  <a href="#EnumConstant_396_408" id="EnumConstant_221_233" title="Referenced at line 22, 27">EnumConstant</a>
  <a href="#EnumConstantArgs_655_671" id="EnumConstantArgs_236_252" title="Referenced at line 31, 35">EnumConstantArgs</a>
  <a href="#EnumBodyDeclarations_423_443" id="EnumBodyDeclarations_255_275" title="Referenced at line 23, 28">EnumBodyDeclarations</a>

<span class="keyword">context-free syntax</span>

  <a href="../ClassDeclarations.sdf3/#EnumDeclaration_751_766" id="EnumDeclaration_300_315" title="Referenced at ../ClassDeclarations.sdf3 line 34">EnumDeclaration</a>.<span class="cons_Constructor"><span id="EnumDeclComma_316_329" title="Not referenced locally, nor via imports">EnumDeclComma</span></span> = &lt;
  &lt;{<a href="../ClassDeclarations.sdf3/#ClassModifier_551_564" id="ClassModifier_338_351" title="Defined at ../ClassDeclarations.sdf3 line 24, 41, 42, 43, 44, 45, 46, 47, 48">ClassModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">enum</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_365_367" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="../ClassDeclarations.sdf3/#SuperInterfaces_597_612" id="SuperInterfaces_370_385" title="Defined at ../ClassDeclarations.sdf3 line 27, 56">SuperInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#EnumConstant_221_233" id="EnumConstant_396_408" title="Defined at line 14, 30, 34">EnumConstant</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">,</span>
    &lt;<a href="#EnumBodyDeclarations_255_275" id="EnumBodyDeclarations_423_443" title="Defined at line 16, 38">EnumBodyDeclarations</a>?&gt;
  <span class="cons_String">}</span>&gt;
  <a href="../ClassDeclarations.sdf3/#EnumDeclaration_751_766" id="EnumDeclaration_453_468" title="Referenced at ../ClassDeclarations.sdf3 line 34">EnumDeclaration</a>.<span class="cons_Constructor"><span id="EnumDecl_469_477" title="Not referenced locally, nor via imports">EnumDecl</span></span> = &lt;
  &lt;{<a href="../ClassDeclarations.sdf3/#ClassModifier_551_564" id="ClassModifier_486_499" title="Defined at ../ClassDeclarations.sdf3 line 24, 41, 42, 43, 44, 45, 46, 47, 48">ClassModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">enum</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_513_515" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="../ClassDeclarations.sdf3/#SuperInterfaces_597_612" id="SuperInterfaces_518_533" title="Defined at ../ClassDeclarations.sdf3 line 27, 56">SuperInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#EnumConstant_221_233" id="EnumConstant_544_556" title="Defined at line 14, 30, 34">EnumConstant</a> <span class="cons_Lit">", "</span>}*&gt;
    &lt;<a href="#EnumBodyDeclarations_255_275" id="EnumBodyDeclarations_570_590" title="Defined at line 16, 38">EnumBodyDeclarations</a>?&gt;
  <span class="cons_String">}</span>&gt;
  <a href="#EnumConstant_396_408" id="EnumConstant_600_612" title="Referenced at line 22, 27">EnumConstant</a>.<span class="cons_Constructor"><span id="EnumConst_613_622" title="Not referenced locally, nor via imports">EnumConst</span></span> = &lt;
  &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_631_641" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_650_652" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="#EnumConstantArgs_236_252" id="EnumConstantArgs_655_671" title="Defined at line 15, 37">EnumConstantArgs</a>?&gt;<span class="cons_String">{</span>
    &lt;{<a href="../ClassDeclarations.sdf3/#ClassBodyDeclaration_615_635" id="ClassBodyDeclaration_681_701" title="Defined at ../ClassDeclarations.sdf3 line 28, 58, 59, 60, 61">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  <a href="#EnumConstant_396_408" id="EnumConstant_717_729" title="Referenced at line 22, 27">EnumConstant</a>.<span class="cons_Constructor"><span id="EnumConstNoBody_730_745" title="Not referenced locally, nor via imports">EnumConstNoBody</span></span> = &lt;
  &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_754_764" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_773_775" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="#EnumConstantArgs_236_252" id="EnumConstantArgs_778_794" title="Defined at line 15, 37">EnumConstantArgs</a>?&gt;&gt;
  
  <a href="#EnumConstantArgs_655_671" id="EnumConstantArgs_803_819" title="Referenced at line 31, 35">EnumConstantArgs</a>.<span class="cons_Constructor"><span id="EnumConstArgs_820_833" title="Not referenced locally, nor via imports">EnumConstArgs</span></span>    = &lt;<span class="cons_String">(</span>&lt;{<a href="../../expressions/Main.sdf3/#Expression_459_469" id="Expression_843_853" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <a href="#EnumBodyDeclarations_423_443" id="EnumBodyDeclarations_866_886" title="Referenced at line 23, 28">EnumBodyDeclarations</a>.<span class="cons_Constructor"><span id="EnumBodyDecs_887_899" title="Not referenced locally, nor via imports">EnumBodyDecs</span></span> = &lt;<span class="cons_String">;</span>  &lt;{<a href="../ClassDeclarations.sdf3/#ClassBodyDeclaration_615_635" id="ClassBodyDeclaration_908_928" title="Defined at ../ClassDeclarations.sdf3 line 28, 58, 59, 60, 61">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt;
</code></pre></td></tr></tbody></table></div>