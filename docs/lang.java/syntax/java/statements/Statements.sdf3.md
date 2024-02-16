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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/statements/Statements_1_8" title="a definition with multiple references" data-urls="../Blocks.sdf3/#java/statements/Statements line 8_3; ../Main.sdf3/#java/statements/Statements line 8_3">java/statements/Statements</button>

<span class="layout">// 14.5. Statements</span>

<span class="keyword">imports</span>
  <a href="../../classes/FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_6_3" title="a reference to a single-file definition">java/classes/FieldDeclarations</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_1_8" id="java/classes/MethodDeclarations_7_3" title="a reference to a single-file definition">java/classes/MethodDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_8_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../Blocks.sdf3/#java/statements/Blocks_1_8" id="java/statements/Blocks_9_3" title="a reference to a single-file definition">java/statements/Blocks</a>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_10_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_11_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_12_3" title="a reference to a single-file definition">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Statement_16_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>
  <a href="#ForInit_41_29" id="ForInit_17_3" title="a definition with a single reference">ForInit</a>
  <a href="#ForUpdate_41_55" id="ForUpdate_18_3" title="a definition with a single reference">ForUpdate</a>
  <button class="modal-open" id="Exprs_19_3" title="a definition with multiple references" data-urls="#Exprs line 44_13, 47_15">Exprs</button>
  <a href="#SwitchGroup_66_7" id="SwitchGroup_20_3" title="a definition with a single reference">SwitchGroup</a>
  <button class="modal-open" id="SwitchLabel_21_3" title="a definition with multiple references" data-urls="#SwitchLabel line 67_7, 71_5">SwitchLabel</button>
  <button class="modal-open" id="CatchClause_22_3" title="a definition with multiple references" data-urls="#CatchClause line 98_5, 102_5, 112_5, 116_5, 120_5, 125_5">CatchClause</button>
  <a href="#CatchFormalParameter_105_31" id="CatchFormalParameter_23_3" title="a definition with a single reference">CatchFormalParameter</a>
  <a href="#CatchType_106_65" id="CatchType_24_3" title="a definition with a single reference">CatchType</a>
  <a href="#CatchTypeRest_107_45" id="CatchTypeRest_25_3" title="a definition with a single reference">CatchTypeRest</a>
  <button class="modal-open" id="Resource_26_3" title="a definition with multiple references" data-urls="#Resource line 111_10, 115_10, 119_10, 124_10">Resource</button>
    
