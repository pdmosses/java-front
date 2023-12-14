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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/literals/EscapeSequences_1_8" title="Multi-file references" data-urls="../CharacterLiterals.sdf3/#java/literals/EscapeSequences_6_3 line 6; ../StringLiterals.sdf3/#java/literals/EscapeSequences_6_3 line 6">java/literals/EscapeSequences</button>

<span class="layout">// 3.10.6. Escape Sequences for Character and String Literals</span>

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="EscapeSeq_7_3" title="Multi-file references" data-urls="../CharacterLiterals.sdf3/#EscapeSeq_28_21 line 28; ../StringLiterals.sdf3/#EscapeSeq_29_16 line 29">EscapeSeq</button>.<span class="cons_Constructor"><span id="NamedEscape_7_13" title="Not referenced">NamedEscape</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">b</span><span class="cons_Regular">t</span><span class="cons_Regular">n</span><span class="cons_Regular">f</span><span class="cons_Regular">r</span>\"\'\\]
  <button class="modal-open" id="EscapeSeq_8_3" title="Multi-file references" data-urls="../CharacterLiterals.sdf3/#EscapeSeq_28_21 line 28; ../StringLiterals.sdf3/#EscapeSeq_29_16 line 29">EscapeSeq</button> = <a href="#OctalEscape_9_3" id="OctalEscape_8_15" title="Defined at line 9, 10, 11, 12">OctalEscape</a>
  <a href="#OctalEscape_8_15" id="OctalEscape_9_3" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape1_9_15" title="Not referenced">OctalEscape1</span></span> = <span class="cons_Lit">"\\"</span> <a href="#LastOcta_13_3" id="LastOcta_9_35" title="Defined at line 13">LastOcta</a>
  <a href="#OctalEscape_8_15" id="OctalEscape_10_3" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape2_10_15" title="Not referenced">OctalEscape2</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">3</span>] <a href="#LastOcta_13_3" id="LastOcta_10_41" title="Defined at line 13">LastOcta</a>
  <a href="#OctalEscape_8_15" id="OctalEscape_11_3" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape2_11_15" title="Not referenced">OctalEscape2</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">4</span>-<span class="cons_Regular">7</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#OctalEscape_8_15" id="OctalEscape_12_3" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape3_12_15" title="Not referenced">OctalEscape3</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">3</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#LastOcta_9_35" id="LastOcta_13_3" title="Referenced at line 9, 10, 17">LastOcta</a> = [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]

<span class="keyword">lexical restrictions</span>

  <a href="#LastOcta_13_3" id="LastOcta_17_3" title="Defined at line 13">LastOcta</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
