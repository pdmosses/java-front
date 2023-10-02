---
title: Statements.sdf3
hide:
  - toc
---

# `Statements.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/statements/Statements.sdf3]

[pdmosses/java-front/lang.java/syntax/java/statements/Statements.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/statements/Statements.sdf3 "The source file on GitHub"

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
110
111
112
113
114
115
116
117
118
119
120
121
122
123
124
125
126
127
128
129
130
131
132
133
134
135
136
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/statements/Statements_146_172" id="java/statements/Statements_7_33" title="Referenced at ../Main.sdf3 line 8">java/statements/Statements</a>

<span class="layout">// 14.5. Statements</span>

<span class="keyword">imports</span>
  <a href="../../classes/FieldDeclarations.sdf3#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_66_96" title="Defined at ../../classes/FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../../classes/MethodDeclarations.sdf3#java/classes/MethodDeclarations_7_38" id="java/classes/MethodDeclarations_99_130" title="Defined at ../../classes/MethodDeclarations.sdf3 line 1">java/classes/MethodDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_133_157" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../Blocks.sdf3#java/statements/Blocks_7_29" id="java/statements/Blocks_160_182" title="Defined at ../Blocks.sdf3 line 1">java/statements/Blocks</a>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_185_201" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_204_229" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../expressions/Main.sdf3#java/expressions/Main_7_28" id="java/expressions/Main_232_253" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="#Statement_3401_3410" id="Statement_277_286" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>
  <a href="#ForInit_763_770" id="ForInit_289_296" title="Referenced at line 41">ForInit</a>
  <a href="#ForUpdate_789_798" id="ForUpdate_299_308" title="Referenced at line 41">ForUpdate</a>
  <a href="#Exprs_1037_1042" id="Exprs_311_316" title="Referenced at line 47">Exprs</a>
  <a href="#SwitchGroup_1648_1659" id="SwitchGroup_319_330" title="Referenced at line 66">SwitchGroup</a>
  <a href="#SwitchLabel_1736_1747" id="SwitchLabel_333_344" title="Referenced at line 71">SwitchLabel</a>
  <a href="#CatchClause_3150_3161" id="CatchClause_347_358" title="Referenced at line 125">CatchClause</a>
  <a href="#CatchFormalParameter_2511_2531" id="CatchFormalParameter_361_381" title="Referenced at line 105">CatchFormalParameter</a>
  <a href="#CatchType_2607_2616" id="CatchType_384_393" title="Referenced at line 106">CatchType</a>
  <a href="#CatchTypeRest_2675_2688" id="CatchTypeRest_396_409" title="Referenced at line 107">CatchTypeRest</a>
  <a href="#Resource_3118_3126" id="Resource_412_420" title="Referenced at line 124">Resource</a>
    
<span class="keyword">context-free priorities</span>

  <a href="#Statement_277_286" id="Statement_453_462" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>.<span class="cons_Constructor"><a href="#IfElse_617_623" id="IfElse_463_469" title="Defined at line 37">IfElse</a></span>  &gt; <a href="#Statement_277_286" id="Statement_473_482" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>.<span class="cons_Constructor"><a href="#If_564_566" id="If_483_485" title="Defined at line 36">If</a></span>

<span class="keyword">context-free syntax</span>

  <a href="#Statement_3401_3410" id="Statement_510_519" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Labeled_520_527" title="Not referenced locally, nor via imports">Labeled</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_532_534" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; <span class="cons_String">:</span> &lt;<a href="#Statement_277_286" id="Statement_539_548" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;&gt;

  <a href="#Statement_3401_3410" id="Statement_554_563" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><a href="#If_3411_3413" id="If_564_566" title="Referenced at line 136">If</a></span>      = &lt;<span class="cons_String">if(</span>&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_579_589" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_277_286" id="Statement_593_602" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;&gt;
  <a href="#Statement_3401_3410" id="Statement_607_616" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><a href="#IfElse_3391_3397" id="IfElse_617_623" title="Referenced at line 136">IfElse</a></span>  = &lt;<span class="cons_String">if(</span>&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_632_642" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_277_286" id="Statement_646_655" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt; <span class="cons_String">else</span> &lt;<a href="#Statement_277_286" id="Statement_663_672" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_680_689" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="While_690_695" title="Not referenced locally, nor via imports">While</span></span> = &lt;<span class="cons_String">while(</span>&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_706_716" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_277_286" id="Statement_720_729" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_737_746" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="For_747_750" title="Not referenced locally, nor via imports">For</span></span>     = &lt;<span class="cons_String">for(</span>&lt;<a href="#ForInit_289_296" id="ForInit_763_770" title="Defined at line 17, 44, 45">ForInit</a>&gt;<span class="cons_String">;</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_774_784" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>?&gt;<span class="cons_String">;</span> &lt;<a href="#ForUpdate_299_308" id="ForUpdate_789_798" title="Defined at line 18, 47">ForUpdate</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_277_286" id="Statement_802_811" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;&gt;
  <a href="#Statement_3401_3410" id="Statement_816_825" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="ForEach_826_833" title="Not referenced locally, nor via imports">ForEach</span></span> = &lt;<span class="cons_String">for(</span>&lt;{<a href="../../classes/MethodDeclarations.sdf3#VariableModifier_462_478" id="VariableModifier_843_859" title="Defined at ../../classes/MethodDeclarations.sdf3 line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#UnannType_403_412" id="UnannType_868_877" title="Defined at ../../classes/FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#VarDeclId_343_352" id="VarDeclId_880_889" title="Defined at ../../classes/FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt; <span class="cons_String">:</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_894_904" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_277_286" id="Statement_908_917" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;&gt;
  
  <a href="#ForInit_763_770" id="ForInit_925_932" title="Referenced at line 41">ForInit</a> = <a href="#Exprs_311_316" id="Exprs_935_940" title="Defined at line 19, 49">Exprs</a>
  <a href="#ForInit_763_770" id="ForInit_943_950" title="Referenced at line 41">ForInit</a>.<span class="cons_Constructor"><span id="VarDecls_951_959" title="Not referenced locally, nor via imports">VarDecls</span></span> = &lt;&lt;{<a href="../../classes/MethodDeclarations.sdf3#VariableModifier_462_478" id="VariableModifier_965_981" title="Defined at ../../classes/MethodDeclarations.sdf3 line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#UnannType_403_412" id="UnannType_990_999" title="Defined at ../../classes/FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="../../classes/FieldDeclarations.sdf3#VarDecl_355_362" id="VarDecl_1003_1010" title="Defined at ../../classes/FieldDeclarations.sdf3 line 19, 33, 34">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#ForUpdate_789_798" id="ForUpdate_1025_1034" title="Referenced at line 41">ForUpdate</a> = <a href="#Exprs_311_316" id="Exprs_1037_1042" title="Defined at line 19, 49">Exprs</a>
  
  <a href="#Exprs_1037_1042" id="Exprs_1048_1053" title="Referenced at line 47">Exprs</a>.<span class="cons_Constructor"><span id="ExprList_1054_1062" title="Not referenced locally, nor via imports">ExprList</span></span> =  &lt;&lt;{<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1069_1079" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a> <span class="cons_Lit">", "</span>}*&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_1094_1103" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a> = <a href="../Blocks.sdf3#Block_185_190" id="Block_1106_1111" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>
  
  <a href="#Statement_3401_3410" id="Statement_1117_1126" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Empty_1127_1132" title="Not referenced locally, nor via imports">Empty</span></span> = <span class="cons_Lit">";"</span>
  
  <a href="#Statement_3401_3410" id="Statement_1144_1153" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="ExpressionStatement_1154_1173" title="Not referenced locally, nor via imports">ExpressionStatement</span></span> = &lt;&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1178_1188" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_1197_1206" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a> = <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1209_1223" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1228_1242" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&gt;"</span> <a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1247_1257" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a> <span class="cons_Lit">";"</span> {<span class="keyword">reject</span>}
  <a href="#Statement_3401_3410" id="Statement_1273_1282" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a> = <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1285_1299" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1304_1318" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1323_1337" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&gt;&gt;"</span> <a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1343_1353" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a> <span class="cons_Lit">";"</span> {<span class="keyword">reject</span>} 
  <a href="#Statement_3401_3410" id="Statement_1370_1379" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a> = <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1382_1396" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1401_1415" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1420_1434" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_1439_1453" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a> <span class="cons_Lit">"&gt;&gt;&gt;"</span> <a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1460_1470" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a> <span class="cons_Lit">";"</span> {<span class="keyword">reject</span>} 
  
  <a href="#Statement_3401_3410" id="Statement_1490_1499" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Assert_1500_1506" title="Not referenced locally, nor via imports">Assert</span></span> = &lt;<span class="cons_String">assert</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1518_1528" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  <a href="#Statement_3401_3410" id="Statement_1534_1543" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Assert_1544_1550" title="Not referenced locally, nor via imports">Assert</span></span> = &lt;<span class="cons_String">assert</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1562_1572" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt; <span class="cons_String">:</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1577_1587" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_1596_1605" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Switch_1606_1612" title="Not referenced locally, nor via imports">Switch</span></span> = &lt;
  <span class="cons_String">switch(</span>&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1627_1637" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">)</span> <span class="cons_String">{</span>
    &lt;{<a href="#SwitchGroup_319_330" id="SwitchGroup_1648_1659" title="Defined at line 20, 70">SwitchGroup</a> <span class="cons_Lit">"\n"</span>}*&gt;
    &lt;{<a href="#SwitchLabel_333_344" id="SwitchLabel_1674_1685" title="Defined at line 21, 75, 77">SwitchLabel</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#SwitchGroup_1648_1659" id="SwitchGroup_1704_1715" title="Referenced at line 66">SwitchGroup</a>.<span class="cons_Constructor"><span id="SwitchGroup_1716_1727" title="Not referenced locally, nor via imports">SwitchGroup</span></span> = &lt;
  &lt;{<a href="#SwitchLabel_333_344" id="SwitchLabel_1736_1747" title="Defined at line 21, 75, 77">SwitchLabel</a> <span class="cons_Lit">"\n"</span>}+&gt;
  &lt;{<a href="../Blocks.sdf3#BlockStatement_193_207" id="BlockStatement_1760_1774" title="Defined at ../Blocks.sdf3 line 13, 21, 22, 23">BlockStatement</a> <span class="cons_Lit">"\n"</span>}+&gt;
  &gt;
  
  <a href="#SwitchLabel_1736_1747" id="SwitchLabel_1792_1803" title="Referenced at line 71">SwitchLabel</a>.<span class="cons_Constructor"><span id="CaseExpr_1804_1812" title="Not referenced locally, nor via imports">CaseExpr</span></span>     = &lt;<span class="cons_String">case</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1826_1836" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt; <span class="cons_String">:</span>&gt;
<span class="layout">//  SwitchLabel.CaseEnumName = &lt;case &lt;Id&gt; :&gt;</span>
  <a href="#SwitchLabel_1736_1747" id="SwitchLabel_1888_1899" title="Referenced at line 71">SwitchLabel</a>.<span class="cons_Constructor"><span id="DefaultCase_1900_1911" title="Not referenced locally, nor via imports">DefaultCase</span></span>  = &lt;<span class="cons_String">default</span> <span class="cons_String">:</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_1932_1941" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="DoWhile_1942_1949" title="Not referenced locally, nor via imports">DoWhile</span></span> = &lt;
  <span class="cons_String">do</span> &lt;<a href="#Statement_277_286" id="Statement_1960_1969" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>&gt;
  <span class="cons_String">while(</span>&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_1980_1990" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">);</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2000_2009" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Break_2010_2015" title="Not referenced locally, nor via imports">Break</span></span> = &lt;<span class="cons_String">break;</span>&gt;
  <a href="#Statement_3401_3410" id="Statement_2029_2038" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Break_2039_2044" title="Not referenced locally, nor via imports">Break</span></span> = &lt;<span class="cons_String">break</span> &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_2055_2057" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2066_2075" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Continue_2076_2084" title="Not referenced locally, nor via imports">Continue</span></span> = &lt;<span class="cons_String">continue;</span>&gt;
  <a href="#Statement_3401_3410" id="Statement_2101_2110" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Continue_2111_2119" title="Not referenced locally, nor via imports">Continue</span></span> = &lt;<span class="cons_String">continue</span> &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_2133_2135" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2144_2153" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Return_2154_2160" title="Not referenced locally, nor via imports">Return</span></span> = &lt;<span class="cons_String">return;</span>&gt;
  <a href="#Statement_3401_3410" id="Statement_2175_2184" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Return_2185_2191" title="Not referenced locally, nor via imports">Return</span></span> = &lt;<span class="cons_String">return</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_2203_2213" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2222_2231" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Synchronized_2232_2244" title="Not referenced locally, nor via imports">Synchronized</span></span> = &lt;<span class="cons_String">synchronized(</span>&lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_2262_2272" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2276_2281" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2289_2298" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Throw_2299_2304" title="Not referenced locally, nor via imports">Throw</span></span> = &lt;<span class="cons_String">throw</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_2315_2325" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2334_2343" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="Try_2344_2347" title="Not referenced locally, nor via imports">Try</span></span> = &lt;
  <span class="cons_String">try</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2359_2364" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;
  &lt;{<a href="#CatchClause_347_358" id="CatchClause_2370_2381" title="Defined at line 22, 105">CatchClause</a> <span class="cons_Lit">"\n"</span>}+&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2396_2405" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="TryFinally_2406_2416" title="Not referenced locally, nor via imports">TryFinally</span></span> = &lt;
  <span class="cons_String">try</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2428_2433" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;
  &lt;{<a href="#CatchClause_347_358" id="CatchClause_2439_2450" title="Defined at line 22, 105">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">finally</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2470_2475" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;&gt;
  
  <a href="#CatchClause_3150_3161" id="CatchClause_2483_2494" title="Referenced at line 125">CatchClause</a>.<span class="cons_Constructor"><span id="Catch_2495_2500" title="Not referenced locally, nor via imports">Catch</span></span> = &lt;<span class="cons_String">catch(</span>&lt;<a href="#CatchFormalParameter_361_381" id="CatchFormalParameter_2511_2531" title="Defined at line 23, 106">CatchFormalParameter</a>&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2535_2540" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;&gt;
  <a href="#CatchFormalParameter_2511_2531" id="CatchFormalParameter_2545_2565" title="Referenced at line 105">CatchFormalParameter</a>.<span class="cons_Constructor"><span id="CatchParam_2566_2576" title="Not referenced locally, nor via imports">CatchParam</span></span> = &lt;&lt;{<a href="../../classes/MethodDeclarations.sdf3#VariableModifier_462_478" id="VariableModifier_2582_2598" title="Defined at ../../classes/MethodDeclarations.sdf3 line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#CatchType_384_393" id="CatchType_2607_2616" title="Defined at line 24, 107">CatchType</a>&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#VarDeclId_343_352" id="VarDeclId_2619_2628" title="Defined at ../../classes/FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt;&gt;
  <a href="#CatchType_2607_2616" id="CatchType_2633_2642" title="Referenced at line 106">CatchType</a>.<span class="cons_Constructor"><span id="CatchType_2643_2652" title="Not referenced locally, nor via imports">CatchType</span></span> = &lt;&lt;<a href="../../classes/FieldDeclarations.sdf3#UnannClassType_457_471" id="UnannClassType_2657_2671" title="Defined at ../../classes/FieldDeclarations.sdf3 line 25, 59, 60">UnannClassType</a>&gt; &lt;{<a href="#CatchTypeRest_396_409" id="CatchTypeRest_2675_2688" title="Defined at line 25, 108">CatchTypeRest</a> <span class="cons_Lit">" "</span>}*&gt;&gt;
  <a href="#CatchTypeRest_2675_2688" id="CatchTypeRest_2699_2712" title="Referenced at line 107">CatchTypeRest</a>.<span class="cons_Constructor"><span id="CatchTypeElem_2713_2726" title="Not referenced locally, nor via imports">CatchTypeElem</span></span> = &lt;<span class="cons_String">|</span> &lt;<a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_2733_2742" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2750_2759" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="TryWithResources_2760_2776" title="Not referenced locally, nor via imports">TryWithResources</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_412_420" id="Resource_2790_2798" title="Defined at line 26, 128">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2809_2814" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt; 
  &lt;{<a href="#CatchClause_347_358" id="CatchClause_2821_2832" title="Defined at line 22, 105">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2847_2856" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="TryWithResourcesSemiColon_2857_2882" title="Not referenced locally, nor via imports">TryWithResourcesSemiColon</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_412_420" id="Resource_2896_2904" title="Defined at line 26, 128">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">;)</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_2916_2921" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt; 
  &lt;{<a href="#CatchClause_347_358" id="CatchClause_2928_2939" title="Defined at line 22, 105">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_2954_2963" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="TryWithResources_2964_2980" title="Not referenced locally, nor via imports">TryWithResources</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_412_420" id="Resource_2994_3002" title="Defined at line 26, 128">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_3013_3018" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt; 
  &lt;{<a href="#CatchClause_347_358" id="CatchClause_3025_3036" title="Defined at line 22, 105">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">finally</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_3056_3061" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;&gt;
  
  <a href="#Statement_3401_3410" id="Statement_3069_3078" title="Referenced at line 136; ../Blocks.sdf3 line 23">Statement</a>.<span class="cons_Constructor"><span id="TryWithResourcesSemiColon_3079_3104" title="Not referenced locally, nor via imports">TryWithResourcesSemiColon</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_412_420" id="Resource_3118_3126" title="Defined at line 26, 128">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">;)</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_3138_3143" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt; 
  &lt;{<a href="#CatchClause_347_358" id="CatchClause_3150_3161" title="Defined at line 22, 105">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">finally</span> &lt;<a href="../Blocks.sdf3#Block_185_190" id="Block_3181_3186" title="Defined at ../Blocks.sdf3 line 12, 17">Block</a>&gt;&gt;
  
  <a href="#Resource_3118_3126" id="Resource_3194_3202" title="Referenced at line 124">Resource</a>.<span class="cons_Constructor"><span id="Resource_3203_3211" title="Not referenced locally, nor via imports">Resource</span></span> = &lt;&lt;{<a href="../../classes/MethodDeclarations.sdf3#VariableModifier_462_478" id="VariableModifier_3217_3233" title="Defined at ../../classes/MethodDeclarations.sdf3 line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#UnannType_403_412" id="UnannType_3242_3251" title="Defined at ../../classes/FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3#VarDeclId_343_352" id="VarDeclId_3254_3263" title="Defined at ../../classes/FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt; <span class="cons_String">=</span> &lt;<a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_3268_3278" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>&gt;&gt;
    
<span class="keyword">template options</span>
  <span class="keyword">tokenize</span> : "(;"
    
<span class="layout">// new SDF3 table generator</span>
<span class="keyword">context-free priorities</span>

  <a href="#Statement_277_286" id="Statement_3381_3390" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>.<span class="cons_Constructor"><a href="#IfElse_617_623" id="IfElse_3391_3397" title="Defined at line 37">IfElse</a></span>  &gt; <a href="#Statement_277_286" id="Statement_3401_3410" title="Defined at line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>.<span class="cons_Constructor"><a href="#If_564_566" id="If_3411_3413" title="Defined at line 36">If</a></span>
</code></pre></td></tr></tbody></table></div>