---
title: LineTerminators.sdf3
hide:
  - toc
---

# `LineTerminators.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/LineTerminators.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/LineTerminators.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/LineTerminators.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/LineTerminators_1_8" title="a definition with multiple references" data-urls="../Comments.sdf3/#java/lexical/LineTerminators line 7_3; ../Main.sdf3/#java/lexical/LineTerminators line 9_3; ../../Test.sdf3/#java/lexical/LineTerminators line 10_3">java/lexical/LineTerminators</button>

<span class="layout">// 3.4. Line Terminators</span>

<span class="keyword">lexical syntax</span>

  <a href="../Comments.sdf3/#LineTerminator_16_34" id="LineTerminator_7_3" title="a definition with a single reference">LineTerminator</a> = [\n]
  <a href="../Comments.sdf3/#LineTerminator_16_34" id="LineTerminator_8_3" title="a definition with a single reference">LineTerminator</a> = [\r] [\n]
  <a href="../Comments.sdf3/#LineTerminator_16_34" id="LineTerminator_9_3" title="a definition with a single reference">LineTerminator</a> = <a href="#CarriageReturn_11_3" id="CarriageReturn_9_20" title="a reference to a single-file definition">CarriageReturn</a>
  <a href="../Comments.sdf3/#LineTerminator_16_34" id="LineTerminator_10_3" title="a definition with a single reference">LineTerminator</a> = <a href="#EndOfFile_19_3" id="EndOfFile_10_20" title="a reference to a single-file definition">EndOfFile</a>
  <button class="modal-open" id="CarriageReturn_11_3" title="a definition with multiple references" data-urls="#CarriageReturn line 9_20, 15_3">CarriageReturn</button> = [\r]

<span class="keyword">lexical restrictions</span>

  <a href="#CarriageReturn_11_3" id="CarriageReturn_15_3" title="a reference to a single-file definition">CarriageReturn</a> -/- [\n]

<span class="keyword">lexical syntax</span>

  <button class="modal-open" id="EndOfFile_19_3" title="a definition with multiple references" data-urls="#EndOfFile line 10_20, 23_3">EndOfFile</button> =

<span class="keyword">lexical restrictions</span>

  <a href="#EndOfFile_19_3" id="EndOfFile_23_3" title="a reference to a single-file definition">EndOfFile</a> -/- ~[]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
