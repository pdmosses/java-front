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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Modifiers_1_8" title="a definition with multiple references" data-urls="../Main.sdf3/#java/lexical/Modifiers line 10_3; ../../classes/ClassDeclarations.sdf3/#java/lexical/Modifiers line 7_3; ../../classes/ConstructorDeclarations.sdf3/#java/lexical/Modifiers line 8_3; ../../classes/FieldDeclarations.sdf3/#java/lexical/Modifiers line 7_3; ../../classes/MethodDeclarations.sdf3/#java/lexical/Modifiers line 9_3; ../../interfaces/AnnotationTypes.sdf3/#java/lexical/Modifiers line 8_3; ../../interfaces/ConstantDeclarations.sdf3/#java/lexical/Modifiers line 6_3; ../../interfaces/InterfaceDeclarations.sdf3/#java/lexical/Modifiers line 7_3; ../../interfaces/InterfaceMethodDeclarations.sdf3/#java/lexical/Modifiers line 6_3">java/lexical/Modifiers</button>

<span class="layout">//  modifier keywards get their own productions,</span>
<span class="layout">//  to prevent duplicate constructors</span>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Abstract_8_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Abstract line 45_19; ../../classes/MethodDeclarations.sdf3/#Abstract line 49_20; ../../interfaces/AnnotationTypes.sdf3/#Abstract line 42_35; ../../interfaces/InterfaceDeclarations.sdf3/#Abstract line 37_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Abstract line 22_29">Abstract</button>
  <a href="../../interfaces/InterfaceMethodDeclarations.sdf3/#Default_23_29" id="Default_9_3" title="a definition with a single reference">Default</a>
  <button class="modal-open" id="Final_10_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Final line 47_19; ../../classes/FieldDeclarations.sdf3/#Final line 44_19; ../../classes/MethodDeclarations.sdf3/#Final line 51_20, 74_22; ../../interfaces/ConstantDeclarations.sdf3/#Final line 23_22">Final</button>
  <a href="../../classes/MethodDeclarations.sdf3/#Native_53_20" id="Native_11_3" title="a definition with a single reference">Native</a>
  <button class="modal-open" id="Private_12_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Private line 44_19; ../../classes/ConstructorDeclarations.sdf3/#Private line 32_25; ../../classes/FieldDeclarations.sdf3/#Private line 42_19; ../../classes/MethodDeclarations.sdf3/#Private line 48_20; ../../interfaces/InterfaceDeclarations.sdf3/#Private line 36_23">Private</button>
  <button class="modal-open" id="Protected_13_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Protected line 43_19; ../../classes/ConstructorDeclarations.sdf3/#Protected line 33_25; ../../classes/FieldDeclarations.sdf3/#Protected line 41_19; ../../classes/MethodDeclarations.sdf3/#Protected line 47_20; ../../interfaces/InterfaceDeclarations.sdf3/#Protected line 35_23">Protected</button>
  <button class="modal-open" id="Public_14_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Public line 42_19; ../../classes/ConstructorDeclarations.sdf3/#Public line 31_25; ../../classes/FieldDeclarations.sdf3/#Public line 40_19; ../../classes/MethodDeclarations.sdf3/#Public line 46_20; ../../interfaces/AnnotationTypes.sdf3/#Public line 41_35; ../../interfaces/ConstantDeclarations.sdf3/#Public line 21_22; ../../interfaces/InterfaceDeclarations.sdf3/#Public line 34_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Public line 21_29">Public</button>
  <button class="modal-open" id="Static_15_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Static line 46_19; ../../classes/FieldDeclarations.sdf3/#Static line 43_19; ../../classes/MethodDeclarations.sdf3/#Static line 50_20; ../../interfaces/ConstantDeclarations.sdf3/#Static line 22_22; ../../interfaces/InterfaceDeclarations.sdf3/#Static line 38_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Static line 24_29">Static</button>
  <button class="modal-open" id="Strictfp_16_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Strictfp line 48_19; ../../classes/MethodDeclarations.sdf3/#Strictfp line 54_20; ../../interfaces/InterfaceDeclarations.sdf3/#Strictfp line 39_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Strictfp line 25_29">Strictfp</button>
  <a href="../../classes/MethodDeclarations.sdf3/#Synchronized_52_20" id="Synchronized_17_3" title="a definition with a single reference">Synchronized</a>
  <a href="../../classes/FieldDeclarations.sdf3/#Transient_45_19" id="Transient_18_3" title="a definition with a single reference">Transient</a>
  <a href="../../classes/FieldDeclarations.sdf3/#Volatile_46_19" id="Volatile_19_3" title="a definition with a single reference">Volatile</a>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Abstract_23_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Abstract line 45_19; ../../classes/MethodDeclarations.sdf3/#Abstract line 49_20; ../../interfaces/AnnotationTypes.sdf3/#Abstract line 42_35; ../../interfaces/InterfaceDeclarations.sdf3/#Abstract line 37_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Abstract line 22_29">Abstract</button>    .<span class="cons_Constructor"><span id="Abstract_23_16" title="a definition with no references">Abstract</span></span>     = <span class="cons_Lit">"abstract"</span>
  <a href="../../interfaces/InterfaceMethodDeclarations.sdf3/#Default_23_29" id="Default_24_3" title="a definition with a single reference">Default</a>     .<span class="cons_Constructor"><span id="Default_24_16" title="a definition with no references">Default</span></span>      = <span class="cons_Lit">"default"</span>
  <button class="modal-open" id="Final_25_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Final line 47_19; ../../classes/FieldDeclarations.sdf3/#Final line 44_19; ../../classes/MethodDeclarations.sdf3/#Final line 51_20, 74_22; ../../interfaces/ConstantDeclarations.sdf3/#Final line 23_22">Final</button>       .<span class="cons_Constructor"><span id="Final_25_16" title="a definition with no references">Final</span></span>        = <span class="cons_Lit">"final"</span>
  <a href="../../classes/MethodDeclarations.sdf3/#Native_53_20" id="Native_26_3" title="a definition with a single reference">Native</a>      .<span class="cons_Constructor"><span id="Native_26_16" title="a definition with no references">Native</span></span>       = <span class="cons_Lit">"native"</span>
  <button class="modal-open" id="Private_27_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Private line 44_19; ../../classes/ConstructorDeclarations.sdf3/#Private line 32_25; ../../classes/FieldDeclarations.sdf3/#Private line 42_19; ../../classes/MethodDeclarations.sdf3/#Private line 48_20; ../../interfaces/InterfaceDeclarations.sdf3/#Private line 36_23">Private</button>     .<span class="cons_Constructor"><span id="Private_27_16" title="a definition with no references">Private</span></span>      = <span class="cons_Lit">"private"</span>
  <button class="modal-open" id="Protected_28_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Protected line 43_19; ../../classes/ConstructorDeclarations.sdf3/#Protected line 33_25; ../../classes/FieldDeclarations.sdf3/#Protected line 41_19; ../../classes/MethodDeclarations.sdf3/#Protected line 47_20; ../../interfaces/InterfaceDeclarations.sdf3/#Protected line 35_23">Protected</button>   .<span class="cons_Constructor"><span id="Protected_28_16" title="a definition with no references">Protected</span></span>    = <span class="cons_Lit">"protected"</span>
  <button class="modal-open" id="Public_29_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Public line 42_19; ../../classes/ConstructorDeclarations.sdf3/#Public line 31_25; ../../classes/FieldDeclarations.sdf3/#Public line 40_19; ../../classes/MethodDeclarations.sdf3/#Public line 46_20; ../../interfaces/AnnotationTypes.sdf3/#Public line 41_35; ../../interfaces/ConstantDeclarations.sdf3/#Public line 21_22; ../../interfaces/InterfaceDeclarations.sdf3/#Public line 34_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Public line 21_29">Public</button>      .<span class="cons_Constructor"><span id="Public_29_16" title="a definition with no references">Public</span></span>       = <span class="cons_Lit">"public"</span>
  <button class="modal-open" id="Static_30_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Static line 46_19; ../../classes/FieldDeclarations.sdf3/#Static line 43_19; ../../classes/MethodDeclarations.sdf3/#Static line 50_20; ../../interfaces/ConstantDeclarations.sdf3/#Static line 22_22; ../../interfaces/InterfaceDeclarations.sdf3/#Static line 38_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Static line 24_29">Static</button>      .<span class="cons_Constructor"><span id="Static_30_16" title="a definition with no references">Static</span></span>       = <span class="cons_Lit">"static"</span>
  <button class="modal-open" id="Strictfp_31_3" title="a definition with multiple references" data-urls="../../classes/ClassDeclarations.sdf3/#Strictfp line 48_19; ../../classes/MethodDeclarations.sdf3/#Strictfp line 54_20; ../../interfaces/InterfaceDeclarations.sdf3/#Strictfp line 39_23; ../../interfaces/InterfaceMethodDeclarations.sdf3/#Strictfp line 25_29">Strictfp</button>    .<span class="cons_Constructor"><span id="Strictfp_31_16" title="a definition with no references">Strictfp</span></span>     = <span class="cons_Lit">"strictfp"</span>
  <a href="../../classes/FieldDeclarations.sdf3/#Transient_45_19" id="Transient_32_3" title="a definition with a single reference">Transient</a>   .<span class="cons_Constructor"><span id="Transient_32_16" title="a definition with no references">Transient</span></span>    = <span class="cons_Lit">"transient"</span>
  <a href="../../classes/FieldDeclarations.sdf3/#Volatile_46_19" id="Volatile_33_3" title="a definition with a single reference">Volatile</a>    .<span class="cons_Constructor"><span id="Volatile_33_16" title="a definition with no references">Volatile</span></span>     = <span class="cons_Lit">"volatile"</span>
  <a href="../../classes/MethodDeclarations.sdf3/#Synchronized_52_20" id="Synchronized_34_3" title="a definition with a single reference">Synchronized</a>.<span class="cons_Constructor"><span id="Synchronized_34_16" title="a definition with no references">Synchronized</span></span> = <span class="cons_Lit">"synchronized"</span>

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
