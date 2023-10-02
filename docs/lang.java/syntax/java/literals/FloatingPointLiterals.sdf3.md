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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/literals/FloatingPointLiterals_88_123" id="java/literals/FloatingPointLiterals_7_42" title="Referenced at ../Main.sdf3 line 7">java/literals/FloatingPointLiterals</a>

<span class="layout">// 3.10.2. Floating-Point Literals</span>

<span class="keyword">context-free start-symbols</span>
  
  <a href="#FloatLiteral_150_162" id="FloatLiteral_112_124" title="Defined at line 11, 15, 16, 17, 18">FloatLiteral</a>

<span class="keyword">context-free sorts</span>
  
  <a href="#FloatLiteral_112_124" id="FloatLiteral_150_162" title="Referenced at line 7; ../Main.sdf3 line 20">FloatLiteral</a>

<span class="keyword">context-free syntax</span>

  <a href="#FloatLiteral_112_124" id="FloatLiteral_187_199" title="Referenced at line 7; ../Main.sdf3 line 20">FloatLiteral</a>.<span class="cons_Constructor"><span id="DeciFloat_200_209" title="Not referenced locally, nor via imports">DeciFloat</span></span> = <a href="#DeciFloatLiteral_383_399" id="DeciFloatLiteral_212_228" title="Defined at line 22, 29, 30, 31, 32">DeciFloatLiteral</a>
  <a href="#FloatLiteral_112_124" id="FloatLiteral_231_243" title="Referenced at line 7; ../Main.sdf3 line 20">FloatLiteral</a>.<span class="cons_Constructor"><span id="HexaFloat_244_253" title="Not referenced locally, nor via imports">HexaFloat</span></span> = <a href="#HexaFloatLiteral_402_418" id="HexaFloatLiteral_256_272" title="Defined at line 23, 59">HexaFloatLiteral</a>
  <a href="#FloatLiteral_112_124" id="FloatLiteral_275_287" title="Referenced at line 7; ../Main.sdf3 line 20">FloatLiteral</a>.<span class="cons_Constructor"><span id="DeciDouble_288_298" title="Not referenced locally, nor via imports">DeciDouble</span></span> = <a href="#DeciDoubleLiteral_421_438" id="DeciDoubleLiteral_301_318" title="Defined at line 24, 34, 35, 36, 37">DeciDoubleLiteral</a>
  <a href="#FloatLiteral_112_124" id="FloatLiteral_321_333" title="Referenced at line 7; ../Main.sdf3 line 20">FloatLiteral</a>.<span class="cons_Constructor"><span id="HexaDouble_334_344" title="Not referenced locally, nor via imports">HexaDouble</span></span> = <a href="#HexaDoubleLiteral_441_458" id="HexaDoubleLiteral_347_364" title="Defined at line 25, 60">HexaDoubleLiteral</a>

<span class="keyword">lexical sorts</span>

  <a href="#DeciFloatLiteral_1224_1240" id="DeciFloatLiteral_383_399" title="Referenced at line 53">DeciFloatLiteral</a>
  <a href="#HexaFloatLiteral_256_272" id="HexaFloatLiteral_402_418" title="Referenced at line 16">HexaFloatLiteral</a>
  <a href="#DeciDoubleLiteral_1252_1269" id="DeciDoubleLiteral_421_438" title="Referenced at line 54">DeciDoubleLiteral</a>
  <a href="#HexaDoubleLiteral_347_364" id="HexaDoubleLiteral_441_458" title="Referenced at line 18">HexaDoubleLiteral</a>

