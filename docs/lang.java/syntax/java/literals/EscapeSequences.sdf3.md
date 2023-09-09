---
title: EscapeSequences.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../StringLiterals.sdf3#java/literals/EscapeSequences_75_104" id="java/literals/EscapeSequences_7_36" title="Referenced at ../StringLiterals.sdf3 line 6">java/literals/EscapeSequences</a>

<span class="layout">// 3.10.6. Escape Sequences for Character and String Literals</span>

<span class="keyword">lexical syntax</span>

  <a href="../CharacterLiterals.sdf3#EscapeSeq_419_428" id="EscapeSeq_119_128" title="Referenced at ../CharacterLiterals.sdf3 line 28; ../StringLiterals.sdf3 line 29">EscapeSeq</a>.<span class="cons_Constructor"><span id="NamedEscape_129_140" title="Not referenced locally, nor via imports">NamedEscape</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">b</span><span class="cons_Regular">t</span><span class="cons_Regular">n</span><span class="cons_Regular">f</span><span class="cons_Regular">r</span>\"\'\\]
  <a href="../CharacterLiterals.sdf3#EscapeSeq_419_428" id="EscapeSeq_164_173" title="Referenced at ../CharacterLiterals.sdf3 line 28; ../StringLiterals.sdf3 line 29">EscapeSeq</a> = <a href="#OctalEscape_190_201" id="OctalEscape_176_187" title="Defined at line 9, 10, 11, 12">OctalEscape</a>
  <a href="#OctalEscape_176_187" id="OctalEscape_190_201" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape1_202_214" title="Not referenced locally, nor via imports">OctalEscape1</span></span> = <span class="cons_Lit">"\\"</span> <a href="#LastOcta_380_388" id="LastOcta_222_230" title="Defined at line 13">LastOcta</a>
  <a href="#OctalEscape_176_187" id="OctalEscape_233_244" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape2_245_257" title="Not referenced locally, nor via imports">OctalEscape2</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">3</span>] <a href="#LastOcta_380_388" id="LastOcta_271_279" title="Defined at line 13">LastOcta</a>
  <a href="#OctalEscape_176_187" id="OctalEscape_282_293" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape2_294_306" title="Not referenced locally, nor via imports">OctalEscape2</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">4</span>-<span class="cons_Regular">7</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#OctalEscape_176_187" id="OctalEscape_328_339" title="Referenced at line 8">OctalEscape</a>.<span class="cons_Constructor"><span id="OctalEscape3_340_352" title="Not referenced locally, nor via imports">OctalEscape3</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">3</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#LastOcta_422_430" id="LastOcta_380_388" title="Referenced at line 17">LastOcta</a> = [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]

<span class="keyword">lexical restrictions</span>

  <a href="#LastOcta_380_388" id="LastOcta_422_430" title="Defined at line 13">LastOcta</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
</code></pre></td></tr></tbody></table></div>