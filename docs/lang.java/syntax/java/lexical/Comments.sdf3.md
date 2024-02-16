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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Comments_1_8" title="a definition with multiple references" data-urls="../Main.sdf3/#java/lexical/Comments line 6_3; ../../Test.sdf3/#java/lexical/Comments line 8_3">java/lexical/Comments</button>

<span class="layout">// 3.7. Comments</span>

<span class="keyword">imports</span>

  <a href="../LineTerminators.sdf3/#java/lexical/LineTerminators_1_8" id="java/lexical/LineTerminators_7_3" title="a reference to a single-file definition">java/lexical/LineTerminators</a>

<span class="keyword">lexical start-symbols</span>
  
  <a href="#Comment_16_3" id="Comment_11_3" title="a reference to a single-file definition">Comment</a>

<span class="keyword">lexical syntax</span>

  <span class="keyword">LAYOUT</span> = <a href="#Comment_16_3" id="Comment_15_12" title="a reference to a single-file definition">Comment</a>
  <button class="modal-open" id="Comment_16_3" title="a definition with multiple references" data-urls="#Comment line 11_3, 15_12">Comment</button> = <span class="cons_Lit">"//"</span> <a href="#EOLCommentChars_17_3" id="EOLCommentChars_16_18" title="a reference to a single-file definition">EOLCommentChars</a> <a href="../LineTerminators.sdf3/#LineTerminator_7_3" id="LineTerminator_16_34" title="a reference to a single-file definition">LineTerminator</a>
  <button class="modal-open" id="EOLCommentChars_17_3" title="a definition with multiple references" data-urls="#EOLCommentChars line 16_18, 39_3">EOLCommentChars</button> = ~[\n\r]*
  <button class="modal-open" id="Comment_18_3" title="a definition with multiple references" data-urls="#Comment line 11_3, 15_12">Comment</button> = <span class="cons_Lit">"/*"</span> <a href="#CommentPart_21_3" id="CommentPart_18_18" title="a reference to a single-file definition">CommentPart</a>* <span class="cons_Lit">"*/"</span>
  <button class="modal-open" id="Comment_19_3" title="a definition with multiple references" data-urls="#Comment line 11_3, 15_12">Comment</button> = <span class="cons_Lit">"/**"</span> <a href="#CommentPart_21_3" id="CommentPart_19_19" title="a reference to a single-file definition">CommentPart</a>* <span class="cons_Lit">"*/"</span>
  <button class="modal-open" id="Comment_20_3" title="a definition with multiple references" data-urls="#Comment line 11_3, 15_12">Comment</button> = <span class="cons_Lit">"/**/"</span>
  <button class="modal-open" id="CommentPart_21_3" title="a definition with multiple references" data-urls="#CommentPart line 18_18, 19_19">CommentPart</button> = <a href="#BlockCommentChars_26_3" id="BlockCommentChars_21_17" title="a reference to a single-file definition">BlockCommentChars</a>
  <button class="modal-open" id="CommentPart_22_3" title="a definition with multiple references" data-urls="#CommentPart line 18_18, 19_19">CommentPart</button> = <a href="#EscChar_29_3" id="EscChar_22_17" title="a reference to a single-file definition">EscChar</a>
  <button class="modal-open" id="CommentPart_23_3" title="a definition with multiple references" data-urls="#CommentPart line 18_18, 19_19">CommentPart</button> = <a href="#EscEscChar_28_3" id="EscEscChar_23_17" title="a reference to a single-file definition">EscEscChar</a>
  <button class="modal-open" id="CommentPart_24_3" title="a definition with multiple references" data-urls="#CommentPart line 18_18, 19_19">CommentPart</button> = <a href="#Asterisk_27_3" id="Asterisk_24_17" title="a reference to a single-file definition">Asterisk</a>
  <button class="modal-open" id="CommentPart_25_3" title="a definition with multiple references" data-urls="#CommentPart line 18_18, 19_19">CommentPart</button> = <a href="#UnicodeEscape_30_3" id="UnicodeEscape_25_17" title="a reference to a single-file definition">UnicodeEscape</a>
  <button class="modal-open" id="BlockCommentChars_26_3" title="a definition with multiple references" data-urls="#BlockCommentChars line 21_17, 38_3">BlockCommentChars</button> = ~[\*\\]+
  <button class="modal-open" id="Asterisk_27_3" title="a definition with multiple references" data-urls="#Asterisk line 24_17, 36_3">Asterisk</button> = <span class="cons_Lit">"*"</span>
  <a href="#EscEscChar_23_17" id="EscEscChar_28_3" title="a definition with a single reference">EscEscChar</a> = <span class="cons_Lit">"\\\\"</span>
  <button class="modal-open" id="EscChar_29_3" title="a definition with multiple references" data-urls="#EscChar line 22_17, 37_3">EscChar</button> = <span class="cons_Lit">"\\"</span>
  <a href="#UnicodeEscape_25_17" id="UnicodeEscape_30_3" title="a definition with a single reference">UnicodeEscape</a> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">u</span>]+ [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]

<span class="keyword">lexical restrictions</span>

  <span class="cons_Lit">"/**"</span> -/- [\/]
  <span class="cons_Lit">"/*"</span> -/- [\*]
  <a href="#Asterisk_27_3" id="Asterisk_36_3" title="a reference to a single-file definition">Asterisk</a> -/- [\/]
  <a href="#EscChar_29_3" id="EscChar_37_3" title="a reference to a single-file definition">EscChar</a> -/- [\\<span class="cons_Regular">u</span>]
  <a href="#BlockCommentChars_26_3" id="BlockCommentChars_38_3" title="a reference to a single-file definition">BlockCommentChars</a> -/- ~[\*\\]
  <a href="#EOLCommentChars_17_3" id="EOLCommentChars_39_3" title="a reference to a single-file definition">EOLCommentChars</a> -/- ~[\n<span class="cons_Decimal">\13</span>]

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
