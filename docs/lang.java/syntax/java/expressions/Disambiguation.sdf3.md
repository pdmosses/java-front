---
title: Disambiguation.sdf3
hide:
  - toc
---

# `Disambiguation.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/Disambiguation.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/Disambiguation.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/Disambiguation.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../Main.sdf3/#java/expressions/Disambiguation_17_3" id="java/expressions/Disambiguation_1_8" title="Referenced at ../../Main.sdf3 line 17">java/expressions/Disambiguation</a>

<span class="keyword">imports</span>
  <a href="../ClassInstanceCreation.sdf3/#java/expressions/ClassInstanceCreation_1_8" id="java/expressions/ClassInstanceCreation_4_3" title="Defined at ../ClassInstanceCreation.sdf3 line 1">java/expressions/ClassInstanceCreation</a>
  <a href="../Postfix.sdf3/#java/expressions/Postfix_1_8" id="java/expressions/Postfix_5_3" title="Defined at ../Postfix.sdf3 line 1">java/expressions/Postfix</a>
  <a href="../UnaryOperators.sdf3/#java/expressions/UnaryOperators_1_8" id="java/expressions/UnaryOperators_6_3" title="Defined at ../UnaryOperators.sdf3 line 1">java/expressions/UnaryOperators</a>
  <a href="../BinaryOperators.sdf3/#java/expressions/BinaryOperators_1_8" id="java/expressions/BinaryOperators_7_3" title="Defined at ../BinaryOperators.sdf3 line 1">java/expressions/BinaryOperators</a>
  <a href="../ArrayAccess.sdf3/#java/expressions/ArrayAccess_1_8" id="java/expressions/ArrayAccess_8_3" title="Defined at ../ArrayAccess.sdf3 line 1">java/expressions/ArrayAccess</a>
  <a href="../FieldAccess.sdf3/#java/expressions/FieldAccess_1_8" id="java/expressions/FieldAccess_9_3" title="Defined at ../FieldAccess.sdf3 line 1">java/expressions/FieldAccess</a>
  <a href="../MethodInvocation.sdf3/#java/expressions/MethodInvocation_1_8" id="java/expressions/MethodInvocation_10_3" title="Defined at ../MethodInvocation.sdf3 line 1">java/expressions/MethodInvocation</a>
  <a href="../AssignmentOperators.sdf3/#java/expressions/AssignmentOperators_1_8" id="java/expressions/AssignmentOperators_11_3" title="Defined at ../AssignmentOperators.sdf3 line 1">java/expressions/AssignmentOperators</a>
  <a href="../LambdaExpressions.sdf3/#java/expressions/LambdaExpressions_1_8" id="java/expressions/LambdaExpressions_12_3" title="Defined at ../LambdaExpressions.sdf3 line 1">java/expressions/LambdaExpressions</a>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_13_3" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  
<span class="keyword">context-free priorities</span>

  <a href="../FieldAccess.sdf3/#FieldAccess_12_3" id="FieldAccess_17_3" title="Defined at ../FieldAccess.sdf3 line 12, 18, 19, 20">FieldAccess</a>.<span class="cons_Constructor"><a href="../FieldAccess.sdf3/#Field_18_15" id="Field_17_15" title="Defined at ../FieldAccess.sdf3 line 18">Field</a></span> &gt; 
  <a href="#Expression_20_18" id="Expression_18_3" title="Referenced at line 20, 21, 25, 27, 28, 30, 31, 35, 37, 38, 39, 43, 44, 45, 46, 47, 49, 50, 51, 58, 60, 61, 62, 63, 64, 65, 66, 67, 69, 70, 71, 73, 74, 76, 77, 78, 80, 81, 82, 83, 84, 86, 87, 88, 89, 90, 91, 92, 93, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107">Expression</a> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_18_16" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>,
  
  <span id="ElementValue_20_3" title="Not referenced">ElementValue</span> = <a href="#Expression_18_3" id="Expression_20_18" title="Defined at line 18">Expression</a> &lt;0&gt; &gt;
  <a href="#Expression_18_3" id="Expression_21_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#Assign_16_14" id="Assign_21_14" title="Defined at ../AssignmentOperators.sdf3 line 16">Assign</a></span>  

