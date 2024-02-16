---
title: ImportDeclarations.sdf3
hide:
  - toc
---

# `ImportDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/packages/ImportDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/packages/ImportDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/packages/ImportDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/packages/ImportDeclarations_1_8" title="a definition with multiple references" data-urls="../CompilationUnits.sdf3/#java/packages/ImportDeclarations line 7_3; ../Main.sdf3/#java/packages/ImportDeclarations line 7_3">java/packages/ImportDeclarations</button>

<span class="layout">// 7.5. Import Declarations</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>

<span class="keyword">context-free sorts</span>

  <a href="../CompilationUnits.sdf3/#ImportDeclaration_20_5" id="ImportDeclaration_11_3" title="a definition with a single reference">ImportDeclaration</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../CompilationUnits.sdf3/#ImportDeclaration_20_5" id="ImportDeclaration_15_3" title="a definition with a single reference">ImportDeclaration</a>.<span class="cons_Constructor"><span id="SingleTypeImport_15_21" title="a definition with no references">SingleTypeImport</span></span>     = &lt;<span class="cons_String">import</span> &lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_15_53" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">;</span>&gt;
  <a href="../CompilationUnits.sdf3/#ImportDeclaration_20_5" id="ImportDeclaration_16_3" title="a definition with a single reference">ImportDeclaration</a>.<span class="cons_Constructor"><span id="TypeImportOnDemand_16_21" title="a definition with no references">TypeImportOnDemand</span></span>   = &lt;<span class="cons_String">import</span> &lt;<a href="../../names/Names.sdf3/#PackageOrTypeName_12_3" id="PackageOrTypeName_16_53" title="a reference to a single-file definition">PackageOrTypeName</a>&gt;<span class="cons_String">.*;</span>&gt;
  <a href="../CompilationUnits.sdf3/#ImportDeclaration_20_5" id="ImportDeclaration_17_3" title="a definition with a single reference">ImportDeclaration</a>.<span class="cons_Constructor"><span id="SingleStaticImport_17_21" title="a definition with no references">SingleStaticImport</span></span>   = &lt;<span class="cons_String">import</span> <span class="cons_String">static</span> &lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_17_60" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">.</span>&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_17_71" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">;</span>&gt;
  <a href="../CompilationUnits.sdf3/#ImportDeclaration_20_5" id="ImportDeclaration_18_3" title="a definition with a single reference">ImportDeclaration</a>.<span class="cons_Constructor"><span id="StaticImportOnDemand_18_21" title="a definition with no references">StaticImportOnDemand</span></span> = &lt;<span class="cons_String">import</span> <span class="cons_String">static</span> &lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_18_60" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">.*;</span>&gt;  

<span class="keyword">template options</span>
  <span class="keyword">tokenize</span> : ".;" 
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
