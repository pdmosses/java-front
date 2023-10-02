---
title: Modifiers.sdf3
hide:
  - toc
---

# `Modifiers.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/Modifiers.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/Modifiers.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/Modifiers.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/lexical/Modifiers_175_197" id="java/lexical/Modifiers_7_29" title="Referenced at ../Main.sdf3 line 10">java/lexical/Modifiers</a>

<span class="layout">//  modifier keywards get their own productions,</span>
<span class="layout">//  to prevent duplicate constructors</span>

<span class="keyword">context-free sorts</span>

  <a href="../../classes/ClassDeclarations.sdf3#Abstract_1073_1081" id="Abstract_141_149" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 45; ../../classes/MethodDeclarations.sdf3 line 49; ../../interfaces/AnnotationTypes.sdf3 line 42; ../../interfaces/InterfaceDeclarations.sdf3 line 37; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 22">Abstract</a>
  <a href="../../interfaces/InterfaceMethodDeclarations.sdf3#Default_536_543" id="Default_152_159" title="Referenced at ../../interfaces/InterfaceMethodDeclarations.sdf3 line 23">Default</a>
  <a href="../../classes/ClassDeclarations.sdf3#Final_1125_1130" id="Final_162_167" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 47; ../../classes/FieldDeclarations.sdf3 line 44; ../../classes/MethodDeclarations.sdf3 line 74; ../../interfaces/ConstantDeclarations.sdf3 line 23">Final</a>
  <a href="../../classes/MethodDeclarations.sdf3#Native_1201_1207" id="Native_170_176" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 53">Native</a>
  <a href="../../classes/ClassDeclarations.sdf3#Private_1047_1054" id="Private_179_186" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 44; ../../classes/ConstructorDeclarations.sdf3 line 32; ../../classes/FieldDeclarations.sdf3 line 42; ../../classes/MethodDeclarations.sdf3 line 48; ../../interfaces/InterfaceDeclarations.sdf3 line 36">Private</a>
  <a href="../../classes/ClassDeclarations.sdf3#Protected_1019_1028" id="Protected_189_198" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 43; ../../classes/ConstructorDeclarations.sdf3 line 33; ../../classes/FieldDeclarations.sdf3 line 41; ../../classes/MethodDeclarations.sdf3 line 47; ../../interfaces/InterfaceDeclarations.sdf3 line 35">Protected</a>
  <a href="../../classes/ClassDeclarations.sdf3#Public_994_1000" id="Public_201_207" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 42; ../../classes/ConstructorDeclarations.sdf3 line 31; ../../classes/FieldDeclarations.sdf3 line 40; ../../classes/MethodDeclarations.sdf3 line 46; ../../interfaces/AnnotationTypes.sdf3 line 41; ../../interfaces/ConstantDeclarations.sdf3 line 21; ../../interfaces/InterfaceDeclarations.sdf3 line 34; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 21">Public</a>
  <a href="../../classes/ClassDeclarations.sdf3#Static_1100_1106" id="Static_210_216" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 46; ../../classes/FieldDeclarations.sdf3 line 43; ../../classes/MethodDeclarations.sdf3 line 50; ../../interfaces/ConstantDeclarations.sdf3 line 22; ../../interfaces/InterfaceDeclarations.sdf3 line 38; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 24">Static</a>
  <a href="../../classes/ClassDeclarations.sdf3#Strictfp_1149_1157" id="Strictfp_219_227" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 48; ../../classes/MethodDeclarations.sdf3 line 54; ../../interfaces/InterfaceDeclarations.sdf3 line 39; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 25">Strictfp</a>
  <a href="../../classes/MethodDeclarations.sdf3#Synchronized_1169_1181" id="Synchronized_230_242" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 52">Synchronized</a>
  <a href="../../classes/FieldDeclarations.sdf3#Transient_1058_1067" id="Transient_245_254" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 45">Transient</a>
  <a href="../../classes/FieldDeclarations.sdf3#Volatile_1086_1094" id="Volatile_257_265" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 46">Volatile</a>

