---
title: StringLiterals.sdf3
hide:
  - toc
---

# `StringLiterals.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/literals/StringLiterals.sdf3]

[pdmosses/java-front/lang.java/syntax/java/literals/StringLiterals.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/literals/StringLiterals.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/literals/StringLiterals_10_3" id="java/literals/StringLiterals_1_8" title="a definition with a single reference">java/literals/StringLiterals</a>

<span class="layout">// 3.10.5. String Literals</span>

<span class="keyword">imports</span>
  <a href="../EscapeSequences.sdf3/#java/literals/EscapeSequences_1_8" id="java/literals/EscapeSequences_6_3" title="a reference to a single-file definition">java/literals/EscapeSequences</a>
  <a href="../../lexical/UnicodeEscapes.sdf3/#java/lexical/UnicodeEscapes_1_8" id="java/lexical/UnicodeEscapes_7_3" title="a reference to a single-file definition">java/lexical/UnicodeEscapes</a>

<span class="keyword">context-free start-symbols</span>

  <a href="#StringLiteral_15_3" id="StringLiteral_11_3" title="a reference to a single-file definition">StringLiteral</a>
  
<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="StringLiteral_15_3" title="a definition with multiple references" data-urls="#StringLiteral line 11_3; ../Main.sdf3/#StringLiteral line 23_13">StringLiteral</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="StringLiteral_19_3" title="a definition with multiple references" data-urls="#StringLiteral line 11_3; ../Main.sdf3/#StringLiteral line 23_13">StringLiteral</button>.<span class="cons_Constructor"><span id="StringLiteral_19_17" title="a definition with no references">StringLiteral</span></span> = <a href="#StringLit_23_3" id="StringLit_19_33" title="a reference to a single-file definition">StringLit</a>  
  
<span class="keyword">lexical sorts</span>

  <a href="#StringLit_19_33" id="StringLit_23_3" title="a definition with a single reference">StringLit</a>

<span class="keyword">lexical syntax</span>

  <a href="#StringLit_19_33" id="StringLit_27_3" title="a definition with a single reference">StringLit</a> = <span class="cons_Lit">"\""</span> <a href="#StringPart_28_3" id="StringPart_27_20" title="a reference to a single-file definition">StringPart</a>* <span class="cons_Lit">"\""</span>
  <a href="#StringPart_27_20" id="StringPart_28_3" title="a definition with a single reference">StringPart</a> = <a href="../../lexical/UnicodeEscapes.sdf3/#UnicodeEscape_7_3" id="UnicodeEscape_28_16" title="a reference to a single-file definition">UnicodeEscape</a>
  <a href="#StringPart_27_20" id="StringPart_29_3" title="a definition with a single reference">StringPart</a> = <a href="../EscapeSequences.sdf3/#EscapeSeq_7_3" id="EscapeSeq_29_16" title="a reference to a single-file definition">EscapeSeq</a>
  <a href="#StringPart_27_20" id="StringPart_30_3" title="a definition with a single reference">StringPart</a> = <a href="#StringChars_31_3" id="StringChars_30_16" title="a reference to a single-file definition">StringChars</a>
  <button class="modal-open" id="StringChars_31_3" title="a definition with multiple references" data-urls="#StringChars line 30_16, 35_3">StringChars</button> = ~[\"\\\n\r]+

<span class="keyword">lexical restrictions</span>

  <a href="#StringChars_31_3" id="StringChars_35_3" title="a reference to a single-file definition">StringChars</a> -/- ~[\"\\\n\r]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
