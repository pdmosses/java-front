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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/literals/StringLiterals_192_220" id="java/literals/StringLiterals_7_35" title="Referenced at ../Main.sdf3 line 10">java/literals/StringLiterals</a>

<span class="layout">// 3.10.5. String Literals</span>

<span class="keyword">imports</span>
  <a href="../EscapeSequences.sdf3#java/literals/EscapeSequences_7_36" id="java/literals/EscapeSequences_75_104" title="Defined at ../EscapeSequences.sdf3 line 1">java/literals/EscapeSequences</a>
  <a href="../../lexical/UnicodeEscapes.sdf3#java/lexical/UnicodeEscapes_7_34" id="java/lexical/UnicodeEscapes_107_134" title="Defined at ../../lexical/UnicodeEscapes.sdf3 line 1">java/lexical/UnicodeEscapes</a>

<span class="keyword">context-free start-symbols</span>

  <a href="#StringLiteral_205_218" id="StringLiteral_166_179" title="Defined at line 15, 19">StringLiteral</a>
  
<span class="keyword">context-free sorts</span>

  <a href="#StringLiteral_166_179" id="StringLiteral_205_218" title="Referenced at line 11; ../Main.sdf3 line 23">StringLiteral</a>

<span class="keyword">context-free syntax</span>

  <a href="#StringLiteral_166_179" id="StringLiteral_243_256" title="Referenced at line 11; ../Main.sdf3 line 23">StringLiteral</a>.<span class="cons_Constructor"><span id="StringLiteral_257_270" title="Not referenced locally, nor via imports">StringLiteral</span></span> = <a href="#StringLit_305_314" id="StringLit_273_282" title="Defined at line 23, 27">StringLit</a>  
  
<span class="keyword">lexical sorts</span>

  <a href="#StringLit_273_282" id="StringLit_305_314" title="Referenced at line 19">StringLit</a>

<span class="keyword">lexical syntax</span>

  <a href="#StringLit_273_282" id="StringLit_334_343" title="Referenced at line 19">StringLit</a> = <span class="cons_Lit">"\""</span> <a href="#StringPart_370_380" id="StringPart_351_361" title="Defined at line 28, 29, 30">StringPart</a>* <span class="cons_Lit">"\""</span>
  <a href="#StringPart_351_361" id="StringPart_370_380" title="Referenced at line 27">StringPart</a> = <a href="../../lexical/UnicodeEscapes.sdf3#UnicodeEscape_71_84" id="UnicodeEscape_383_396" title="Defined at ../../lexical/UnicodeEscapes.sdf3 line 7">UnicodeEscape</a>
  <a href="#StringPart_351_361" id="StringPart_399_409" title="Referenced at line 27">StringPart</a> = <a href="../EscapeSequences.sdf3#EscapeSeq_119_128" id="EscapeSeq_412_421" title="Defined at ../EscapeSequences.sdf3 line 7, 8">EscapeSeq</a>
  <a href="#StringPart_351_361" id="StringPart_424_434" title="Referenced at line 27">StringPart</a> = <a href="#StringChars_451_462" id="StringChars_437_448" title="Defined at line 31">StringChars</a>
  <a href="#StringChars_503_514" id="StringChars_451_462" title="Referenced at line 35">StringChars</a> = ~[\"\\\n\r]+

<span class="keyword">lexical restrictions</span>

  <a href="#StringChars_451_462" id="StringChars_503_514" title="Defined at line 31">StringChars</a> -/- ~[\"\\\n\r]
</code></pre></td></tr></tbody></table></div>