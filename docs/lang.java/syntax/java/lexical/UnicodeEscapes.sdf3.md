---
title: UnicodeEscapes.sdf3
---

# `UnicodeEscapes.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/UnicodeEscapes.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/UnicodeEscapes.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/UnicodeEscapes.sdf3 "The source file on GitHub"

<div class="sdf3"><table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span></span>1
2
3
4
5
6
7
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../literals/StringLiterals.sdf3#java/lexical/UnicodeEscapes_107_134" id="java/lexical/UnicodeEscapes_7_34" title="Referenced at ../../literals/StringLiterals.sdf3 line 7">java/lexical/UnicodeEscapes</a>

<span class="layout">// 3.3. Unicode Escapes</span>

<span class="keyword">syntax</span>

  <a href="../../literals/CharacterLiterals.sdf3#UnicodeEscape_453_466" id="UnicodeEscape_71_84" title="Referenced at ../../literals/CharacterLiterals.sdf3 line 29; ../../literals/StringLiterals.sdf3 line 28">UnicodeEscape</a>.<span class="cons_Constructor"><span id="UnicodeEscape_85_98" title="Not referenced locally, nor via imports">UnicodeEscape</span></span> = <span class="cons_Lit">"\\"</span> [<span class="cons_Regular">u</span>]+ [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>] [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span><span class="cons_Regular">a</span>-<span class="cons_Regular">f</span><span class="cons_Regular">A</span>-<span class="cons_Regular">F</span>]
</code></pre></td></tr></tbody></table></div>