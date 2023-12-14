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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Modifiers_1_8" title="Multi-file references" data-urls="../Main.sdf3/#java/lexical/Modifiers_10_3 line 10; ../../classes/ClassDeclarations.sdf3/#java/lexical/Modifiers_7_3 line 7; ../../classes/ConstructorDeclarations.sdf3/#java/lexical/Modifiers_8_3 line 8; ../../classes/FieldDeclarations.sdf3/#java/lexical/Modifiers_7_3 line 7; ../../classes/MethodDeclarations.sdf3/#java/lexical/Modifiers_9_3 line 9; ../../interfaces/AnnotationTypes.sdf3/#java/lexical/Modifiers_8_3 line 8; ../../interfaces/ConstantDeclarations.sdf3/#java/lexical/Modifiers_6_3 line 6; ../../interfaces/InterfaceDeclarations.sdf3/#java/lexical/Modifiers_7_3 line 7; ../../interfaces/InterfaceMethodDeclarations.sdf3/#java/lexical/Modifiers_6_3 line 6">java/lexical/Modifiers</button>

<span class="layout">//  modifier keywards get their own productions,</span>
<span class="layout">//  to prevent duplicate constructors</span>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Abstract_8_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Abstract_45_19 line 45; ../../classes/MethodDeclarations.sdf3/#Abstract_49_20 line 49; ../../interfaces/AnnotationTypes.sdf3/#Abstract_42_35 line 42; ../../interfaces/InterfaceDeclarations.sdf3/#Abstract_37_23 line 37; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Abstract_22_29 line 22">Abstract</button>
  <a href="../../interfaces/InterfaceMethodDeclarations.sdf3/#Default_23_29" id="Default_9_3" title="Referenced at ../../interfaces/InterfaceMethodDeclarations.sdf3 line 23">Default</a>
  <button class="modal-open" id="Final_10_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Final_47_19 line 47; ../../classes/FieldDeclarations.sdf3/#Final_44_19 line 44; ../../classes/MethodDeclarations.sdf3/#Final_51_20 line 51, 74; ../../interfaces/ConstantDeclarations.sdf3/#Final_23_22 line 23">Final</button>
  <a href="../../classes/MethodDeclarations.sdf3/#Native_53_20" id="Native_11_3" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 53">Native</a>
  <button class="modal-open" id="Private_12_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Private_44_19 line 44; ../../classes/ConstructorDeclarations.sdf3/#Private_32_25 line 32; ../../classes/FieldDeclarations.sdf3/#Private_42_19 line 42; ../../classes/MethodDeclarations.sdf3/#Private_48_20 line 48; ../../interfaces/InterfaceDeclarations.sdf3/#Private_36_23 line 36">Private</button>
  <button class="modal-open" id="Protected_13_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Protected_43_19 line 43; ../../classes/ConstructorDeclarations.sdf3/#Protected_33_25 line 33; ../../classes/FieldDeclarations.sdf3/#Protected_41_19 line 41; ../../classes/MethodDeclarations.sdf3/#Protected_47_20 line 47; ../../interfaces/InterfaceDeclarations.sdf3/#Protected_35_23 line 35">Protected</button>
  <button class="modal-open" id="Public_14_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Public_42_19 line 42; ../../classes/ConstructorDeclarations.sdf3/#Public_31_25 line 31; ../../classes/FieldDeclarations.sdf3/#Public_40_19 line 40; ../../classes/MethodDeclarations.sdf3/#Public_46_20 line 46; ../../interfaces/AnnotationTypes.sdf3/#Public_41_35 line 41; ../../interfaces/ConstantDeclarations.sdf3/#Public_21_22 line 21; ../../interfaces/InterfaceDeclarations.sdf3/#Public_34_23 line 34; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Public_21_29 line 21">Public</button>
  <button class="modal-open" id="Static_15_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Static_46_19 line 46; ../../classes/FieldDeclarations.sdf3/#Static_43_19 line 43; ../../classes/MethodDeclarations.sdf3/#Static_50_20 line 50; ../../interfaces/ConstantDeclarations.sdf3/#Static_22_22 line 22; ../../interfaces/InterfaceDeclarations.sdf3/#Static_38_23 line 38; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Static_24_29 line 24">Static</button>
  <button class="modal-open" id="Strictfp_16_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Strictfp_48_19 line 48; ../../classes/MethodDeclarations.sdf3/#Strictfp_54_20 line 54; ../../interfaces/InterfaceDeclarations.sdf3/#Strictfp_39_23 line 39; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Strictfp_25_29 line 25">Strictfp</button>
  <a href="../../classes/MethodDeclarations.sdf3/#Synchronized_52_20" id="Synchronized_17_3" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 52">Synchronized</a>
  <a href="../../classes/FieldDeclarations.sdf3/#Transient_45_19" id="Transient_18_3" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 45">Transient</a>
  <a href="../../classes/FieldDeclarations.sdf3/#Volatile_46_19" id="Volatile_19_3" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 46">Volatile</a>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Abstract_23_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Abstract_45_19 line 45; ../../classes/MethodDeclarations.sdf3/#Abstract_49_20 line 49; ../../interfaces/AnnotationTypes.sdf3/#Abstract_42_35 line 42; ../../interfaces/InterfaceDeclarations.sdf3/#Abstract_37_23 line 37; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Abstract_22_29 line 22">Abstract</button>    .<span class="cons_Constructor"><span id="Abstract_23_16" title="Not referenced">Abstract</span></span>     = <span class="cons_Lit">"abstract"</span>
  <a href="../../interfaces/InterfaceMethodDeclarations.sdf3/#Default_23_29" id="Default_24_3" title="Referenced at ../../interfaces/InterfaceMethodDeclarations.sdf3 line 23">Default</a>     .<span class="cons_Constructor"><span id="Default_24_16" title="Not referenced">Default</span></span>      = <span class="cons_Lit">"default"</span>
  <button class="modal-open" id="Final_25_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Final_47_19 line 47; ../../classes/FieldDeclarations.sdf3/#Final_44_19 line 44; ../../classes/MethodDeclarations.sdf3/#Final_51_20 line 51, 74; ../../interfaces/ConstantDeclarations.sdf3/#Final_23_22 line 23">Final</button>       .<span class="cons_Constructor"><span id="Final_25_16" title="Not referenced">Final</span></span>        = <span class="cons_Lit">"final"</span>
  <a href="../../classes/MethodDeclarations.sdf3/#Native_53_20" id="Native_26_3" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 53">Native</a>      .<span class="cons_Constructor"><span id="Native_26_16" title="Not referenced">Native</span></span>       = <span class="cons_Lit">"native"</span>
  <button class="modal-open" id="Private_27_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Private_44_19 line 44; ../../classes/ConstructorDeclarations.sdf3/#Private_32_25 line 32; ../../classes/FieldDeclarations.sdf3/#Private_42_19 line 42; ../../classes/MethodDeclarations.sdf3/#Private_48_20 line 48; ../../interfaces/InterfaceDeclarations.sdf3/#Private_36_23 line 36">Private</button>     .<span class="cons_Constructor"><span id="Private_27_16" title="Not referenced">Private</span></span>      = <span class="cons_Lit">"private"</span>
  <button class="modal-open" id="Protected_28_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Protected_43_19 line 43; ../../classes/ConstructorDeclarations.sdf3/#Protected_33_25 line 33; ../../classes/FieldDeclarations.sdf3/#Protected_41_19 line 41; ../../classes/MethodDeclarations.sdf3/#Protected_47_20 line 47; ../../interfaces/InterfaceDeclarations.sdf3/#Protected_35_23 line 35">Protected</button>   .<span class="cons_Constructor"><span id="Protected_28_16" title="Not referenced">Protected</span></span>    = <span class="cons_Lit">"protected"</span>
  <button class="modal-open" id="Public_29_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Public_42_19 line 42; ../../classes/ConstructorDeclarations.sdf3/#Public_31_25 line 31; ../../classes/FieldDeclarations.sdf3/#Public_40_19 line 40; ../../classes/MethodDeclarations.sdf3/#Public_46_20 line 46; ../../interfaces/AnnotationTypes.sdf3/#Public_41_35 line 41; ../../interfaces/ConstantDeclarations.sdf3/#Public_21_22 line 21; ../../interfaces/InterfaceDeclarations.sdf3/#Public_34_23 line 34; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Public_21_29 line 21">Public</button>      .<span class="cons_Constructor"><span id="Public_29_16" title="Not referenced">Public</span></span>       = <span class="cons_Lit">"public"</span>
  <button class="modal-open" id="Static_30_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Static_46_19 line 46; ../../classes/FieldDeclarations.sdf3/#Static_43_19 line 43; ../../classes/MethodDeclarations.sdf3/#Static_50_20 line 50; ../../interfaces/ConstantDeclarations.sdf3/#Static_22_22 line 22; ../../interfaces/InterfaceDeclarations.sdf3/#Static_38_23 line 38; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Static_24_29 line 24">Static</button>      .<span class="cons_Constructor"><span id="Static_30_16" title="Not referenced">Static</span></span>       = <span class="cons_Lit">"static"</span>
  <button class="modal-open" id="Strictfp_31_3" title="Multi-file references" data-urls="../../classes/ClassDeclarations.sdf3/#Strictfp_48_19 line 48; ../../classes/MethodDeclarations.sdf3/#Strictfp_54_20 line 54; ../../interfaces/InterfaceDeclarations.sdf3/#Strictfp_39_23 line 39; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Strictfp_25_29 line 25">Strictfp</button>    .<span class="cons_Constructor"><span id="Strictfp_31_16" title="Not referenced">Strictfp</span></span>     = <span class="cons_Lit">"strictfp"</span>
  <a href="../../classes/FieldDeclarations.sdf3/#Transient_45_19" id="Transient_32_3" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 45">Transient</a>   .<span class="cons_Constructor"><span id="Transient_32_16" title="Not referenced">Transient</span></span>    = <span class="cons_Lit">"transient"</span>
  <a href="../../classes/FieldDeclarations.sdf3/#Volatile_46_19" id="Volatile_33_3" title="Referenced at ../../classes/FieldDeclarations.sdf3 line 46">Volatile</a>    .<span class="cons_Constructor"><span id="Volatile_33_16" title="Not referenced">Volatile</span></span>     = <span class="cons_Lit">"volatile"</span>
  <a href="../../classes/MethodDeclarations.sdf3/#Synchronized_52_20" id="Synchronized_34_3" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 52">Synchronized</a>.<span class="cons_Constructor"><span id="Synchronized_34_16" title="Not referenced">Synchronized</span></span> = <span class="cons_Lit">"synchronized"</span>

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