<span class="keyword">context-free priorities</span>

  <a href="#Expression_18_3" id="Expression_25_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../ClassInstanceCreation.sdf3/#QualifiedInstance_21_14" id="QualifiedInstance_25_14" title="Defined at ../ClassInstanceCreation.sdf3 line 21">QualifiedInstance</a></span> &gt; 
  {<span class="keyword">right</span>: 
    <a href="#Expression_18_3" id="Expression_27_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3/#PostIncr_11_14" id="PostIncr_27_16" title="Defined at ../Postfix.sdf3 line 11">PostIncr</a></span> 
    <a href="#Expression_18_3" id="Expression_28_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3/#PostDecr_12_14" id="PostDecr_28_16" title="Defined at ../Postfix.sdf3 line 12">PostDecr</a></span> } &gt;
  { 
    <a href="#Expression_18_3" id="Expression_30_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#CastPrimitive_22_14" id="CastPrimitive_30_16" title="Defined at ../UnaryOperators.sdf3 line 22">CastPrimitive</a></span> 
    <a href="#Expression_18_3" id="Expression_31_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#CastReference_23_14" id="CastReference_31_16" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span> }

<span class="keyword">context-free priorities</span>
  
  <a href="#Expression_18_3" id="Expression_35_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#CastPrimitive_22_14" id="CastPrimitive_35_14" title="Defined at ../UnaryOperators.sdf3 line 22">CastPrimitive</a></span> &gt; 
  {<span class="keyword">left</span>: 
    <a href="#Expression_18_3" id="Expression_37_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Mul_17_14" id="Mul_37_16" title="Defined at ../BinaryOperators.sdf3 line 17">Mul</a></span> 
    <a href="#Expression_18_3" id="Expression_38_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Div_18_14" id="Div_38_16" title="Defined at ../BinaryOperators.sdf3 line 18">Div</a></span>
    <a href="#Expression_18_3" id="Expression_39_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Mod_19_14" id="Mod_39_16" title="Defined at ../BinaryOperators.sdf3 line 19">Mod</a></span> }
  
<span class="keyword">context-free priorities</span>
  
  <a href="#Expression_18_3" id="Expression_43_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#CastReference_23_14" id="CastReference_43_14" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span> &gt; 
  { <a href="#Expression_18_3" id="Expression_44_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#PreIncr_18_14" id="PreIncr_44_16" title="Defined at ../UnaryOperators.sdf3 line 18">PreIncr</a></span>
    <a href="#Expression_18_3" id="Expression_45_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#PreDecr_19_14" id="PreDecr_45_16" title="Defined at ../UnaryOperators.sdf3 line 19">PreDecr</a></span>
    <a href="#Expression_18_3" id="Expression_46_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Plus_16_14" id="Plus_46_16" title="Defined at ../UnaryOperators.sdf3 line 16">Plus</a></span>
    <a href="#Expression_18_3" id="Expression_47_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Minus_17_14" id="Minus_47_16" title="Defined at ../UnaryOperators.sdf3 line 17">Minus</a></span> }
  ,
  <a href="#Expression_18_3" id="Expression_49_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#CastReference_23_14" id="CastReference_49_14" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span> &lt;4&gt; .&gt; 
  { <a href="#Expression_18_3" id="Expression_50_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Plus_16_14" id="Plus_50_16" title="Defined at ../UnaryOperators.sdf3 line 16">Plus</a></span>
    <a href="#Expression_18_3" id="Expression_51_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Minus_17_14" id="Minus_51_16" title="Defined at ../UnaryOperators.sdf3 line 17">Minus</a></span> }   
    
 
