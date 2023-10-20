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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/literals/IntegerLiterals_56_85" id="java/literals/IntegerLiterals_7_36" title="Referenced at ../Main.sdf3 line 6">java/literals/IntegerLiterals</a>

<span class="layout">// 3.10.1. Integer Literals</span>

<span class="keyword">context-free start-symbols</span>
  
  <a href="#IntLiteral_135_145" id="IntLiteral_99_109" title="Defined at line 11, 15, 16, 17, 18">IntLiteral</a>

<span class="keyword">context-free sorts</span>
  
  <a href="#IntLiteral_99_109" id="IntLiteral_135_145" title="Referenced at line 7; ../Main.sdf3 line 19">IntLiteral</a>

<span class="keyword">context-free syntax</span>

  <a href="#IntLiteral_99_109" id="IntLiteral_170_180" title="Referenced at line 7; ../Main.sdf3 line 19">IntLiteral</a>.<span class="cons_Constructor"><span id="Deci_181_185" title="Not referenced locally, nor via imports">Deci</span></span> = <a href="#DeciLiteral_352_363" id="DeciLiteral_188_199" title="Defined at line 22, 29">DeciLiteral</a> {<span class="keyword">prefer</span>}
  <a href="#IntLiteral_99_109" id="IntLiteral_211_221" title="Referenced at line 7; ../Main.sdf3 line 19">IntLiteral</a>.<span class="cons_Constructor"><span id="Hexa_222_226" title="Not referenced locally, nor via imports">Hexa</span></span> = <a href="#HexaLiteral_366_377" id="HexaLiteral_229_240" title="Defined at line 23, 30">HexaLiteral</a> {<span class="keyword">prefer</span>}
  <a href="#IntLiteral_99_109" id="IntLiteral_252_262" title="Referenced at line 7; ../Main.sdf3 line 19">IntLiteral</a>.<span class="cons_Constructor"><span id="Octa_263_267" title="Not referenced locally, nor via imports">Octa</span></span> = <a href="#OctaLiteral_380_391" id="OctaLiteral_270_281" title="Defined at line 24, 31">OctaLiteral</a> {<span class="keyword">prefer</span>}
  <a href="#IntLiteral_99_109" id="IntLiteral_293_303" title="Referenced at line 7; ../Main.sdf3 line 19">IntLiteral</a>.<span class="cons_Constructor"><span id="Bin_304_307" title="Not referenced locally, nor via imports">Bin</span></span>  = <a href="#BinLiteral_394_404" id="BinLiteral_311_321" title="Defined at line 25, 32">BinLiteral</a>  {<span class="keyword">prefer</span>}
  
<span class="keyword">lexical sorts</span>

  <a href="#DeciLiteral_188_199" id="DeciLiteral_352_363" title="Referenced at line 15, 48">DeciLiteral</a>
  <a href="#HexaLiteral_229_240" id="HexaLiteral_366_377" title="Referenced at line 16, 49">HexaLiteral</a>
  <a href="#OctaLiteral_270_281" id="OctaLiteral_380_391" title="Referenced at line 17, 50">OctaLiteral</a>
  <a href="#BinLiteral_311_321" id="BinLiteral_394_404" title="Referenced at line 18, 51">BinLiteral</a>

<span class="keyword">lexical syntax</span>

  <a href="#DeciLiteral_188_199" id="DeciLiteral_424_435" title="Referenced at line 15, 48">DeciLiteral</a> = <a href="#DeciNumeral_560_571" id="DeciNumeral_438_449" title="Defined at line 33, 34, 35">DeciNumeral</a> [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <a href="#HexaLiteral_229_240" id="HexaLiteral_458_469" title="Referenced at line 16, 49">HexaLiteral</a> = <a href="#HexaNumeral_639_650" id="HexaNumeral_472_483" title="Defined at line 36">HexaNumeral</a> [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <a href="#OctaLiteral_270_281" id="OctaLiteral_492_503" title="Referenced at line 17, 50">OctaLiteral</a> = <a href="#OctaNumeral_691_702" id="OctaNumeral_506_517" title="Defined at line 37">OctaNumeral</a> [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <a href="#BinLiteral_311_321" id="BinLiteral_526_536" title="Referenced at line 18, 51">BinLiteral</a>  = <a href="#BinNumeral_726_736" id="BinNumeral_540_550" title="Defined at line 38">BinNumeral</a>  [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]?
  <a href="#DeciNumeral_438_449" id="DeciNumeral_560_571" title="Referenced at line 29, 44">DeciNumeral</a> = <span class="cons_Lit">"0"</span>
  <a href="#DeciNumeral_438_449" id="DeciNumeral_580_591" title="Referenced at line 29, 44">DeciNumeral</a> = [<span class="cons_Regular">1</span>-<span class="cons_Regular">9</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]
  <a href="#DeciNumeral_438_449" id="DeciNumeral_617_628" title="Referenced at line 29, 44">DeciNumeral</a> = [<span class="cons_Regular">1</span>-<span class="cons_Regular">9</span>]
  <a href="#HexaNumeral_472_483" id="HexaNumeral_639_650" title="Referenced at line 30, 45">HexaNumeral</a> = [<span class="cons_Regular">0</span>] [<span class="cons_Regular">x</span><span class="cons_Regular">X</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
  <a href="#OctaNumeral_506_517" id="OctaNumeral_691_702" title="Referenced at line 31, 46">OctaNumeral</a> = [<span class="cons_Regular">0</span>] [\_<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#BinNumeral_540_550" id="BinNumeral_726_736" title="Referenced at line 32, 47">BinNumeral</a>  = <span class="cons_Lit">"0"</span> [<span class="cons_Regular">b</span><span class="cons_Regular">B</span>] <a href="#BinDigits_761_770" id="BinDigits_749_758" title="Defined at line 39, 40">BinDigits</a>
  <a href="#BinDigits_749_758" id="BinDigits_761_770" title="Referenced at line 38">BinDigits</a>   = [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>]
  <a href="#BinDigits_749_758" id="BinDigits_782_791" title="Referenced at line 38">BinDigits</a>   = [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>] [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>\_]* [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>]

<span class="keyword">lexical restrictions</span>

  <a href="#DeciNumeral_560_571" id="DeciNumeral_839_850" title="Defined at line 33, 34, 35">DeciNumeral</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\.<span class="cons_Regular">f</span><span class="cons_Regular">F</span><span class="cons_Regular">d</span><span class="cons_Regular">D</span>]
  <a href="#HexaNumeral_639_650" id="HexaNumeral_869_880" title="Defined at line 36">HexaNumeral</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
  <a href="#OctaNumeral_691_702" id="OctaNumeral_899_910" title="Defined at line 37">OctaNumeral</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">7</span>]
  <a href="#BinNumeral_726_736" id="BinNumeral_923_933" title="Defined at line 38">BinNumeral</a>  -/- [<span class="cons_Regular">0</span><span class="cons_Regular">1</span>]
  <a href="#DeciLiteral_352_363" id="DeciLiteral_946_957" title="Defined at line 22, 29">DeciLiteral</a> -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]
  <a href="#HexaLiteral_366_377" id="HexaLiteral_969_980" title="Defined at line 23, 30">HexaLiteral</a> -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]
  <a href="#OctaLiteral_380_391" id="OctaLiteral_992_1003" title="Defined at line 24, 31">OctaLiteral</a> -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]
  <a href="#BinLiteral_394_404" id="BinLiteral_1015_1025" title="Defined at line 25, 32">BinLiteral</a>  -/- [<span class="cons_Regular">l</span><span class="cons_Regular">L</span>]  
</code></pre></td></tr></tbody></table></div>