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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../Main.sdf3#java/expressions/Disambiguation_294_325" id="java/expressions/Disambiguation_7_38" title="Referenced at ../../Main.sdf3 line 17">java/expressions/Disambiguation</a>

<span class="keyword">imports</span>
  <a href="../ClassInstanceCreation.sdf3#java/expressions/ClassInstanceCreation_7_45" id="java/expressions/ClassInstanceCreation_50_88" title="Defined at ../ClassInstanceCreation.sdf3 line 1">java/expressions/ClassInstanceCreation</a>
  <a href="../Postfix.sdf3#java/expressions/Postfix_7_31" id="java/expressions/Postfix_91_115" title="Defined at ../Postfix.sdf3 line 1">java/expressions/Postfix</a>
  <a href="../UnaryOperators.sdf3#java/expressions/UnaryOperators_7_38" id="java/expressions/UnaryOperators_118_149" title="Defined at ../UnaryOperators.sdf3 line 1">java/expressions/UnaryOperators</a>
  <a href="../BinaryOperators.sdf3#java/expressions/BinaryOperators_7_39" id="java/expressions/BinaryOperators_152_184" title="Defined at ../BinaryOperators.sdf3 line 1">java/expressions/BinaryOperators</a>
  <a href="../ArrayAccess.sdf3#java/expressions/ArrayAccess_7_35" id="java/expressions/ArrayAccess_187_215" title="Defined at ../ArrayAccess.sdf3 line 1">java/expressions/ArrayAccess</a>
  <a href="../FieldAccess.sdf3#java/expressions/FieldAccess_7_35" id="java/expressions/FieldAccess_218_246" title="Defined at ../FieldAccess.sdf3 line 1">java/expressions/FieldAccess</a>
  <a href="../MethodInvocation.sdf3#java/expressions/MethodInvocation_7_40" id="java/expressions/MethodInvocation_249_282" title="Defined at ../MethodInvocation.sdf3 line 1">java/expressions/MethodInvocation</a>
  <a href="../AssignmentOperators.sdf3#java/expressions/AssignmentOperators_7_43" id="java/expressions/AssignmentOperators_285_321" title="Defined at ../AssignmentOperators.sdf3 line 1">java/expressions/AssignmentOperators</a>
  <a href="../LambdaExpressions.sdf3#java/expressions/LambdaExpressions_7_41" id="java/expressions/LambdaExpressions_324_358" title="Defined at ../LambdaExpressions.sdf3 line 1">java/expressions/LambdaExpressions</a>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_361_377" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  
<span class="keyword">context-free priorities</span>

  <a href="../FieldAccess.sdf3#FieldAccess_174_185" id="FieldAccess_408_419" title="Defined at ../FieldAccess.sdf3 line 12, 18, 19, 20">FieldAccess</a>.<span class="cons_Constructor"><a href="../FieldAccess.sdf3#Field_254_259" id="Field_420_425" title="Defined at ../FieldAccess.sdf3 line 18">Field</a></span> &gt; 
  <a href="#Expression_2245_2255" id="Expression_431_441" title="Referenced at line 107">Expression</a> = <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_444_458" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>,
  
  <span id="ElementValue_465_477" title="Not referenced locally, nor via imports">ElementValue</span> = <a href="#Expression_431_441" id="Expression_480_490" title="Defined at line 18">Expression</a> &lt;0&gt; &gt;
  <a href="#Expression_431_441" id="Expression_499_509" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#Assign_230_236" id="Assign_510_516" title="Defined at ../AssignmentOperators.sdf3 line 16">Assign</a></span>  