<span class="keyword">context-free priorities</span>
  
  { <a href="../ArrayAccess.sdf3/#ArrayAccess_11_3" id="ArrayAccess_56_5" title="Defined at ../ArrayAccess.sdf3 line 11, 17">ArrayAccess</a>.<span class="cons_Constructor"><a href="../ArrayAccess.sdf3/#ArrayAccess_17_15" id="ArrayAccess_56_17" title="Defined at ../ArrayAccess.sdf3 line 17">ArrayAccess</a></span> 
    <a href="../FieldAccess.sdf3/#FieldAccess_12_3" id="FieldAccess_57_5" title="Defined at ../FieldAccess.sdf3 line 12, 18, 19, 20">FieldAccess</a>.<span class="cons_Constructor"><a href="../FieldAccess.sdf3/#Field_18_15" id="Field_57_17" title="Defined at ../FieldAccess.sdf3 line 18">Field</a></span> 
    <a href="#Expression_18_3" id="Expression_58_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../MethodInvocation.sdf3/#InvokeQExp_16_14" id="InvokeQExp_58_16" title="Defined at ../MethodInvocation.sdf3 line 16">InvokeQExp</a></span> } &lt;0&gt; &gt;
  {<span class="keyword">right</span>: 
    <a href="#Expression_18_3" id="Expression_60_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3/#PostIncr_11_14" id="PostIncr_60_16" title="Defined at ../Postfix.sdf3 line 11">PostIncr</a></span> 
    <a href="#Expression_18_3" id="Expression_61_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3/#PostDecr_12_14" id="PostDecr_61_16" title="Defined at ../Postfix.sdf3 line 12">PostDecr</a></span> } &gt;
  { <a href="#Expression_18_3" id="Expression_62_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#PreIncr_18_14" id="PreIncr_62_16" title="Defined at ../UnaryOperators.sdf3 line 18">PreIncr</a></span> 
    <a href="#Expression_18_3" id="Expression_63_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#PreDecr_19_14" id="PreDecr_63_16" title="Defined at ../UnaryOperators.sdf3 line 19">PreDecr</a></span> 
    <a href="#Expression_18_3" id="Expression_64_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Plus_16_14" id="Plus_64_16" title="Defined at ../UnaryOperators.sdf3 line 16">Plus</a></span> 
    <a href="#Expression_18_3" id="Expression_65_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Minus_17_14" id="Minus_65_16" title="Defined at ../UnaryOperators.sdf3 line 17">Minus</a></span> 
    <a href="#Expression_18_3" id="Expression_66_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Complement_20_14" id="Complement_66_16" title="Defined at ../UnaryOperators.sdf3 line 20">Complement</a></span> 
    <a href="#Expression_18_3" id="Expression_67_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#Not_21_14" id="Not_67_16" title="Defined at ../UnaryOperators.sdf3 line 21">Not</a></span> } &gt;
  {<span class="keyword">left</span>:
     <a href="#Expression_18_3" id="Expression_69_6" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Mul_17_14" id="Mul_69_17" title="Defined at ../BinaryOperators.sdf3 line 17">Mul</a></span> 
     <a href="#Expression_18_3" id="Expression_70_6" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Div_18_14" id="Div_70_17" title="Defined at ../BinaryOperators.sdf3 line 18">Div</a></span> 
     <a href="#Expression_18_3" id="Expression_71_6" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Mod_19_14" id="Mod_71_17" title="Defined at ../BinaryOperators.sdf3 line 19">Mod</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_18_3" id="Expression_73_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Add_21_14" id="Add_73_16" title="Defined at ../BinaryOperators.sdf3 line 21">Add</a></span> 
    <a href="#Expression_18_3" id="Expression_74_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Sub_22_14" id="Sub_74_16" title="Defined at ../BinaryOperators.sdf3 line 22">Sub</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_18_3" id="Expression_76_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#LeftShift_24_14" id="LeftShift_76_16" title="Defined at ../BinaryOperators.sdf3 line 24">LeftShift</a></span> 
    <a href="#Expression_18_3" id="Expression_77_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#RightShift_25_14" id="RightShift_77_16" title="Defined at ../BinaryOperators.sdf3 line 25">RightShift</a></span> 
    <a href="#Expression_18_3" id="Expression_78_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#URightShift_26_14" id="URightShift_78_16" title="Defined at ../BinaryOperators.sdf3 line 26">URightShift</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_18_3" id="Expression_80_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#InstanceOf_32_14" id="InstanceOf_80_16" title="Defined at ../BinaryOperators.sdf3 line 32">InstanceOf</a></span> 
    <a href="#Expression_18_3" id="Expression_81_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Lt_28_14" id="Lt_81_16" title="Defined at ../BinaryOperators.sdf3 line 28">Lt</a></span> 
    <a href="#Expression_18_3" id="Expression_82_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Gt_29_14" id="Gt_82_16" title="Defined at ../BinaryOperators.sdf3 line 29">Gt</a></span> 
    <a href="#Expression_18_3" id="Expression_83_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#LtEq_30_14" id="LtEq_83_16" title="Defined at ../BinaryOperators.sdf3 line 30">LtEq</a></span> 
    <a href="#Expression_18_3" id="Expression_84_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#GtEq_31_14" id="GtEq_84_16" title="Defined at ../BinaryOperators.sdf3 line 31">GtEq</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_18_3" id="Expression_86_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Eq_34_14" id="Eq_86_16" title="Defined at ../BinaryOperators.sdf3 line 34">Eq</a></span> 
    <a href="#Expression_18_3" id="Expression_87_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#NotEq_35_14" id="NotEq_87_16" title="Defined at ../BinaryOperators.sdf3 line 35">NotEq</a></span> } &gt;
  <a href="#Expression_18_3" id="Expression_88_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#And_37_14" id="And_88_14" title="Defined at ../BinaryOperators.sdf3 line 37">And</a></span> &gt;
  <a href="#Expression_18_3" id="Expression_89_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Xor_38_14" id="Xor_89_14" title="Defined at ../BinaryOperators.sdf3 line 38">Xor</a></span> &gt;
  <a href="#Expression_18_3" id="Expression_90_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Or_39_14" id="Or_90_14" title="Defined at ../BinaryOperators.sdf3 line 39">Or</a></span> &gt;
  <a href="#Expression_18_3" id="Expression_91_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#LazyAnd_41_14" id="LazyAnd_91_14" title="Defined at ../BinaryOperators.sdf3 line 41">LazyAnd</a></span> &gt;
  <a href="#Expression_18_3" id="Expression_92_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#LazyOr_42_14" id="LazyOr_92_14" title="Defined at ../BinaryOperators.sdf3 line 42">LazyOr</a></span> &gt;
  <a href="#Expression_18_3" id="Expression_93_3" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3/#Cond_44_14" id="Cond_93_14" title="Defined at ../BinaryOperators.sdf3 line 44">Cond</a></span> &gt;
  {<span class="keyword">right</span>: 
    <a href="#Expression_18_3" id="Expression_95_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#Assign_16_14" id="Assign_95_16" title="Defined at ../AssignmentOperators.sdf3 line 16">Assign</a></span>
    <a href="#Expression_18_3" id="Expression_96_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignMul_17_14" id="AssignMul_96_16" title="Defined at ../AssignmentOperators.sdf3 line 17">AssignMul</a></span>
    <a href="#Expression_18_3" id="Expression_97_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignDiv_18_14" id="AssignDiv_97_16" title="Defined at ../AssignmentOperators.sdf3 line 18">AssignDiv</a></span>
    <a href="#Expression_18_3" id="Expression_98_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignMod_19_14" id="AssignMod_98_16" title="Defined at ../AssignmentOperators.sdf3 line 19">AssignMod</a></span>
    <a href="#Expression_18_3" id="Expression_99_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignAdd_20_14" id="AssignAdd_99_16" title="Defined at ../AssignmentOperators.sdf3 line 20">AssignAdd</a></span>
    <a href="#Expression_18_3" id="Expression_100_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignSub_21_14" id="AssignSub_100_16" title="Defined at ../AssignmentOperators.sdf3 line 21">AssignSub</a></span>
    <a href="#Expression_18_3" id="Expression_101_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignLeftShift_22_14" id="AssignLeftShift_101_16" title="Defined at ../AssignmentOperators.sdf3 line 22">AssignLeftShift</a></span>
    <a href="#Expression_18_3" id="Expression_102_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignRightShift_23_14" id="AssignRightShift_102_16" title="Defined at ../AssignmentOperators.sdf3 line 23">AssignRightShift</a></span>
    <a href="#Expression_18_3" id="Expression_103_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignURightShift_24_14" id="AssignURightShift_103_16" title="Defined at ../AssignmentOperators.sdf3 line 24">AssignURightShift</a></span>
    <a href="#Expression_18_3" id="Expression_104_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignAnd_25_14" id="AssignAnd_104_16" title="Defined at ../AssignmentOperators.sdf3 line 25">AssignAnd</a></span>
    <a href="#Expression_18_3" id="Expression_105_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignXor_26_14" id="AssignXor_105_16" title="Defined at ../AssignmentOperators.sdf3 line 26">AssignXor</a></span>
    <a href="#Expression_18_3" id="Expression_106_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3/#AssignOr_27_14" id="AssignOr_106_16" title="Defined at ../AssignmentOperators.sdf3 line 27">AssignOr</a></span>
    <a href="#Expression_18_3" id="Expression_107_5" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../LambdaExpressions.sdf3/#LambdaExpression_16_14" id="LambdaExpression_107_16" title="Defined at ../LambdaExpressions.sdf3 line 16">LambdaExpression</a></span> }

<span class="keyword">lexical restrictions</span>

  <span class="cons_Lit">"+"</span> -/- [\+]
  <span class="cons_Lit">"-"</span> -/- [\-]
  <span class="cons_Lit">"/"</span> -/- [\/]

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
