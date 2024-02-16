---
title: IntegerLiterals.sdf3
hide:
  - toc
---

# `IntegerLiterals.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/literals/IntegerLiterals.sdf3]

[pdmosses/java-front/lang.java/syntax/java/literals/IntegerLiterals.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/literals/IntegerLiterals.sdf3 "The source file on GitHub"

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
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/literals/IntegerLiterals_6_3" id="java/literals/IntegerLiterals_1_8" title="a definition with a single reference">java/literals/IntegerLiterals</a>

<span class="layout">// 3.10.1. Integer Literals</span>

<span class="keyword">context-free start-symbols</span>
  
  <a href="#IntLiteral_11_3" id="IntLiteral_7_3" title="a reference to a single-file definition">IntLiteral</a>

<span class="keyword">context-free sorts</span>
  
  <button class="modal-open" id="IntLiteral_11_3" title="a definition with multiple references" data-urls="#IntLiteral line 7_3; ../Main.sdf3/#IntLiteral line 19_13">IntLiteral</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="IntLiteral_15_3" title="a definition with multiple references" data-urls="#IntLiteral line 7_3; ../Main.sdf3/#IntLiteral line 19_13">IntLiteral</button>.<span class="cons_Constructor"><span id="Deci_15_14" title="a definition with no references">Deci</span></span> = <a href="#DeciLiteral_22_3" id="DeciLiteral_15_21" title="a reference to a single-file definition">DeciLiteral</a> {<span class="keyword">prefer</span>}
  <button class="modal-open" id="IntLiteral_16_3" title="a definition with multiple references" data-urls="#IntLiteral line 7_3; ../Main.sdf3/#IntLiteral line 19_13">IntLiteral</button>.<span class="cons_Constructor"><span id="Hexa_16_14" title="a definition with no references">Hexa</span></span> = <a href="#HexaLiteral_23_3" id="HexaLiteral_16_21" title="a reference to a single-file definition">HexaLiteral</a> {<span class="keyword">prefer</span>}
  <button class="modal-open" id="IntLiteral_17_3" title="a definition with multiple references" data-urls="#IntLiteral line 7_3; ../Main.sdf3/#IntLiteral line 19_13">IntLiteral</button>.<span class="cons_Constructor"><span id="Octa_17_14" title="a definition with no references">Octa</span></span> = <a href="#OctaLiteral_24_3" id="OctaLiteral_17_21" title="a reference to a single-file definition">OctaLiteral</a> {<span class="keyword">prefer</span>}
  <button class="modal-open" id="IntLiteral_18_3" title="a definition with multiple references" data-urls="#IntLiteral line 7_3; ../Main.sdf3/#IntLiteral line 19_13">IntLiteral</button>.<span class="cons_Constructor"><span id="Bin_18_14" title="a definition with no references">Bin</span></span>  = <a href="#BinLiteral_25_3" id="BinLiteral_18_21" title="a reference to a single-file definition">BinLiteral</a>  {<span class="keyword">prefer</span>}
  
<span class="keyword">lexical sorts</span>

  <button class="modal-open" id="DeciLiteral_22_3" title="a definition with multiple references" data-urls="#DeciLiteral line 15_21, 48_3">DeciLiteral</button>
  <button class="modal-open" id="HexaLiteral_23_3" title="a definition with multiple references" data-urls="#HexaLiteral line 16_21, 49_3">HexaLiteral</button>
  <button class="modal-open" id="OctaLiteral_24_3" title="a definition with multiple references" data-urls="#OctaLiteral line 17_21, 50_3">OctaLiteral</button>
  <button class="modal-open" id="BinLiteral_25_3" title="a definition with multiple references" data-urls="#BinLiteral line 18_21, 51_3">BinLiteral</button>

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="DeciLiteral_29_3" title="a definition with multiple references" data-urls="#DeciLiteral line 15_21, 48_3">DeciLiteral</button> = <a href="#DeciNumeral_33_3" id="DeciNumeral_29_17" title="a reference to a single-file definition">DeciNumeral</a> [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <button class="modal-open" id="HexaLiteral_30_3" title="a definition with multiple references" data-urls="#HexaLiteral line 16_21, 49_3">HexaLiteral</button> = <a href="#HexaNumeral_36_3" id="HexaNumeral_30_17" title="a reference to a single-file definition">HexaNumeral</a> [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <button class="modal-open" id="OctaLiteral_31_3" title="a definition with multiple references" data-urls="#OctaLiteral line 17_21, 50_3">OctaLiteral</button> = <a href="#OctaNumeral_37_3" id="OctaNumeral_31_17" title="a reference to a single-file definition">OctaNumeral</a> [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <button class="modal-open" id="BinLiteral_32_3" title="a definition with multiple references" data-urls="#BinLiteral line 18_21, 51_3">BinLiteral</button>  = <a href="#BinNumeral_38_3" id="BinNumeral_32_17" title="a reference to a single-file definition">BinNumeral</a>  [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <button class="modal-open" id="DeciNumeral_33_3" title="a definition with multiple references" data-urls="#DeciNumeral line 29_17, 44_3">DeciNumeral</button> = <span class="cons_Lit">"0"</span>
  <button class="modal-open" id="DeciNumeral_34_3" title="a definition with multiple references" data-urls="#DeciNumeral line 29_17, 44_3">DeciNumeral</button> = [<span class="cons_Regular">1</span>-<span class="cons_Regular">9</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]
  <button class="modal-open" id="DeciNumeral_35_3" title="a definition with multiple references" data-urls="#DeciNumeral line 29_17, 44_3">DeciNumeral</button> = [<span class="cons_Regular">1</span>-<span class="cons_Regular">9</span>]
  <button class="modal-open" id="HexaNumeral_36_3" title="a definition with multiple references" data-urls="#HexaNumeral line 30_17, 45_3">HexaNumeral</button> = [<span class="cons_Regular">0</span>] [<span class="cons_Regular">x</span><span class="cons_Regular">X</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
  <button class="modal-open" id="OctaNumeral_37_3" title="a definition with multiple references" data-urls="#OctaNumeral line 31_17, 46_3">OctaNumeral</button> = [<span class="cons_Regular">0</span>] [\_<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <button class="modal-open" id="BinNumeral_38_3" title="a definition with multiple references" data-urls="#BinNumeral line 32_17, 47_3">BinNumeral</button>  = <span class="cons_Lit">"0"</span> [<span class="cons_Regular">b</span><span class="cons_Regular">B</span>] <a href="#BinDigits_39_3" id="BinDigits_38_26" title="a reference to a single-file definition">BinDigits</a>
  <a href="#BinDigits_38_26" id="BinDigits_39_3" title="a definition with a single reference">BinDigits</a>   = [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>]
  <a href="#BinDigits_38_26" id="BinDigits_40_3" title="a definition with a single reference">BinDigits</a>   = [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>] [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>\_]* [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>]

<span class="keyword">lexical restrictions</span>

  <a href="#DeciNumeral_33_3" id="DeciNumeral_44_3" title="a reference to a single-file definition">DeciNumeral</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\.<span class="cons_Regular">f</span><span class="cons_Regular">F</span><span class="cons_Regular">d</span><span class="cons_Regular">D</span>]
  <a href="#HexaNumeral_36_3" id="HexaNumeral_45_3" title="a reference to a single-file definition">HexaNumeral</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
  <a href="#OctaNumeral_37_3" id="OctaNumeral_46_3" title="a reference to a single-file definition">OctaNumeral</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#BinNumeral_38_3" id="BinNumeral_47_3" title="a reference to a single-file definition">BinNumeral</a>  -/- [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>]
  <a href="#DeciLiteral_22_3" id="DeciLiteral_48_3" title="a reference to a single-file definition">DeciLiteral</a> -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]
  <a href="#HexaLiteral_23_3" id="HexaLiteral_49_3" title="a reference to a single-file definition">HexaLiteral</a> -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]
  <a href="#OctaLiteral_24_3" id="OctaLiteral_50_3" title="a reference to a single-file definition">OctaLiteral</a> -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]
  <a href="#BinLiteral_25_3" id="BinLiteral_51_3" title="a reference to a single-file definition">BinLiteral</a>  -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
