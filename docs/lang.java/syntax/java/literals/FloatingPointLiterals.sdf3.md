---
title: FloatingPointLiterals.sdf3
hide:
  - toc
---

# `FloatingPointLiterals.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/literals/FloatingPointLiterals.sdf3]

[pdmosses/java-front/lang.java/syntax/java/literals/FloatingPointLiterals.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/literals/FloatingPointLiterals.sdf3 "The source file on GitHub"

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
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/literals/FloatingPointLiterals_7_3" id="java/literals/FloatingPointLiterals_1_8" title="a definition with a single reference">java/literals/FloatingPointLiterals</a>

<span class="layout">// 3.10.2. Floating-Point Literals</span>

<span class="keyword">context-free start-symbols</span>
  
  <a href="#FloatLiteral_11_3" id="FloatLiteral_7_3" title="a reference to a single-file definition">FloatLiteral</a>

<span class="keyword">context-free sorts</span>
  
  <button class="modal-open" id="FloatLiteral_11_3" title="a definition with multiple references" data-urls="#FloatLiteral line 7_3; ../Main.sdf3/#FloatLiteral line 20_13">FloatLiteral</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="FloatLiteral_15_3" title="a definition with multiple references" data-urls="#FloatLiteral line 7_3; ../Main.sdf3/#FloatLiteral line 20_13">FloatLiteral</button>.<span class="cons_Constructor"><span id="DeciFloat_15_16" title="a definition with no references">DeciFloat</span></span> = <a href="#DeciFloatLiteral_22_3" id="DeciFloatLiteral_15_28" title="a reference to a single-file definition">DeciFloatLiteral</a>
  <button class="modal-open" id="FloatLiteral_16_3" title="a definition with multiple references" data-urls="#FloatLiteral line 7_3; ../Main.sdf3/#FloatLiteral line 20_13">FloatLiteral</button>.<span class="cons_Constructor"><span id="HexaFloat_16_16" title="a definition with no references">HexaFloat</span></span> = <a href="#HexaFloatLiteral_23_3" id="HexaFloatLiteral_16_28" title="a reference to a single-file definition">HexaFloatLiteral</a>
  <button class="modal-open" id="FloatLiteral_17_3" title="a definition with multiple references" data-urls="#FloatLiteral line 7_3; ../Main.sdf3/#FloatLiteral line 20_13">FloatLiteral</button>.<span class="cons_Constructor"><span id="DeciDouble_17_16" title="a definition with no references">DeciDouble</span></span> = <a href="#DeciDoubleLiteral_24_3" id="DeciDoubleLiteral_17_29" title="a reference to a single-file definition">DeciDoubleLiteral</a>
  <button class="modal-open" id="FloatLiteral_18_3" title="a definition with multiple references" data-urls="#FloatLiteral line 7_3; ../Main.sdf3/#FloatLiteral line 20_13">FloatLiteral</button>.<span class="cons_Constructor"><span id="HexaDouble_18_16" title="a definition with no references">HexaDouble</span></span> = <a href="#HexaDoubleLiteral_25_3" id="HexaDoubleLiteral_18_29" title="a reference to a single-file definition">HexaDoubleLiteral</a>

<span class="keyword">lexical sorts</span>

  <button class="modal-open" id="DeciFloatLiteral_22_3" title="a definition with multiple references" data-urls="#DeciFloatLiteral line 15_28, 53_3">DeciFloatLiteral</button>
  <a href="#HexaFloatLiteral_16_28" id="HexaFloatLiteral_23_3" title="a definition with a single reference">HexaFloatLiteral</a>
  <button class="modal-open" id="DeciDoubleLiteral_24_3" title="a definition with multiple references" data-urls="#DeciDoubleLiteral line 17_29, 54_3">DeciDoubleLiteral</button>
  <a href="#HexaDoubleLiteral_18_29" id="HexaDoubleLiteral_25_3" title="a definition with a single reference">HexaDoubleLiteral</a>

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="DeciFloatLiteral_29_3" title="a definition with multiple references" data-urls="#DeciFloatLiteral line 15_28, 53_3">DeciFloatLiteral</button> = <a href="#Digits_42_3" id="Digits_29_22" title="a reference to a single-file definition">Digits</a> <span class="cons_Lit">"."</span> <a href="#Digits_42_3" id="Digits_29_33" title="a reference to a single-file definition">Digits</a>? <a href="#DeciFloatExponentPart_39_3" id="DeciFloatExponentPart_29_41" title="a reference to a single-file definition">DeciFloatExponentPart</a>? [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <button class="modal-open" id="DeciFloatLiteral_30_3" title="a definition with multiple references" data-urls="#DeciFloatLiteral line 15_28, 53_3">DeciFloatLiteral</button> = <span class="cons_Lit">"."</span> <a href="#Digits_42_3" id="Digits_30_26" title="a reference to a single-file definition">Digits</a> <a href="#DeciFloatExponentPart_39_3" id="DeciFloatExponentPart_30_33" title="a reference to a single-file definition">DeciFloatExponentPart</a>? [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <button class="modal-open" id="DeciFloatLiteral_31_3" title="a definition with multiple references" data-urls="#DeciFloatLiteral line 15_28, 53_3">DeciFloatLiteral</button> = <a href="#Digits_42_3" id="Digits_31_22" title="a reference to a single-file definition">Digits</a> <a href="#DeciFloatExponentPart_39_3" id="DeciFloatExponentPart_31_29" title="a reference to a single-file definition">DeciFloatExponentPart</a> [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <button class="modal-open" id="DeciFloatLiteral_32_3" title="a definition with multiple references" data-urls="#DeciFloatLiteral line 15_28, 53_3">DeciFloatLiteral</button> = <a href="#Digits_42_3" id="Digits_32_22" title="a reference to a single-file definition">Digits</a> [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  
  <button class="modal-open" id="DeciDoubleLiteral_34_3" title="a definition with multiple references" data-urls="#DeciDoubleLiteral line 17_29, 54_3">DeciDoubleLiteral</button> = <a href="#Digits_42_3" id="Digits_34_23" title="a reference to a single-file definition">Digits</a> <span class="cons_Lit">"."</span> <a href="#Digits_42_3" id="Digits_34_34" title="a reference to a single-file definition">Digits</a>? <a href="#DeciFloatExponentPart_39_3" id="DeciFloatExponentPart_34_42" title="a reference to a single-file definition">DeciFloatExponentPart</a>? [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <button class="modal-open" id="DeciDoubleLiteral_35_3" title="a definition with multiple references" data-urls="#DeciDoubleLiteral line 17_29, 54_3">DeciDoubleLiteral</button> = <span class="cons_Lit">"."</span> <a href="#Digits_42_3" id="Digits_35_27" title="a reference to a single-file definition">Digits</a> <a href="#DeciFloatExponentPart_39_3" id="DeciFloatExponentPart_35_34" title="a reference to a single-file definition">DeciFloatExponentPart</a>? [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <button class="modal-open" id="DeciDoubleLiteral_36_3" title="a definition with multiple references" data-urls="#DeciDoubleLiteral line 17_29, 54_3">DeciDoubleLiteral</button> = <a href="#Digits_42_3" id="Digits_36_23" title="a reference to a single-file definition">Digits</a> <a href="#DeciFloatExponentPart_39_3" id="DeciFloatExponentPart_36_30" title="a reference to a single-file definition">DeciFloatExponentPart</a> [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <button class="modal-open" id="DeciDoubleLiteral_37_3" title="a definition with multiple references" data-urls="#DeciDoubleLiteral line 17_29, 54_3">DeciDoubleLiteral</button> = <a href="#Digits_42_3" id="Digits_37_23" title="a reference to a single-file definition">Digits</a> [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]
 
  <button class="modal-open" id="DeciFloatExponentPart_39_3" title="a definition with multiple references" data-urls="#DeciFloatExponentPart line 29_41, 30_33, 31_29, 34_42, 35_34, 36_30">DeciFloatExponentPart</button> = [<span class="cons_Regular">e</span><span class="cons_Regular">E</span>] <a href="#SignedInteger_40_3" id="SignedInteger_39_32" title="a reference to a single-file definition">SignedInteger</a>
  <button class="modal-open" id="SignedInteger_40_3" title="a definition with multiple references" data-urls="#SignedInteger line 39_32, 55_3, 63_25">SignedInteger</button> = [\+\-]? <a href="#Digits_42_3" id="Digits_40_27" title="a reference to a single-file definition">Digits</a>
  
  <button class="modal-open" id="Digits_42_3" title="a definition with multiple references" data-urls="#Digits line 29_22, 29_33, 30_26, 31_22, 32_22, 34_23, 34_34, 35_27, 36_23, 37_23, 40_27">Digits</button> = <a href="#Digit_44_3" id="Digit_42_12" title="a reference to a single-file definition">Digit</a>
  <button class="modal-open" id="Digits_43_3" title="a definition with multiple references" data-urls="#Digits line 29_22, 29_33, 30_26, 31_22, 32_22, 34_23, 34_34, 35_27, 36_23, 37_23, 40_27">Digits</button> = <a href="#Digit_44_3" id="Digit_43_12" title="a reference to a single-file definition">Digit</a> <a href="#DigitsAndUnderscores_46_3" id="DigitsAndUnderscores_43_18" title="a reference to a single-file definition">DigitsAndUnderscores</a>? <a href="#Digit_44_3" id="Digit_43_40" title="a reference to a single-file definition">Digit</a>
  <button class="modal-open" id="Digit_44_3" title="a definition with multiple references" data-urls="#Digit line 42_12, 43_12, 43_40, 47_25">Digit</button> = [<span class="cons_Regular">0</span>]
  <button class="modal-open" id="Digit_45_3" title="a definition with multiple references" data-urls="#Digit line 42_12, 43_12, 43_40, 47_25">Digit</button> = [<span class="cons_Regular">1</span>-<span class="cons_Regular">9</span>]
  <a href="#DigitsAndUnderscores_43_18" id="DigitsAndUnderscores_46_3" title="a definition with a single reference">DigitsAndUnderscores</a> = <a href="#DigitsOrUnderscore_47_3" id="DigitsOrUnderscore_46_26" title="a reference to a single-file definition">DigitsOrUnderscore</a>+
  <a href="#DigitsOrUnderscore_46_26" id="DigitsOrUnderscore_47_3" title="a definition with a single reference">DigitsOrUnderscore</a> = (<a href="#Digit_44_3" id="Digit_47_25" title="a reference to a single-file definition">Digit</a> | [\_])
  <span id="Underscores_48_3" title="a definition with no references">Underscores</span> = [\_]+


<span class="keyword">lexical restrictions</span>

  <a href="#DeciFloatLiteral_22_3" id="DeciFloatLiteral_53_3" title="a reference to a single-file definition">DeciFloatLiteral</a> -/- [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#DeciDoubleLiteral_24_3" id="DeciDoubleLiteral_54_3" title="a reference to a single-file definition">DeciDoubleLiteral</a> -/- [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]
  <a href="#SignedInteger_40_3" id="SignedInteger_55_3" title="a reference to a single-file definition">SignedInteger</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]

<span class="keyword">lexical syntax</span>

  <a href="#HexaFloatLiteral_16_28" id="HexaFloatLiteral_59_3" title="a definition with a single reference">HexaFloatLiteral</a> = <a href="#HexaSignificand_61_3" id="HexaSignificand_59_22" title="a reference to a single-file definition">HexaSignificand</a> <a href="#BinaryExponent_63_3" id="BinaryExponent_59_38" title="a reference to a single-file definition">BinaryExponent</a> [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#HexaDoubleLiteral_18_29" id="HexaDoubleLiteral_60_3" title="a definition with a single reference">HexaDoubleLiteral</a> = <a href="#HexaSignificand_61_3" id="HexaSignificand_60_23" title="a reference to a single-file definition">HexaSignificand</a> <a href="#BinaryExponent_63_3" id="BinaryExponent_60_39" title="a reference to a single-file definition">BinaryExponent</a> [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <button class="modal-open" id="HexaSignificand_61_3" title="a definition with multiple references" data-urls="#HexaSignificand line 59_22, 60_23, 67_3">HexaSignificand</button> = [<span class="cons_Regular">0</span>] [<span class="cons_Regular">x</span><span class="cons_Regular">X</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] <span class="cons_Lit">"."</span>?  
  <button class="modal-open" id="HexaSignificand_62_3" title="a definition with multiple references" data-urls="#HexaSignificand line 59_22, 60_23, 67_3">HexaSignificand</button> = [<span class="cons_Regular">0</span>] [<span class="cons_Regular">x</span><span class="cons_Regular">X</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] <span class="cons_Lit">"."</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
  <button class="modal-open" id="BinaryExponent_63_3" title="a definition with multiple references" data-urls="#BinaryExponent line 59_38, 60_39">BinaryExponent</button> = [<span class="cons_Regular">p</span><span class="cons_Regular">P</span>] <a href="#SignedInteger_40_3" id="SignedInteger_63_25" title="a reference to a single-file definition">SignedInteger</a>

<span class="keyword">lexical restrictions</span>

  <a href="#HexaSignificand_61_3" id="HexaSignificand_67_3" title="a reference to a single-file definition">HexaSignificand</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\.]

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
