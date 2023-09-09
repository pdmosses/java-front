---
title: LineTerminators.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/lexical/LineTerminators_144_172" id="java/lexical/LineTerminators_7_35" title="Referenced at ../Main.sdf3 line 9">java/lexical/LineTerminators</a>

<span class="layout">// 3.4. Line Terminators</span>

<span class="keyword">lexical syntax</span>

  <a href="../Comments.sdf3#LineTerminator_193_207" id="LineTerminator_81_95" title="Referenced at ../Comments.sdf3 line 16">LineTerminator</a> = [\n]
  <a href="../Comments.sdf3#LineTerminator_193_207" id="LineTerminator_105_119" title="Referenced at ../Comments.sdf3 line 16">LineTerminator</a> = [\r] [\n]
  <a href="../Comments.sdf3#LineTerminator_193_207" id="LineTerminator_134_148" title="Referenced at ../Comments.sdf3 line 16">LineTerminator</a> = <a href="#CarriageReturn_197_211" id="CarriageReturn_151_165" title="Defined at line 11">CarriageReturn</a>
  <a href="../Comments.sdf3#LineTerminator_193_207" id="LineTerminator_168_182" title="Referenced at ../Comments.sdf3 line 16">LineTerminator</a> = <a href="#EndOfFile_287_296" id="EndOfFile_185_194" title="Defined at line 19">EndOfFile</a>
  <a href="#CarriageReturn_244_258" id="CarriageReturn_197_211" title="Referenced at line 15">CarriageReturn</a> = [\r]

<span class="keyword">lexical restrictions</span>

  <a href="#CarriageReturn_197_211" id="CarriageReturn_244_258" title="Defined at line 11">CarriageReturn</a> -/- [\n]

<span class="keyword">lexical syntax</span>

  <a href="#EndOfFile_324_333" id="EndOfFile_287_296" title="Referenced at line 23">EndOfFile</a> =

<span class="keyword">lexical restrictions</span>

  <a href="#EndOfFile_287_296" id="EndOfFile_324_333" title="Defined at line 19">EndOfFile</a> -/- ~[]
</code></pre></td></tr></tbody></table></div>