<span class="keyword">lexical syntax</span>

  <a href="#DeciFloatLiteral_1224_1240" id="DeciFloatLiteral_478_494" title="Referenced at line 53">DeciFloatLiteral</a> = <a href="#Digits_1003_1009" id="Digits_497_503" title="Defined at line 42, 43">Digits</a> <span class="cons_Lit">"."</span> <a href="#Digits_1003_1009" id="Digits_508_514" title="Defined at line 42, 43">Digits</a>? <a href="#DeciFloatExponentPart_922_943" id="DeciFloatExponentPart_516_537" title="Defined at line 39">DeciFloatExponentPart</a>? [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#DeciFloatLiteral_1224_1240" id="DeciFloatLiteral_546_562" title="Referenced at line 53">DeciFloatLiteral</a> = <span class="cons_Lit">"."</span> <a href="#Digits_1003_1009" id="Digits_569_575" title="Defined at line 42, 43">Digits</a> <a href="#DeciFloatExponentPart_922_943" id="DeciFloatExponentPart_576_597" title="Defined at line 39">DeciFloatExponentPart</a>? [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#DeciFloatLiteral_1224_1240" id="DeciFloatLiteral_606_622" title="Referenced at line 53">DeciFloatLiteral</a> = <a href="#Digits_1003_1009" id="Digits_625_631" title="Defined at line 42, 43">Digits</a> <a href="#DeciFloatExponentPart_922_943" id="DeciFloatExponentPart_632_653" title="Defined at line 39">DeciFloatExponentPart</a> [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#DeciFloatLiteral_1224_1240" id="DeciFloatLiteral_661_677" title="Referenced at line 53">DeciFloatLiteral</a> = <a href="#Digits_1003_1009" id="Digits_680_686" title="Defined at line 42, 43">Digits</a> [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  
  <a href="#DeciDoubleLiteral_1252_1269" id="DeciDoubleLiteral_697_714" title="Referenced at line 54">DeciDoubleLiteral</a> = <a href="#Digits_1003_1009" id="Digits_717_723" title="Defined at line 42, 43">Digits</a> <span class="cons_Lit">"."</span> <a href="#Digits_1003_1009" id="Digits_728_734" title="Defined at line 42, 43">Digits</a>? <a href="#DeciFloatExponentPart_922_943" id="DeciFloatExponentPart_736_757" title="Defined at line 39">DeciFloatExponentPart</a>? [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <a href="#DeciDoubleLiteral_1252_1269" id="DeciDoubleLiteral_767_784" title="Referenced at line 54">DeciDoubleLiteral</a> = <span class="cons_Lit">"."</span> <a href="#Digits_1003_1009" id="Digits_791_797" title="Defined at line 42, 43">Digits</a> <a href="#DeciFloatExponentPart_922_943" id="DeciFloatExponentPart_798_819" title="Defined at line 39">DeciFloatExponentPart</a>? [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <a href="#DeciDoubleLiteral_1252_1269" id="DeciDoubleLiteral_829_846" title="Referenced at line 54">DeciDoubleLiteral</a> = <a href="#Digits_1003_1009" id="Digits_849_855" title="Defined at line 42, 43">Digits</a> <a href="#DeciFloatExponentPart_922_943" id="DeciFloatExponentPart_856_877" title="Defined at line 39">DeciFloatExponentPart</a> [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <a href="#DeciDoubleLiteral_1252_1269" id="DeciDoubleLiteral_886_903" title="Referenced at line 54">DeciDoubleLiteral</a> = <a href="#Digits_1003_1009" id="Digits_906_912" title="Defined at line 42, 43">Digits</a> [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]
 
  <a href="#DeciFloatExponentPart_856_877" id="DeciFloatExponentPart_922_943" title="Referenced at line 36">DeciFloatExponentPart</a> = [<span class="cons_Regular">e</span><span class="cons_Regular">E</span>] <a href="#SignedInteger_967_980" id="SignedInteger_951_964" title="Defined at line 40">SignedInteger</a>
  <a href="#SignedInteger_1612_1625" id="SignedInteger_967_980" title="Referenced at line 63">SignedInteger</a> = [\+\-]? <a href="#Digits_1003_1009" id="Digits_991_997" title="Defined at line 42, 43">Digits</a>
  
  <a href="#Digits_991_997" id="Digits_1003_1009" title="Referenced at line 40">Digits</a> = <a href="#Digit_1065_1070" id="Digit_1012_1017" title="Defined at line 44, 45">Digit</a>
  <a href="#Digits_991_997" id="Digits_1020_1026" title="Referenced at line 40">Digits</a> = <a href="#Digit_1065_1070" id="Digit_1029_1034" title="Defined at line 44, 45">Digit</a> <a href="#DigitsAndUnderscores_1095_1115" id="DigitsAndUnderscores_1035_1055" title="Defined at line 46">DigitsAndUnderscores</a>? <a href="#Digit_1065_1070" id="Digit_1057_1062" title="Defined at line 44, 45">Digit</a>
  <a href="#Digit_1162_1167" id="Digit_1065_1070" title="Referenced at line 47">Digit</a> = [<span class="cons_Regular">0</span>]
  <a href="#Digit_1162_1167" id="Digit_1079_1084" title="Referenced at line 47">Digit</a> = [<span class="cons_Regular">1</span>-<span class="cons_Regular">9</span>]
  <a href="#DigitsAndUnderscores_1035_1055" id="DigitsAndUnderscores_1095_1115" title="Referenced at line 43">DigitsAndUnderscores</a> = <a href="#DigitsOrUnderscore_1140_1158" id="DigitsOrUnderscore_1118_1136" title="Defined at line 47">DigitsOrUnderscore</a>+
  <a href="#DigitsOrUnderscore_1118_1136" id="DigitsOrUnderscore_1140_1158" title="Referenced at line 46">DigitsOrUnderscore</a> = (<a href="#Digit_1065_1070" id="Digit_1162_1167" title="Defined at line 44, 45">Digit</a> | [\_])
  <span id="Underscores_1178_1189" title="Not referenced locally, nor via imports">Underscores</span> = [\_]+


<span class="keyword">lexical restrictions</span>

  <a href="#DeciFloatLiteral_383_399" id="DeciFloatLiteral_1224_1240" title="Defined at line 22, 29, 30, 31, 32">DeciFloatLiteral</a> -/- [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#DeciDoubleLiteral_421_438" id="DeciDoubleLiteral_1252_1269" title="Defined at line 24, 34, 35, 36, 37">DeciDoubleLiteral</a> -/- [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]
  <a href="#SignedInteger_967_980" id="SignedInteger_1281_1294" title="Defined at line 40">SignedInteger</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]

<span class="keyword">lexical syntax</span>

  <a href="#HexaFloatLiteral_256_272" id="HexaFloatLiteral_1324_1340" title="Referenced at line 16">HexaFloatLiteral</a> = <a href="#HexaSignificand_1440_1455" id="HexaSignificand_1343_1358" title="Defined at line 61, 62">HexaSignificand</a> <a href="#BinaryExponent_1590_1604" id="BinaryExponent_1359_1373" title="Defined at line 63">BinaryExponent</a> [<span class="cons_Regular">f</span><span class="cons_Regular">F</span>]
  <a href="#HexaDoubleLiteral_347_364" id="HexaDoubleLiteral_1381_1398" title="Referenced at line 18">HexaDoubleLiteral</a> = <a href="#HexaSignificand_1440_1455" id="HexaSignificand_1401_1416" title="Defined at line 61, 62">HexaSignificand</a> <a href="#BinaryExponent_1590_1604" id="BinaryExponent_1417_1431" title="Defined at line 63">BinaryExponent</a> [<span class="cons_Regular">d</span><span class="cons_Regular">D</span>]?
  <a href="#HexaSignificand_1651_1666" id="HexaSignificand_1440_1455" title="Referenced at line 67">HexaSignificand</a> = [<span class="cons_Regular">0</span>] [<span class="cons_Regular">x</span><span class="cons_Regular">X</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] <span class="cons_Lit">"."</span>?  
  <a href="#HexaSignificand_1651_1666" id="HexaSignificand_1503_1518" title="Referenced at line 67">HexaSignificand</a> = [<span class="cons_Regular">0</span>] [<span class="cons_Regular">x</span><span class="cons_Regular">X</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] <span class="cons_Lit">"."</span> [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\_]* [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
  <a href="#BinaryExponent_1417_1431" id="BinaryExponent_1590_1604" title="Referenced at line 60">BinaryExponent</a> = [<span class="cons_Regular">p</span><span class="cons_Regular">P</span>] <a href="#SignedInteger_967_980" id="SignedInteger_1612_1625" title="Defined at line 40">SignedInteger</a>

<span class="keyword">lexical restrictions</span>

  <a href="#HexaSignificand_1440_1455" id="HexaSignificand_1651_1666" title="Defined at line 61, 62">HexaSignificand</a> -/- [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>\.]

</code></pre></td></tr></tbody></table></div>