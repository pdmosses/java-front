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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Comments_1_8" title="Multi-file references" data-urls="../Main.sdf3/#java/lexical/Comments_6_3 line 6; ../../Test.sdf3/#java/lexical/Comments_8_3 line 8">java/lexical/Comments</button>

<span class="layout">// 3.7. Comments</span>

<span class="keyword">imports</span>

  <a href="../LineTerminators.sdf3/#java/lexical/LineTerminators_1_8" id="java/lexical/LineTerminators_7_3" title="Defined at ../LineTerminators.sdf3 line 1">java/lexical/LineTerminators</a>

<span class="keyword">lexical start-symbols</span>
  
  <a href="#Comment_16_3" id="Comment_11_3" title="Defined at line 16, 18, 19, 20">Comment</a>

<span class="keyword">lexical syntax</span>

  <span class="keyword">LAYOUT</span> = <a href="#Comment_16_3" id="Comment_15_12" title="Defined at line 16, 18, 19, 20">Comment</a>
  <a href="#Comment_11_3" id="Comment_16_3" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"//"</span> <a href="#EOLCommentChars_17_3" id="EOLCommentChars_16_18" title="Defined at line 17">EOLCommentChars</a> <a href="../LineTerminators.sdf3/#LineTerminator_7_3" id="LineTerminator_16_34" title="Defined at ../LineTerminators.sdf3 line 7, 8, 9, 10">LineTerminator</a>
  <a href="#EOLCommentChars_16_18" id="EOLCommentChars_17_3" title="Referenced at line 16, 39">EOLCommentChars</a> = ~[\n\r]*
  <a href="#Comment_11_3" id="Comment_18_3" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"/*"</span> <a href="#CommentPart_21_3" id="CommentPart_18_18" title="Defined at line 21, 22, 23, 24, 25">CommentPart</a>* <span class="cons_Lit">"*/"</span>
  <a href="#Comment_11_3" id="Comment_19_3" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"/**"</span> <a href="#CommentPart_21_3" id="CommentPart_19_19" title="Defined at line 21, 22, 23, 24, 25">CommentPart</a>* <span class="cons_Lit">"*/"</span>
  <a href="#Comment_11_3" id="Comment_20_3" title="Referenced at line 11, 15">Comment</a> = <span class="cons_Lit">"/**/"</span>
  <a href="#CommentPart_18_18" id="CommentPart_21_3" title="Referenced at line 18, 19">CommentPart</a> = <a href="#BlockCommentChars_26_3" id="BlockCommentChars_21_17" title="Defined at line 26">BlockCommentChars</a>
  <a href="#CommentPart_18_18" id="CommentPart_22_3" title="Referenced at line 18, 19">CommentPart</a> = <a href="#EscChar_29_3" id="EscChar_22_17" title="Defined at line 29">EscChar</a>
  <a href="#CommentPart_18_18" id="CommentPart_23_3" title="Referenced at line 18, 19">CommentPart</a> = <a href="#EscEscChar_28_3" id="EscEscChar_23_17" title="Defined at line 28">EscEscChar</a>
  <a href="#CommentPart_18_18" id="CommentPart_24_3" title="Referenced at line 18, 19">CommentPart</a> = <a href="#Asterisk_27_3" id="Asterisk_24_17" title="Defined at line 27">Asterisk</a>
  <a href="#CommentPart_18_18" id="CommentPart_25_3" title="Referenced at line 18, 19">CommentPart</a> = <a href="#UnicodeEscape_30_3" id="UnicodeEscape_25_17" title="Defined at line 30">UnicodeEscape</a>
  <a href="#BlockCommentChars_21_17" id="BlockCommentChars_26_3" title="Referenced at line 21, 38">BlockCommentChars</a> = ~[\*\\]+
  <a href="#Asterisk_24_17" id="Asterisk_27_3" title="Referenced at line 24, 36">Asterisk</a> = <span class="cons_Lit">"*"</span>
  <a href="#EscEscChar_23_17" id="EscEscChar_28_3" title="Referenced at line 23">EscEscChar</a> = <span class="cons_Lit">"\\\\"</span>
  <a href="#EscChar_22_17" id="EscChar_29_3" title="Referenced at line 22, 37">EscChar</a> = <span class="cons_Lit">"\\"</span>
  <a href="#UnicodeEscape_25_17" id="UnicodeEscape_30_3" title="Referenced at line 25">UnicodeEscape</a> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">u</span>]+ [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]

<span class="keyword">lexical restrictions</span>

  <span class="cons_Lit">"/**"</span> -/- [\/]
  <span class="cons_Lit">"/*"</span> -/- [\*]
  <a href="#Asterisk_27_3" id="Asterisk_36_3" title="Defined at line 27">Asterisk</a> -/- [\/]
  <a href="#EscChar_29_3" id="EscChar_37_3" title="Defined at line 29">EscChar</a> -/- [\\<span class="cons_Regular">u</span>]
  <a href="#BlockCommentChars_26_3" id="BlockCommentChars_38_3" title="Defined at line 26">BlockCommentChars</a> -/- ~[\*\\]
  <a href="#EOLCommentChars_17_3" id="EOLCommentChars_39_3" title="Defined at line 17">EOLCommentChars</a> -/- ~[\n<span class="cons_Decimal">\13</span>]

<span class="keyword">context-free restrictions</span>

  <span class="keyword">LAYOUT</span>? -/- [\/].[\*]
  <span class="keyword">LAYOUT</span>? -/- [\/].[\/]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
