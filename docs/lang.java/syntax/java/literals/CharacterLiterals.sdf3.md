---
title: CharacterLiterals.sdf3
hide:
  - toc
---

# `CharacterLiterals.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/literals/CharacterLiterals.sdf3]

[pdmosses/java-front/lang.java/syntax/java/literals/CharacterLiterals.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/literals/CharacterLiterals.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/literals/CharacterLiterals_9_3" id="java/literals/CharacterLiterals_1_8" title="a definition with a single reference">java/literals/CharacterLiterals</a>

<span class="layout">// 3.10.4. Character Literals</span>

<span class="keyword">imports</span>
  <a href="../EscapeSequences.sdf3/#java/literals/EscapeSequences_1_8" id="java/literals/EscapeSequences_6_3" title="a reference to a single-file definition">java/literals/EscapeSequences</a>
  <a href="../../lexical/UnicodeEscapes.sdf3/#java/lexical/UnicodeEscapes_1_8" id="java/lexical/UnicodeEscapes_7_3" title="a reference to a single-file definition">java/lexical/UnicodeEscapes</a>
  
<span class="keyword">context-free start-symbols</span>
  
  <a href="#CharacterLiteral_15_3" id="CharacterLiteral_11_3" title="a reference to a single-file definition">CharacterLiteral</a>  
  
<span class="keyword">context-free sorts</span>
  
  <button class="modal-open" id="CharacterLiteral_15_3" title="a definition with multiple references" data-urls="#CharacterLiteral line 11_3; ../Main.sdf3/#CharacterLiteral line 22_13">CharacterLiteral</button>  
  
<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="CharacterLiteral_19_3" title="a definition with multiple references" data-urls="#CharacterLiteral line 11_3; ../Main.sdf3/#CharacterLiteral line 22_13">CharacterLiteral</button>.<span class="cons_Constructor"><span id="CharLiteral_19_20" title="a definition with no references">CharLiteral</span></span> = <a href="#CharLiteral_23_3" id="CharLiteral_19_34" title="a reference to a single-file definition">CharLiteral</a>  
  
<span class="keyword">lexical sorts</span>

  <a href="#CharLiteral_19_34" id="CharLiteral_23_3" title="a definition with a single reference">CharLiteral</a>  

<span class="keyword">lexical syntax</span>

  <a href="#CharLiteral_19_34" id="CharLiteral_27_3" title="a definition with a single reference">CharLiteral</a> = <span class="cons_Lit">"'"</span> ~[\n\r\'\\] <span class="cons_Lit">"'"</span>
  <a href="#CharLiteral_19_34" id="CharLiteral_28_3" title="a definition with a single reference">CharLiteral</a> = <span class="cons_Lit">"'"</span> <a href="../EscapeSequences.sdf3/#EscapeSeq_7_3" id="EscapeSeq_28_21" title="a reference to a single-file definition">EscapeSeq</a> <span class="cons_Lit">"'"</span>
  <a href="#CharLiteral_19_34" id="CharLiteral_29_3" title="a definition with a single reference">CharLiteral</a> = <span class="cons_Lit">"'"</span> <a href="../../lexical/UnicodeEscapes.sdf3/#UnicodeEscape_7_3" id="UnicodeEscape_29_21" title="a reference to a single-file definition">UnicodeEscape</a> <span class="cons_Lit">"'"</span>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
