---
title: PackageDeclarations.sdf3
---

# `PackageDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/packages/PackageDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/packages/PackageDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/packages/PackageDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/packages/PackageDeclarations_129_162" id="java/packages/PackageDeclarations_7_40" title="Referenced at ../Main.sdf3 line 8">java/packages/PackageDeclarations</a>

<span class="layout">// 7.4. Package Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_82_106" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_109_136" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  
<span class="keyword">context-free sorts</span>

  <a href="../CompilationUnits.sdf3#PackageDeclaration_282_300" id="PackageDeclaration_162_180" title="Referenced at ../CompilationUnits.sdf3 line 18">PackageDeclaration</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../CompilationUnits.sdf3#PackageDeclaration_282_300" id="PackageDeclaration_207_225" title="Referenced at ../CompilationUnits.sdf3 line 18">PackageDeclaration</a>.<span class="cons_Constructor"><span id="PackageDeclaration_226_244" title="Not referenced locally, nor via imports">PackageDeclaration</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_250_260" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">package</span> &lt;{<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_278_280" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a> <span class="cons_Lit">"."</span>}+&gt;<span class="cons_String">;</span>&gt;
  
</code></pre></td></tr></tbody></table></div>