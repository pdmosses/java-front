---
title: Keywords.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/lexical/Keywords_120_141" id="java/lexical/Keywords_7_28" title="Referenced at ../Main.sdf3 line 8">java/lexical/Keywords</a>

<span class="layout">// 3.9. Keywords</span>

<span class="keyword">lexical syntax</span>

  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_66_73" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"abstract"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_89_96" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"assert"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_110_117" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"boolean"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_132_139" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"break"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_152_159" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"byte"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_171_178" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"case"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_190_197" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"catch"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_210_217" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"char"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_229_236" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"class"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_249_256" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"const"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_269_276" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"continue"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_292_299" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"default"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_314_321" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"do"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_331_338" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"double"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_352_359" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"else"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_371_378" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"enum"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_390_397" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"extends"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_412_419" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"final"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_432_439" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"finally"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_454_461" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"float"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_474_481" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"for"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_492_499" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"goto"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_511_518" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"if"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_528_535" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"implements"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_553_560" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"import"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_574_581" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"instanceof"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_599_606" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"int"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_617_624" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"interface"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_641_648" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"long"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_660_667" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"native"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_681_688" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"new"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_699_706" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"package"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_721_728" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"private"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_743_750" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"protected"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_767_774" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"public"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_788_795" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"return"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_809_816" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"short"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_829_836" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"static"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_850_857" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"strictfp"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_873_880" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"super"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_893_900" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"switch"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_914_921" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"synchronized"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_941_948" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"this"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_960_967" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"throw"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_980_987" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"throws"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_1001_1008" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"transient"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_1025_1032" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"try"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_1043_1050" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"void"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_1062_1069" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"volatile"</span>
  <a href="../Identifiers.sdf3#Keyword_263_270" id="Keyword_1085_1092" title="Referenced at ../Identifiers.sdf3 line 28">Keyword</a> = <span class="cons_Lit">"while"</span>

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