---
title: Comments.sdf3
hide:
  - toc
---

# `Comments.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/Comments.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/Comments.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/Comments.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/lexical/Comments_69_90" id="java/lexical/Comments_7_28" title="Referenced at ../Main.sdf3 line 6; ../../Test.sdf3 line 8">java/lexical/Comments</a>

<span class="layout">// 3.7. Comments</span>

<span class="keyword">imports</span>

  <a href="../LineTerminators.sdf3/#java/lexical/LineTerminators_7_35" id="java/lexical/LineTerminators_59_87" title="Defined at ../LineTerminators.sdf3 line 1">java/lexical/LineTerminators</a>

<span class="keyword">lexical start-symbols</span>
  
  <a href="#Comment_162_169" id="Comment_116_123" title="Defined at line 16, 18, 19, 20">Comment</a>

<span class="keyword">lexical syntax</span>

  <span class="keyword">LAYOUT</span> = <a href="#Comment_162_169" id="Comment_152_159" title="Defined at line 16, 18, 19, 20">Comment</a>
  <a href="#Comment_116_123" id="Comment_162_169" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"//"</span> <a href="#EOLCommentChars_210_225" id="EOLCommentChars_177_192" title="Defined at line 17">EOLCommentChars</a> <a href="../LineTerminators.sdf3/#LineTerminator_81_95" id="LineTerminator_193_207" title="Defined at ../LineTerminators.sdf3 line 7, 8, 9, 10">LineTerminator</a>
  <a href="#EOLCommentChars_177_192" id="EOLCommentChars_210_225" title="Referenced at line 16, 39">EOLCommentChars</a> = ~[\n\r]*
  <a href="#Comment_116_123" id="Comment_239_246" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"/*"</span> <a href="#CommentPart_329_340" id="CommentPart_254_265" title="Defined at line 21, 22, 23, 24, 25">CommentPart</a>* <span class="cons_Lit">"*/"</span>
  <a href="#Comment_116_123" id="Comment_274_281" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"/**"</span> <a href="#CommentPart_329_340" id="CommentPart_290_301" title="Defined at line 21, 22, 23, 24, 25">CommentPart</a>* <span class="cons_Lit">"*/"</span>
  <a href="#Comment_116_123" id="Comment_310_317" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"/**/"</span>
  <a href="#CommentPart_254_265" id="CommentPart_329_340" title="Referenced at line 18, 19">CommentPart</a> = <a href="#BlockCommentChars_469_486" id="BlockCommentChars_343_360" title="Defined at line 26">BlockCommentChars</a>
  <a href="#CommentPart_254_265" id="CommentPart_363_374" title="Referenced at line 18, 19">CommentPart</a> = <a href="#EscChar_539_546" id="EscChar_377_384" title="Defined at line 29">EscChar</a>
  <a href="#CommentPart_254_265" id="CommentPart_387_398" title="Referenced at line 18, 19">CommentPart</a> = <a href="#EscEscChar_517_527" id="EscEscChar_401_411" title="Defined at line 28">EscEscChar</a>
  <a href="#CommentPart_254_265" id="CommentPart_414_425" title="Referenced at line 18, 19">CommentPart</a> = <a href="#Asterisk_500_508" id="Asterisk_428_436" title="Defined at line 27">Asterisk</a>
  <a href="#CommentPart_254_265" id="CommentPart_439_450" title="Referenced at line 18, 19">CommentPart</a> = <a href="#UnicodeEscape_556_569" id="UnicodeEscape_453_466" title="Defined at line 30">UnicodeEscape</a>
  <a href="#BlockCommentChars_343_360" id="BlockCommentChars_469_486" title="Referenced at line 21, 38">BlockCommentChars</a> = ~[\*\\]+
  <a href="#Asterisk_428_436" id="Asterisk_500_508" title="Referenced at line 24, 36">Asterisk</a> = <span class="cons_Lit">"*"</span>
  <a href="#EscEscChar_401_411" id="EscEscChar_517_527" title="Referenced at line 23">EscEscChar</a> = <span class="cons_Lit">"\\\\"</span>
  <a href="#EscChar_377_384" id="EscChar_539_546" title="Referenced at line 22, 37">EscChar</a> = <span class="cons_Lit">"\\"</span>
  <a href="#UnicodeEscape_453_466" id="UnicodeEscape_556_569" title="Referenced at line 25">UnicodeEscape</a> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">u</span>]+ [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]

<span class="keyword">lexical restrictions</span>

  <span class="cons_Lit">"/**"</span> -/- [\/]
  <span class="cons_Lit">"/*"</span> -/- [\*]
  <a href="#Asterisk_500_508" id="Asterisk_688_696" title="Defined at line 27">Asterisk</a> -/- [\/]
  <a href="#EscChar_539_546" id="EscChar_708_715" title="Defined at line 29">EscChar</a> -/- [\\<span class="cons_Regular">u</span>]
  <a href="#BlockCommentChars_469_486" id="BlockCommentChars_728_745" title="Defined at line 26">BlockCommentChars</a> -/- ~[\*\\]
  <a href="#EOLCommentChars_210_225" id="EOLCommentChars_760_775" title="Defined at line 17">EOLCommentChars</a> -/- ~[\n<span class="cons_Decimal">\13</span>]

<span class="keyword">context-free restrictions</span>

  <span class="keyword">LAYOUT</span>? -/- [\/].[\*]
  <span class="keyword">LAYOUT</span>? -/- [\/].[\/]
</code></pre></td></tr></tbody></table></div>