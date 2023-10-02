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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/literals/CharacterLiterals_158_189" id="java/literals/CharacterLiterals_7_38" title="Referenced at ../Main.sdf3 line 9">java/literals/CharacterLiterals</a>

<span class="layout">// 3.10.4. Character Literals</span>

<span class="keyword">imports</span>
  <a href="../EscapeSequences.sdf3#java/literals/EscapeSequences_7_36" id="java/literals/EscapeSequences_81_110" title="Defined at ../EscapeSequences.sdf3 line 1">java/literals/EscapeSequences</a>
  <a href="../../lexical/UnicodeEscapes.sdf3#java/lexical/UnicodeEscapes_7_34" id="java/lexical/UnicodeEscapes_113_140" title="Defined at ../../lexical/UnicodeEscapes.sdf3 line 1">java/lexical/UnicodeEscapes</a>
  
<span class="keyword">context-free start-symbols</span>
  
  <a href="#CharacterLiteral_222_238" id="CharacterLiteral_176_192" title="Defined at line 15, 19">CharacterLiteral</a>  
  
<span class="keyword">context-free sorts</span>
  
  <a href="#CharacterLiteral_176_192" id="CharacterLiteral_222_238" title="Referenced at line 11; ../Main.sdf3 line 22">CharacterLiteral</a>  
  
<span class="keyword">context-free syntax</span>

  <a href="#CharacterLiteral_176_192" id="CharacterLiteral_267_283" title="Referenced at line 11; ../Main.sdf3 line 22">CharacterLiteral</a>.<span class="cons_Constructor"><span id="CharLiteral_284_295" title="Not referenced locally, nor via imports">CharLiteral</span></span> = <a href="#CharLiteral_332_343" id="CharLiteral_298_309" title="Defined at line 23, 27, 28, 29">CharLiteral</a>  
  
<span class="keyword">lexical sorts</span>

  <a href="#CharLiteral_298_309" id="CharLiteral_332_343" title="Referenced at line 19">CharLiteral</a>  

<span class="keyword">lexical syntax</span>

  <a href="#CharLiteral_298_309" id="CharLiteral_365_376" title="Referenced at line 19">CharLiteral</a> = <span class="cons_Lit">"'"</span> ~[\n\r\'\\] <span class="cons_Lit">"'"</span>
  <a href="#CharLiteral_298_309" id="CharLiteral_401_412" title="Referenced at line 19">CharLiteral</a> = <span class="cons_Lit">"'"</span> <a href="../EscapeSequences.sdf3#EscapeSeq_119_128" id="EscapeSeq_419_428" title="Defined at ../EscapeSequences.sdf3 line 7, 8">EscapeSeq</a> <span class="cons_Lit">"'"</span>
  <a href="#CharLiteral_298_309" id="CharLiteral_435_446" title="Referenced at line 19">CharLiteral</a> = <span class="cons_Lit">"'"</span> <a href="../../lexical/UnicodeEscapes.sdf3#UnicodeEscape_71_84" id="UnicodeEscape_453_466" title="Defined at ../../lexical/UnicodeEscapes.sdf3 line 7">UnicodeEscape</a> <span class="cons_Lit">"'"</span>
</code></pre></td></tr></tbody></table></div>