---
title: Keywords.sdf3
hide:
  - toc
---

# `Keywords.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/Keywords.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/Keywords.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/Keywords.sdf3 "The source file on GitHub"

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
68
69
70
71
72
73
74
75
76
77
78
79
80
81
82
83
84
85
86
87
88
89
90
91
92
93
94
95
96
97
98
99
100
101
102
103
104
105
106
107
108
109
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/lexical/Keywords_1_8" title="a definition with multiple references" data-urls="../Identifiers.sdf3/#java/lexical/Keywords line 7_3; ../Main.sdf3/#java/lexical/Keywords line 8_3">java/lexical/Keywords</button>

<span class="layout">// 3.9. Keywords</span>

<span class="keyword">lexical syntax</span>

  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_7_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"abstract"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_8_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"assert"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_9_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"boolean"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_10_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"break"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_11_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"byte"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_12_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"case"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_13_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"catch"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_14_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"char"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_15_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"class"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_16_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"const"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_17_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"continue"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_18_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"default"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_19_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"do"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_20_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"double"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_21_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"else"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_22_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"enum"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_23_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"extends"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_24_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"final"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_25_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"finally"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_26_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"float"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_27_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"for"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_28_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"goto"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_29_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"if"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_30_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"implements"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_31_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"import"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_32_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"instanceof"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_33_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"int"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_34_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"interface"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_35_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"long"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_36_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"native"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_37_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"new"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_38_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"package"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_39_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"private"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_40_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"protected"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_41_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"public"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_42_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"return"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_43_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"short"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_44_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"static"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_45_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"strictfp"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_46_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"super"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_47_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"switch"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_48_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"synchronized"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_49_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"this"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_50_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"throw"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_51_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"throws"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_52_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"transient"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_53_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"try"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_54_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"void"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_55_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"volatile"</span>
  <a href="../Identifiers.sdf3/#Keyword_28_8" id="Keyword_56_3" title="a definition with a single reference">Keyword</a> = <span class="cons_Lit">"while"</span>

<span class="keyword">lexical restrictions</span>

  <span class="cons_Lit">"abstract"</span>
  <span class="cons_Lit">"assert"</span>
  <span class="cons_Lit">"boolean"</span>
  <span class="cons_Lit">"break"</span>
  <span class="cons_Lit">"byte"</span>
  <span class="cons_Lit">"case"</span>
  <span class="cons_Lit">"catch"</span>
  <span class="cons_Lit">"char"</span>
  <span class="cons_Lit">"class"</span>
  <span class="cons_Lit">"const"</span>
  <span class="cons_Lit">"continue"</span>
  <span class="cons_Lit">"default"</span>
  <span class="cons_Lit">"do"</span>
  <span class="cons_Lit">"double"</span>
  <span class="cons_Lit">"else"</span>
  <span class="cons_Lit">"enum"</span>
  <span class="cons_Lit">"extends"</span>
  <span class="cons_Lit">"final"</span>
  <span class="cons_Lit">"finally"</span>
  <span class="cons_Lit">"float"</span>
  <span class="cons_Lit">"for"</span>
  <span class="cons_Lit">"goto"</span>
  <span class="cons_Lit">"if"</span>
  <span class="cons_Lit">"implements"</span>
  <span class="cons_Lit">"import"</span>
  <span class="cons_Lit">"instanceof"</span>
  <span class="cons_Lit">"int"</span>
  <span class="cons_Lit">"interface"</span>
  <span class="cons_Lit">"long"</span>
  <span class="cons_Lit">"native"</span>
  <span class="cons_Lit">"new"</span>
  <span class="cons_Lit">"package"</span>
  <span class="cons_Lit">"private"</span>
  <span class="cons_Lit">"protected"</span>
  <span class="cons_Lit">"public"</span>
  <span class="cons_Lit">"return"</span>
  <span class="cons_Lit">"short"</span>
  <span class="cons_Lit">"static"</span>
  <span class="cons_Lit">"strictfp"</span>
  <span class="cons_Lit">"super"</span>
  <span class="cons_Lit">"switch"</span>
  <span class="cons_Lit">"synchronized"</span>
  <span class="cons_Lit">"this"</span>
  <span class="cons_Lit">"throw"</span>
  <span class="cons_Lit">"throws"</span>
  <span class="cons_Lit">"transient"</span>
  <span class="cons_Lit">"try"</span>
  <span class="cons_Lit">"void"</span>
  <span class="cons_Lit">"volatile"</span>
  <span class="cons_Lit">"while"</span> -/- [<span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$]
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