<span class="keyword">context-free syntax</span>

  <a href="../../classes/ClassDeclarations.sdf3#Abstract_1073_1081" id="Abstract_290_298" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 45; ../../classes/MethodDeclarations.sdf3 line 49; ../../interfaces/AnnotationTypes.sdf3 line 42; ../../interfaces/InterfaceDeclarations.sdf3 line 37; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 22">Abstract</a>    .<span class="cons_Constructor"><span id="Abstract_303_311" title="Not referenced locally, nor via imports">Abstract</span></span>     = <span class="cons_Lit">"abstract"</span>
  <a href="../../interfaces/InterfaceMethodDeclarations.sdf3#Default_536_543" id="Default_331_338" title="Referenced at ../../interfaces/InterfaceMethodDeclarations.sdf3 line 23">Default</a>     .<span class="cons_Constructor"><span id="Default_344_351" title="Not referenced locally, nor via imports">Default</span></span>      = <span class="cons_Lit">"default"</span>
  <a href="../../classes/ClassDeclarations.sdf3#Final_1125_1130" id="Final_371_376" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 47; ../../classes/FieldDeclarations.sdf3 line 44; ../../classes/MethodDeclarations.sdf3 line 74; ../../interfaces/ConstantDeclarations.sdf3 line 23">Final</a>       .<span class="cons_Constructor"><span id="Final_384_389" title="Not referenced locally, nor via imports">Final</span></span>        = <span class="cons_Lit">"final"</span>
  <a href="../../classes/MethodDeclarations.sdf3#Native_1201_1207" id="Native_409_415" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 53">Native</a>      .<span class="cons_Constructor"><span id="Native_422_428" title="Not referenced locally, nor via imports">Native</span></span>       = <span class="cons_Lit">"native"</span>
  <a href="../../classes/ClassDeclarations.sdf3#Private_1047_1054" id="Private_448_455" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 44; ../../classes/ConstructorDeclarations.sdf3 line 32; ../../classes/FieldDeclarations.sdf3 line 42; ../../classes/MethodDeclarations.sdf3 line 48; ../../interfaces/InterfaceDeclarations.sdf3 line 36">Private</a>     .<span class="cons_Constructor"><span id="Private_461_468" title="Not referenced locally, nor via imports">Private</span></span>      = <span class="cons_Lit">"private"</span>
  <a href="../../classes/ClassDeclarations.sdf3#Protected_1019_1028" id="Protected_488_497" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 43; ../../classes/ConstructorDeclarations.sdf3 line 33; ../../classes/FieldDeclarations.sdf3 line 41; ../../classes/MethodDeclarations.sdf3 line 47; ../../interfaces/InterfaceDeclarations.sdf3 line 35">Protected</a>   .<span class="cons_Constructor"><span id="Protected_501_510" title="Not referenced locally, nor via imports">Protected</span></span>    = <span class="cons_Lit">"protected"</span>
  <a href="../../classes/ClassDeclarations.sdf3#Public_994_1000" id="Public_530_536" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 42; ../../classes/ConstructorDeclarations.sdf3 line 31; ../../classes/FieldDeclarations.sdf3 line 40; ../../classes/MethodDeclarations.sdf3 line 46; ../../interfaces/AnnotationTypes.sdf3 line 41; ../../interfaces/ConstantDeclarations.sdf3 line 21; ../../interfaces/InterfaceDeclarations.sdf3 line 34; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 21">Public</a>      .<span class="cons_Constructor"><span id="Public_543_549" title="Not referenced locally, nor via imports">Public</span></span>       = <span class="cons_Lit">"public"</span>
  <a href="../../classes/ClassDeclarations.sdf3#Static_1100_1106" id="Static_569_575" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 46; ../../classes/FieldDeclarations.sdf3 line 43; ../../classes/MethodDeclarations.sdf3 line 50; ../../interfaces/ConstantDeclarations.sdf3 line 22; ../../interfaces/InterfaceDeclarations.sdf3 line 38; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 24">Static</a>      .<span class="cons_Constructor"><span id="Static_582_588" title="Not referenced locally, nor via imports">Static</span></span>       = <span class="cons_Lit">"static"</span>
  <a href="../../classes/ClassDeclarations.sdf3#Strictfp_1149_1157" id="Strictfp_608_616" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 48; ../../classes/MethodDeclarations.sdf3 line 54; ../../interfaces/InterfaceDeclarations.sdf3 line 39; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 25">Strictfp</a>    .<span class="cons_Constructor"><span id="Strictfp_621_629" title="Not referenced locally, nor via imports">Strictfp</span></span>     = <span class="cons_Lit">"strictfp"</span>
  <a href="../../classes/FieldDeclarations.sdf3#Transient_1058_1067" id="Transient_649_658" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 45">Transient</a>   .<span class="cons_Constructor"><span id="Transient_662_671" title="Not referenced locally, nor via imports">Transient</span></span>    = <span class="cons_Lit">"transient"</span>
  <a href="../../classes/FieldDeclarations.sdf3#Volatile_1086_1094" id="Volatile_691_699" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 46">Volatile</a>    .<span class="cons_Constructor"><span id="Volatile_704_712" title="Not referenced locally, nor via imports">Volatile</span></span>     = <span class="cons_Lit">"volatile"</span>
  <a href="../../classes/MethodDeclarations.sdf3#Synchronized_1169_1181" id="Synchronized_732_744" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 52">Synchronized</a>.<span class="cons_Constructor"><span id="Synchronized_745_757" title="Not referenced locally, nor via imports">Synchronized</span></span> = <span class="cons_Lit">"synchronized"</span>

</code></pre></td></tr></tbody></table></div>