<span class="keyword">context-free priorities</span>

  <a href="#Expression_431_441" id="Expression_547_557" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../ClassInstanceCreation.sdf3#QualifiedInstance_409_426" id="QualifiedInstance_558_575" title="Defined at ../ClassInstanceCreation.sdf3 line 21">QualifiedInstance</a></span> &gt; 
  {<span class="keyword">right</span>: 
    <a href="#Expression_431_441" id="Expression_594_604" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3#PostIncr_152_160" id="PostIncr_605_613" title="Defined at ../Postfix.sdf3 line 11">PostIncr</a></span> 
    <a href="#Expression_431_441" id="Expression_619_629" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3#PostDecr_193_201" id="PostDecr_630_638" title="Defined at ../Postfix.sdf3 line 12">PostDecr</a></span> } &gt;
  { 
    <a href="#Expression_431_441" id="Expression_652_662" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#CastPrimitive_483_496" id="CastPrimitive_663_676" title="Defined at ../UnaryOperators.sdf3 line 22">CastPrimitive</a></span> 
    <a href="#Expression_431_441" id="Expression_682_692" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#CastReference_545_558" id="CastReference_693_706" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span> }

<span class="keyword">context-free priorities</span>
  
  <a href="#Expression_431_441" id="Expression_739_749" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#CastPrimitive_483_496" id="CastPrimitive_750_763" title="Defined at ../UnaryOperators.sdf3 line 22">CastPrimitive</a></span> &gt; 
  {<span class="keyword">left</span>: 
    <a href="#Expression_431_441" id="Expression_781_791" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Mul_380_383" id="Mul_792_795" title="Defined at ../BinaryOperators.sdf3 line 17">Mul</a></span> 
    <a href="#Expression_431_441" id="Expression_801_811" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Div_436_439" id="Div_812_815" title="Defined at ../BinaryOperators.sdf3 line 18">Div</a></span>
    <a href="#Expression_431_441" id="Expression_820_830" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Mod_492_495" id="Mod_831_834" title="Defined at ../BinaryOperators.sdf3 line 19">Mod</a></span> }
  
<span class="keyword">context-free priorities</span>
  
  <a href="#Expression_431_441" id="Expression_869_879" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#CastReference_545_558" id="CastReference_880_893" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span> &gt; 
  { <a href="#Expression_431_441" id="Expression_901_911" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#PreIncr_319_326" id="PreIncr_912_919" title="Defined at ../UnaryOperators.sdf3 line 18">PreIncr</a></span>
    <a href="#Expression_431_441" id="Expression_924_934" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#PreDecr_359_366" id="PreDecr_935_942" title="Defined at ../UnaryOperators.sdf3 line 19">PreDecr</a></span>
    <a href="#Expression_431_441" id="Expression_947_957" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Plus_245_249" id="Plus_958_962" title="Defined at ../UnaryOperators.sdf3 line 16">Plus</a></span>
    <a href="#Expression_431_441" id="Expression_967_977" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Minus_282_287" id="Minus_978_983" title="Defined at ../UnaryOperators.sdf3 line 17">Minus</a></span> }
  ,
  <a href="#Expression_431_441" id="Expression_992_1002" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#CastReference_545_558" id="CastReference_1003_1016" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span> &lt;4&gt; .&gt; 
  { <a href="#Expression_431_441" id="Expression_1029_1039" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Plus_245_249" id="Plus_1040_1044" title="Defined at ../UnaryOperators.sdf3 line 16">Plus</a></span>
    <a href="#Expression_431_441" id="Expression_1049_1059" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Minus_282_287" id="Minus_1060_1065" title="Defined at ../UnaryOperators.sdf3 line 17">Minus</a></span> }   
    
 
<span class="keyword">context-free priorities</span>
  
  { <a href="../ArrayAccess.sdf3#ArrayAccess_158_169" id="ArrayAccess_1109_1120" title="Defined at ../ArrayAccess.sdf3 line 11, 17">ArrayAccess</a>.<span class="cons_Constructor"><a href="../ArrayAccess.sdf3#ArrayAccess_236_247" id="ArrayAccess_1121_1132" title="Defined at ../ArrayAccess.sdf3 line 17">ArrayAccess</a></span> 
    <a href="../FieldAccess.sdf3#FieldAccess_174_185" id="FieldAccess_1138_1149" title="Defined at ../FieldAccess.sdf3 line 12, 18, 19, 20">FieldAccess</a>.<span class="cons_Constructor"><a href="../FieldAccess.sdf3#Field_254_259" id="Field_1150_1155" title="Defined at ../FieldAccess.sdf3 line 18">Field</a></span> 
    <a href="#Expression_431_441" id="Expression_1161_1171" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../MethodInvocation.sdf3#InvokeQExp_493_503" id="InvokeQExp_1172_1182" title="Defined at ../MethodInvocation.sdf3 line 16">InvokeQExp</a></span> } &lt;0&gt; &gt;
  {<span class="keyword">right</span>: 
    <a href="#Expression_431_441" id="Expression_1206_1216" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3#PostIncr_152_160" id="PostIncr_1217_1225" title="Defined at ../Postfix.sdf3 line 11">PostIncr</a></span> 
    <a href="#Expression_431_441" id="Expression_1231_1241" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../Postfix.sdf3#PostDecr_193_201" id="PostDecr_1242_1250" title="Defined at ../Postfix.sdf3 line 12">PostDecr</a></span> } &gt;
  { <a href="#Expression_431_441" id="Expression_1259_1269" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#PreIncr_319_326" id="PreIncr_1270_1277" title="Defined at ../UnaryOperators.sdf3 line 18">PreIncr</a></span> 
    <a href="#Expression_431_441" id="Expression_1283_1293" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#PreDecr_359_366" id="PreDecr_1294_1301" title="Defined at ../UnaryOperators.sdf3 line 19">PreDecr</a></span> 
    <a href="#Expression_431_441" id="Expression_1307_1317" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Plus_245_249" id="Plus_1318_1322" title="Defined at ../UnaryOperators.sdf3 line 16">Plus</a></span> 
    <a href="#Expression_431_441" id="Expression_1328_1338" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Minus_282_287" id="Minus_1339_1344" title="Defined at ../UnaryOperators.sdf3 line 17">Minus</a></span> 
    <a href="#Expression_431_441" id="Expression_1350_1360" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Complement_399_409" id="Complement_1361_1371" title="Defined at ../UnaryOperators.sdf3 line 20">Complement</a></span> 
    <a href="#Expression_431_441" id="Expression_1377_1387" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#Not_441_444" id="Not_1388_1391" title="Defined at ../UnaryOperators.sdf3 line 21">Not</a></span> } &gt;
  {<span class="keyword">left</span>:
     <a href="#Expression_431_441" id="Expression_1410_1420" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Mul_380_383" id="Mul_1421_1424" title="Defined at ../BinaryOperators.sdf3 line 17">Mul</a></span> 
     <a href="#Expression_431_441" id="Expression_1431_1441" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Div_436_439" id="Div_1442_1445" title="Defined at ../BinaryOperators.sdf3 line 18">Div</a></span> 
     <a href="#Expression_431_441" id="Expression_1452_1462" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Mod_492_495" id="Mod_1463_1466" title="Defined at ../BinaryOperators.sdf3 line 19">Mod</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_431_441" id="Expression_1485_1495" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Add_551_554" id="Add_1496_1499" title="Defined at ../BinaryOperators.sdf3 line 21">Add</a></span> 
    <a href="#Expression_431_441" id="Expression_1505_1515" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Sub_607_610" id="Sub_1516_1519" title="Defined at ../BinaryOperators.sdf3 line 22">Sub</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_431_441" id="Expression_1538_1548" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#LeftShift_666_675" id="LeftShift_1549_1558" title="Defined at ../BinaryOperators.sdf3 line 24">LeftShift</a></span> 
    <a href="#Expression_431_441" id="Expression_1564_1574" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#RightShift_729_739" id="RightShift_1575_1585" title="Defined at ../BinaryOperators.sdf3 line 25">RightShift</a></span> 
    <a href="#Expression_431_441" id="Expression_1591_1601" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#URightShift_793_804" id="URightShift_1602_1613" title="Defined at ../BinaryOperators.sdf3 line 26">URightShift</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_431_441" id="Expression_1632_1642" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#InstanceOf_1092_1102" id="InstanceOf_1643_1653" title="Defined at ../BinaryOperators.sdf3 line 32">InstanceOf</a></span> 
    <a href="#Expression_431_441" id="Expression_1659_1669" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Lt_862_864" id="Lt_1670_1672" title="Defined at ../BinaryOperators.sdf3 line 28">Lt</a></span> 
    <a href="#Expression_431_441" id="Expression_1678_1688" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Gt_919_921" id="Gt_1689_1691" title="Defined at ../BinaryOperators.sdf3 line 29">Gt</a></span> 
    <a href="#Expression_431_441" id="Expression_1697_1707" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#LtEq_976_980" id="LtEq_1708_1712" title="Defined at ../BinaryOperators.sdf3 line 30">LtEq</a></span> 
    <a href="#Expression_431_441" id="Expression_1718_1728" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#GtEq_1034_1038" id="GtEq_1729_1733" title="Defined at ../BinaryOperators.sdf3 line 31">GtEq</a></span> } &gt;
  {<span class="keyword">left</span>: 
    <a href="#Expression_431_441" id="Expression_1752_1762" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Eq_1163_1165" id="Eq_1763_1765" title="Defined at ../BinaryOperators.sdf3 line 34">Eq</a></span> 
    <a href="#Expression_431_441" id="Expression_1771_1781" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#NotEq_1222_1227" id="NotEq_1782_1787" title="Defined at ../BinaryOperators.sdf3 line 35">NotEq</a></span> } &gt;
  <a href="#Expression_431_441" id="Expression_1794_1804" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#And_1284_1287" id="And_1805_1808" title="Defined at ../BinaryOperators.sdf3 line 37">And</a></span> &gt;
  <a href="#Expression_431_441" id="Expression_1813_1823" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Xor_1340_1343" id="Xor_1824_1827" title="Defined at ../BinaryOperators.sdf3 line 38">Xor</a></span> &gt;
  <a href="#Expression_431_441" id="Expression_1832_1842" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Or_1396_1398" id="Or_1843_1845" title="Defined at ../BinaryOperators.sdf3 line 39">Or</a></span> &gt;
  <a href="#Expression_431_441" id="Expression_1850_1860" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#LazyAnd_1455_1462" id="LazyAnd_1861_1868" title="Defined at ../BinaryOperators.sdf3 line 41">LazyAnd</a></span> &gt;
  <a href="#Expression_431_441" id="Expression_1873_1883" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#LazyOr_1516_1522" id="LazyOr_1884_1890" title="Defined at ../BinaryOperators.sdf3 line 42">LazyOr</a></span> &gt;
  <a href="#Expression_431_441" id="Expression_1895_1905" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../BinaryOperators.sdf3#Cond_1580_1584" id="Cond_1906_1910" title="Defined at ../BinaryOperators.sdf3 line 44">Cond</a></span> &gt;
  {<span class="keyword">right</span>: 
    <a href="#Expression_431_441" id="Expression_1928_1938" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#Assign_230_236" id="Assign_1939_1945" title="Defined at ../AssignmentOperators.sdf3 line 16">Assign</a></span>
    <a href="#Expression_431_441" id="Expression_1950_1960" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignMul_286_295" id="AssignMul_1961_1970" title="Defined at ../AssignmentOperators.sdf3 line 17">AssignMul</a></span>
    <a href="#Expression_431_441" id="Expression_1975_1985" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignDiv_343_352" id="AssignDiv_1986_1995" title="Defined at ../AssignmentOperators.sdf3 line 18">AssignDiv</a></span>
    <a href="#Expression_431_441" id="Expression_2000_2010" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignMod_400_409" id="AssignMod_2011_2020" title="Defined at ../AssignmentOperators.sdf3 line 19">AssignMod</a></span>
    <a href="#Expression_431_441" id="Expression_2025_2035" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignAdd_457_466" id="AssignAdd_2036_2045" title="Defined at ../AssignmentOperators.sdf3 line 20">AssignAdd</a></span>
    <a href="#Expression_431_441" id="Expression_2050_2060" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignSub_514_523" id="AssignSub_2061_2070" title="Defined at ../AssignmentOperators.sdf3 line 21">AssignSub</a></span>
    <a href="#Expression_431_441" id="Expression_2075_2085" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignLeftShift_571_586" id="AssignLeftShift_2086_2101" title="Defined at ../AssignmentOperators.sdf3 line 22">AssignLeftShift</a></span>
    <a href="#Expression_431_441" id="Expression_2106_2116" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignRightShift_629_645" id="AssignRightShift_2117_2133" title="Defined at ../AssignmentOperators.sdf3 line 23">AssignRightShift</a></span>
    <a href="#Expression_431_441" id="Expression_2138_2148" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignURightShift_687_704" id="AssignURightShift_2149_2166" title="Defined at ../AssignmentOperators.sdf3 line 24">AssignURightShift</a></span>
    <a href="#Expression_431_441" id="Expression_2171_2181" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignAnd_746_755" id="AssignAnd_2182_2191" title="Defined at ../AssignmentOperators.sdf3 line 25">AssignAnd</a></span>
    <a href="#Expression_431_441" id="Expression_2196_2206" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignXor_803_812" id="AssignXor_2207_2216" title="Defined at ../AssignmentOperators.sdf3 line 26">AssignXor</a></span>
    <a href="#Expression_431_441" id="Expression_2221_2231" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../AssignmentOperators.sdf3#AssignOr_860_868" id="AssignOr_2232_2240" title="Defined at ../AssignmentOperators.sdf3 line 27">AssignOr</a></span>
    <a href="#Expression_431_441" id="Expression_2245_2255" title="Defined at line 18">Expression</a>.<span class="cons_Constructor"><a href="../LambdaExpressions.sdf3#LambdaExpression_244_260" id="LambdaExpression_2256_2272" title="Defined at ../LambdaExpressions.sdf3 line 16">LambdaExpression</a></span> }

<span class="keyword">lexical restrictions</span>

  <span class="cons_Lit">"+"</span> -/- [\+]
  <span class="cons_Lit">"-"</span> -/- [\-]
  <span class="cons_Lit">"/"</span> -/- [\/]

</code></pre></td></tr></tbody></table></div>