<span class="keyword">context-free priorities</span>

  <a href="#Statement_16_3" id="Statement_30_3" title="a reference to a single-file definition">Statement</a>.<span class="cons_Constructor"><a href="#IfElse_37_13" id="IfElse_30_13" title="a reference to a single-file definition">IfElse</a></span>  &gt; <a href="#Statement_16_3" id="Statement_30_23" title="a reference to a single-file definition">Statement</a>.<span class="cons_Constructor"><a href="#If_36_13" id="If_30_33" title="a reference to a single-file definition">If</a></span>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Statement_34_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Labeled_34_13" title="a definition with no references">Labeled</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_34_25" title="a reference to a single-file definition">Id</a>&gt; <span class="cons_String">:</span> &lt;<a href="#Statement_16_3" id="Statement_34_32" title="a reference to a single-file definition">Statement</a>&gt;&gt;

  <button class="modal-open" id="Statement_36_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><button class="modal-open" id="If_36_13" title="a definition with multiple references" data-urls="#If line 30_33, 136_33">If</button></span>      = &lt;<span class="cons_String">if(</span>&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_36_28" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_16_3" id="Statement_36_42" title="a reference to a single-file definition">Statement</a>&gt;&gt;
  <button class="modal-open" id="Statement_37_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><button class="modal-open" id="IfElse_37_13" title="a definition with multiple references" data-urls="#IfElse line 30_13, 136_13">IfElse</button></span>  = &lt;<span class="cons_String">if(</span>&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_37_28" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_16_3" id="Statement_37_42" title="a reference to a single-file definition">Statement</a>&gt; <span class="cons_String">else</span> &lt;<a href="#Statement_16_3" id="Statement_37_59" title="a reference to a single-file definition">Statement</a>&gt;&gt;
  
  <button class="modal-open" id="Statement_39_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="While_39_13" title="a definition with no references">While</span></span> = &lt;<span class="cons_String">while(</span>&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_39_29" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_16_3" id="Statement_39_43" title="a reference to a single-file definition">Statement</a>&gt;&gt;
  
  <button class="modal-open" id="Statement_41_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="For_41_13" title="a definition with no references">For</span></span>     = &lt;<span class="cons_String">for(</span>&lt;<a href="#ForInit_17_3" id="ForInit_41_29" title="a reference to a single-file definition">ForInit</a>&gt;<span class="cons_String">;</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_41_40" title="a reference to a single-file definition">Expression</a>?&gt;<span class="cons_String">;</span> &lt;<a href="#ForUpdate_18_3" id="ForUpdate_41_55" title="a reference to a single-file definition">ForUpdate</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_16_3" id="Statement_41_68" title="a reference to a single-file definition">Statement</a>&gt;&gt;
  <button class="modal-open" id="Statement_42_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="ForEach_42_13" title="a definition with no references">ForEach</span></span> = &lt;<span class="cons_String">for(</span>&lt;{<a href="../../classes/MethodDeclarations.sdf3/#VariableModifier_26_3" id="VariableModifier_42_30" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_42_55" title="a reference to a single-file definition">UnannType</a>&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_42_67" title="a reference to a single-file definition">VarDeclId</a>&gt; <span class="cons_String">:</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_42_81" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Statement_16_3" id="Statement_42_95" title="a reference to a single-file definition">Statement</a>&gt;&gt;
  
  <a href="#ForInit_41_29" id="ForInit_44_3" title="a definition with a single reference">ForInit</a> = <a href="#Exprs_19_3" id="Exprs_44_13" title="a reference to a single-file definition">Exprs</a>
  <a href="#ForInit_41_29" id="ForInit_45_3" title="a definition with a single reference">ForInit</a>.<span class="cons_Constructor"><span id="VarDecls_45_11" title="a definition with no references">VarDecls</span></span> = &lt;&lt;{<a href="../../classes/MethodDeclarations.sdf3/#VariableModifier_26_3" id="VariableModifier_45_25" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_45_50" title="a reference to a single-file definition">UnannType</a>&gt; &lt;{<a href="../../classes/FieldDeclarations.sdf3/#VarDecl_19_3" id="VarDecl_45_63" title="a reference to a single-file definition">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#ForUpdate_41_55" id="ForUpdate_47_3" title="a definition with a single reference">ForUpdate</a> = <a href="#Exprs_19_3" id="Exprs_47_15" title="a reference to a single-file definition">Exprs</a>
  
  <button class="modal-open" id="Exprs_49_3" title="a definition with multiple references" data-urls="#Exprs line 44_13, 47_15">Exprs</button>.<span class="cons_Constructor"><span id="ExprList_49_9" title="a definition with no references">ExprList</span></span> =  &lt;&lt;{<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_49_24" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">", "</span>}*&gt;&gt;
  
  <button class="modal-open" id="Statement_51_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button> = <a href="../Blocks.sdf3/#Block_12_3" id="Block_51_15" title="a reference to a single-file definition">Block</a>
  
  <button class="modal-open" id="Statement_53_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Empty_53_13" title="a definition with no references">Empty</span></span> = <span class="cons_Lit">";"</span>
  
  <button class="modal-open" id="Statement_55_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="ExpressionStatement_55_13" title="a definition with no references">ExpressionStatement</span></span> = &lt;&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_55_37" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <button class="modal-open" id="Statement_57_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_57_15" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_57_34" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&gt;"</span> <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_57_53" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">";"</span> {<span class="keyword">reject</span>}
  <button class="modal-open" id="Statement_58_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_58_15" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_58_34" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_58_53" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&gt;&gt;"</span> <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_58_73" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">";"</span> {<span class="keyword">reject</span>} 
  <button class="modal-open" id="Statement_59_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_59_15" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_59_34" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_59_53" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&lt;"</span> <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_59_72" title="a reference to a single-file definition">ExpressionName</a> <span class="cons_Lit">"&gt;&gt;&gt;"</span> <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_59_93" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">";"</span> {<span class="keyword">reject</span>} 
  
  <button class="modal-open" id="Statement_61_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Assert_61_13" title="a definition with no references">Assert</span></span> = &lt;<span class="cons_String">assert</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_61_31" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  <button class="modal-open" id="Statement_62_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Assert_62_13" title="a definition with no references">Assert</span></span> = &lt;<span class="cons_String">assert</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_62_31" title="a reference to a single-file definition">Expression</a>&gt; <span class="cons_String">:</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_62_46" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <button class="modal-open" id="Statement_64_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Switch_64_13" title="a definition with no references">Switch</span></span> = &lt;
  <span class="cons_String">switch(</span>&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_65_11" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span> <span class="cons_String">{</span>
    &lt;{<a href="#SwitchGroup_20_3" id="SwitchGroup_66_7" title="a reference to a single-file definition">SwitchGroup</a> <span class="cons_Lit">"\n"</span>}*&gt;
    &lt;{<a href="#SwitchLabel_21_3" id="SwitchLabel_67_7" title="a reference to a single-file definition">SwitchLabel</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#SwitchGroup_66_7" id="SwitchGroup_70_3" title="a definition with a single reference">SwitchGroup</a>.<span class="cons_Constructor"><span id="SwitchGroup_70_15" title="a definition with no references">SwitchGroup</span></span> = &lt;
  &lt;{<a href="#SwitchLabel_21_3" id="SwitchLabel_71_5" title="a reference to a single-file definition">SwitchLabel</a> <span class="cons_Lit">"\n"</span>}+&gt;
  &lt;{<a href="../Blocks.sdf3/#BlockStatement_13_3" id="BlockStatement_72_5" title="a reference to a single-file definition">BlockStatement</a> <span class="cons_Lit">"\n"</span>}+&gt;
  &gt;
  
  <button class="modal-open" id="SwitchLabel_75_3" title="a definition with multiple references" data-urls="#SwitchLabel line 67_7, 71_5">SwitchLabel</button>.<span class="cons_Constructor"><span id="CaseExpr_75_15" title="a definition with no references">CaseExpr</span></span>     = &lt;<span class="cons_String">case</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_75_37" title="a reference to a single-file definition">Expression</a>&gt; <span class="cons_String">:</span>&gt;
<span class="layout">//  SwitchLabel.CaseEnumName = &lt;case &lt;Id&gt; :&gt;</span>
  <button class="modal-open" id="SwitchLabel_77_3" title="a definition with multiple references" data-urls="#SwitchLabel line 67_7, 71_5">SwitchLabel</button>.<span class="cons_Constructor"><span id="DefaultCase_77_15" title="a definition with no references">DefaultCase</span></span>  = &lt;<span class="cons_String">default</span> <span class="cons_String">:</span>&gt;
  
  <button class="modal-open" id="Statement_79_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="DoWhile_79_13" title="a definition with no references">DoWhile</span></span> = &lt;
  <span class="cons_String">do</span> &lt;<a href="#Statement_16_3" id="Statement_80_7" title="a reference to a single-file definition">Statement</a>&gt;
  <span class="cons_String">while(</span>&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_81_10" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">);</span>&gt;
  
  <button class="modal-open" id="Statement_83_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Break_83_13" title="a definition with no references">Break</span></span> = &lt;<span class="cons_String">break;</span>&gt;
  <button class="modal-open" id="Statement_84_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Break_84_13" title="a definition with no references">Break</span></span> = &lt;<span class="cons_String">break</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_84_29" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">;</span>&gt;
  
  <button class="modal-open" id="Statement_86_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Continue_86_13" title="a definition with no references">Continue</span></span> = &lt;<span class="cons_String">continue;</span>&gt;
  <button class="modal-open" id="Statement_87_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Continue_87_13" title="a definition with no references">Continue</span></span> = &lt;<span class="cons_String">continue</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_87_35" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">;</span>&gt;
  
  <button class="modal-open" id="Statement_89_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Return_89_13" title="a definition with no references">Return</span></span> = &lt;<span class="cons_String">return;</span>&gt;
  <button class="modal-open" id="Statement_90_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Return_90_13" title="a definition with no references">Return</span></span> = &lt;<span class="cons_String">return</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_90_31" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <button class="modal-open" id="Statement_92_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Synchronized_92_13" title="a definition with no references">Synchronized</span></span> = &lt;<span class="cons_String">synchronized(</span>&lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_92_43" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_92_57" title="a reference to a single-file definition">Block</a>&gt;&gt;
  
  <button class="modal-open" id="Statement_94_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Throw_94_13" title="a definition with no references">Throw</span></span> = &lt;<span class="cons_String">throw</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_94_29" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">;</span>&gt;
  
  <button class="modal-open" id="Statement_96_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="Try_96_13" title="a definition with no references">Try</span></span> = &lt;
  <span class="cons_String">try</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_97_8" title="a reference to a single-file definition">Block</a>&gt;
  &lt;{<a href="#CatchClause_22_3" id="CatchClause_98_5" title="a reference to a single-file definition">CatchClause</a> <span class="cons_Lit">"\n"</span>}+&gt;&gt;
  
  <button class="modal-open" id="Statement_100_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="TryFinally_100_13" title="a definition with no references">TryFinally</span></span> = &lt;
  <span class="cons_String">try</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_101_8" title="a reference to a single-file definition">Block</a>&gt;
  &lt;{<a href="#CatchClause_22_3" id="CatchClause_102_5" title="a reference to a single-file definition">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">finally</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_103_12" title="a reference to a single-file definition">Block</a>&gt;&gt;
  
  <button class="modal-open" id="CatchClause_105_3" title="a definition with multiple references" data-urls="#CatchClause line 98_5, 102_5, 112_5, 116_5, 120_5, 125_5">CatchClause</button>.<span class="cons_Constructor"><span id="Catch_105_15" title="a definition with no references">Catch</span></span> = &lt;<span class="cons_String">catch(</span>&lt;<a href="#CatchFormalParameter_23_3" id="CatchFormalParameter_105_31" title="a reference to a single-file definition">CatchFormalParameter</a>&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_105_55" title="a reference to a single-file definition">Block</a>&gt;&gt;
  <a href="#CatchFormalParameter_105_31" id="CatchFormalParameter_106_3" title="a definition with a single reference">CatchFormalParameter</a>.<span class="cons_Constructor"><span id="CatchParam_106_24" title="a definition with no references">CatchParam</span></span> = &lt;&lt;{<a href="../../classes/MethodDeclarations.sdf3/#VariableModifier_26_3" id="VariableModifier_106_40" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#CatchType_24_3" id="CatchType_106_65" title="a reference to a single-file definition">CatchType</a>&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_106_77" title="a reference to a single-file definition">VarDeclId</a>&gt;&gt;
  <a href="#CatchType_106_65" id="CatchType_107_3" title="a definition with a single reference">CatchType</a>.<span class="cons_Constructor"><span id="CatchType_107_13" title="a definition with no references">CatchType</span></span> = &lt;&lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannClassType_25_3" id="UnannClassType_107_27" title="a reference to a single-file definition">UnannClassType</a>&gt; &lt;{<a href="#CatchTypeRest_25_3" id="CatchTypeRest_107_45" title="a reference to a single-file definition">CatchTypeRest</a> <span class="cons_Lit">" "</span>}*&gt;&gt;
  <a href="#CatchTypeRest_107_45" id="CatchTypeRest_108_3" title="a definition with a single reference">CatchTypeRest</a>.<span class="cons_Constructor"><span id="CatchTypeElem_108_17" title="a definition with no references">CatchTypeElem</span></span> = &lt;<span class="cons_String">|</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_108_37" title="a reference to a single-file definition">ClassType</a>&gt;&gt;
  
  <button class="modal-open" id="Statement_110_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="TryWithResources_110_13" title="a definition with no references">TryWithResources</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_26_3" id="Resource_111_10" title="a reference to a single-file definition">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_111_29" title="a reference to a single-file definition">Block</a>&gt; 
  &lt;{<a href="#CatchClause_22_3" id="CatchClause_112_5" title="a reference to a single-file definition">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt;
  
  <button class="modal-open" id="Statement_114_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="TryWithResourcesSemiColon_114_13" title="a definition with no references">TryWithResourcesSemiColon</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_26_3" id="Resource_115_10" title="a reference to a single-file definition">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">;)</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_115_30" title="a reference to a single-file definition">Block</a>&gt; 
  &lt;{<a href="#CatchClause_22_3" id="CatchClause_116_5" title="a reference to a single-file definition">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt;
  
  <button class="modal-open" id="Statement_118_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="TryWithResources_118_13" title="a definition with no references">TryWithResources</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_26_3" id="Resource_119_10" title="a reference to a single-file definition">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_119_29" title="a reference to a single-file definition">Block</a>&gt; 
  &lt;{<a href="#CatchClause_22_3" id="CatchClause_120_5" title="a reference to a single-file definition">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">finally</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_121_12" title="a reference to a single-file definition">Block</a>&gt;&gt;
  
  <button class="modal-open" id="Statement_123_3" title="a definition with multiple references" data-urls="#Statement line 30_3, 30_23, 34_32, 36_42, 37_42, 37_59, 39_43, 41_68, 42_95, 80_7, 136_3, 136_23; ../Blocks.sdf3/#Statement line 23_23">Statement</button>.<span class="cons_Constructor"><span id="TryWithResourcesSemiColon_123_13" title="a definition with no references">TryWithResourcesSemiColon</span></span> = &lt;
  <span class="cons_String">try</span> <span class="cons_String">(</span>&lt;{<a href="#Resource_26_3" id="Resource_124_10" title="a reference to a single-file definition">Resource</a> <span class="cons_Lit">"; "</span>}*&gt;<span class="cons_String">;)</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_124_30" title="a reference to a single-file definition">Block</a>&gt; 
  &lt;{<a href="#CatchClause_22_3" id="CatchClause_125_5" title="a reference to a single-file definition">CatchClause</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">finally</span> &lt;<a href="../Blocks.sdf3/#Block_12_3" id="Block_126_12" title="a reference to a single-file definition">Block</a>&gt;&gt;
  
  <button class="modal-open" id="Resource_128_3" title="a definition with multiple references" data-urls="#Resource line 111_10, 115_10, 119_10, 124_10">Resource</button>.<span class="cons_Constructor"><span id="Resource_128_12" title="a definition with no references">Resource</span></span> = &lt;&lt;{<a href="../../classes/MethodDeclarations.sdf3/#VariableModifier_26_3" id="VariableModifier_128_26" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_128_51" title="a reference to a single-file definition">UnannType</a>&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_128_63" title="a reference to a single-file definition">VarDeclId</a>&gt; <span class="cons_String">=</span> &lt;<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_128_77" title="a reference to a single-file definition">Expression</a>&gt;&gt;
    
<span class="keyword">template options</span>
  <span class="keyword">tokenize</span> : "(;"
    
<span class="layout">// new SDF3 table generator</span>
<span class="keyword">context-free priorities</span>

  <a href="#Statement_16_3" id="Statement_136_3" title="a reference to a single-file definition">Statement</a>.<span class="cons_Constructor"><a href="#IfElse_37_13" id="IfElse_136_13" title="a reference to a single-file definition">IfElse</a></span>  &gt; <a href="#Statement_16_3" id="Statement_136_23" title="a reference to a single-file definition">Statement</a>.<span class="cons_Constructor"><a href="#If_36_13" id="If_136_33" title="a reference to a single-file definition">If</a></span>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
