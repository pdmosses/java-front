---
title: EscapeSequences.sdf3
hide:
  - toc
---

# `EscapeSequences.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/literals/EscapeSequences.sdf3]

[pdmosses/java-front/lang.java/syntax/java/literals/EscapeSequences.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/literals/EscapeSequences.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/literals/EscapeSequences_1_8" title="a definition with multiple references" data-urls="../CharacterLiterals.sdf3/#java/literals/EscapeSequences line 6_3; ../StringLiterals.sdf3/#java/literals/EscapeSequences line 6_3">java/literals/EscapeSequences</button>

<span class="layout">// 3.10.6. Escape Sequences for Character and String Literals</span>

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="EscapeSeq_7_3" title="a definition with multiple references" data-urls="../CharacterLiterals.sdf3/#EscapeSeq line 28_21; ../StringLiterals.sdf3/#EscapeSeq line 29_16">EscapeSeq</button>.<span class="cons_Constructor"><span id="NamedEscape_7_13" title="a definition with no references">NamedEscape</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">b</span><span class="cons_Regular">t</span><span class="cons_Regular">n</span><span class="cons_Regular">f</span><span class="cons_Regular">r</span>\"\'\\]
  <button class="modal-open" id="EscapeSeq_8_3" title="a definition with multiple references" data-urls="../CharacterLiterals.sdf3/#EscapeSeq line 28_21; ../StringLiterals.sdf3/#EscapeSeq line 29_16">EscapeSeq</button> = <a href="#OctalEscape_9_3" id="OctalEscape_8_15" title="a reference to a single-file definition">OctalEscape</a>
  <a href="#OctalEscape_8_15" id="OctalEscape_9_3" title="a definition with a single reference">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape1_9_15" title="a definition with no references">OctalEscape1</span></span> = <span class="cons_Lit">"\\"</span> <a href="#LastOcta_13_3" id="LastOcta_9_35" title="a reference to a single-file definition">LastOcta</a>
  <a href="#OctalEscape_8_15" id="OctalEscape_10_3" title="a definition with a single reference">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape2_10_15" title="a definition with no references">OctalEscape2</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">3</span>] <a href="#LastOcta_13_3" id="LastOcta_10_41" title="a reference to a single-file definition">LastOcta</a>
  <a href="#OctalEscape_8_15" id="OctalEscape_11_3" title="a definition with a single reference">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape2_11_15" title="a definition with no references">OctalEscape2</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">4</span>-<span class="cons_Regular">7</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#OctalEscape_8_15" id="OctalEscape_12_3" title="a definition with a single reference">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape3_12_15" title="a definition with no references">OctalEscape3</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">3</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <button class="modal-open" id="LastOcta_13_3" title="a definition with multiple references" data-urls="#LastOcta line 9_35, 10_41, 17_3">LastOcta</button> = [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]

<span class="keyword">lexical restrictions</span>

  <a href="#LastOcta_13_3" id="LastOcta_17_3" title="a reference to a single-file definition">LastOcta</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
