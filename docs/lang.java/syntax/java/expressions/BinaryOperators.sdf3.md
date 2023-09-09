---
title: BinaryOperators.sdf3
---

# `BinaryOperators.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/BinaryOperators.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/BinaryOperators.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/BinaryOperators.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/BinaryOperators_375_407" id="java/expressions/BinaryOperators_7_39" title="Referenced at ../Main.sdf3 line 16">java/expressions/BinaryOperators</a>

<span class="layout">// 15.17. Multiplicative Operators</span>
<span class="layout">// 15.18. Additive Operators</span>
<span class="layout">// 15.19. Shift Operators</span>
<span class="layout">// 15.20. Relational Operators</span>
<span class="layout">// 15.21. Equality Operators</span>
<span class="layout">// 15.22. Bitwise and Logical Operators</span>
<span class="layout">// 15.23. Conditional-And Operator &amp;&amp;</span>
<span class="layout">// 15.24. Conditional-Or Operator ||</span>

<span class="keyword">imports</span>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_317_342" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_1619_1629" id="Expression_369_379" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Mul_1421_1424" id="Mul_380_383" title="Referenced at ../Disambiguation.sdf3 line 69">Mul</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_388_398" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">*</span> &lt;<a href="#Expression_369_379" id="Expression_403_413" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_425_435" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Div_1442_1445" id="Div_436_439" title="Referenced at ../Disambiguation.sdf3 line 70">Div</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_444_454" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">/</span> &lt;<a href="#Expression_369_379" id="Expression_459_469" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_481_491" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Mod_1463_1466" id="Mod_492_495" title="Referenced at ../Disambiguation.sdf3 line 71">Mod</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_500_510" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">%</span> &lt;<a href="#Expression_369_379" id="Expression_515_525" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_1619_1629" id="Expression_540_550" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Add_1496_1499" id="Add_551_554" title="Referenced at ../Disambiguation.sdf3 line 73">Add</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_559_569" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">+</span> &lt;<a href="#Expression_369_379" id="Expression_574_584" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_596_606" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Sub_1516_1519" id="Sub_607_610" title="Referenced at ../Disambiguation.sdf3 line 74">Sub</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_615_625" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">-</span> &lt;<a href="#Expression_369_379" id="Expression_630_640" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_1619_1629" id="Expression_655_665" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#LeftShift_1549_1558" id="LeftShift_666_675" title="Referenced at ../Disambiguation.sdf3 line 76">LeftShift</a></span> = [[<a href="#Expression_369_379" id="Expression_680_690" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&lt;&lt;</span> [<a href="#Expression_369_379" id="Expression_696_706" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_718_728" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#RightShift_1575_1585" id="RightShift_729_739" title="Referenced at ../Disambiguation.sdf3 line 77">RightShift</a></span> = [[<a href="#Expression_369_379" id="Expression_744_754" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;&gt;</span> [<a href="#Expression_369_379" id="Expression_760_770" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_782_792" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#URightShift_1602_1613" id="URightShift_793_804" title="Referenced at ../Disambiguation.sdf3 line 78">URightShift</a></span> = [[<a href="#Expression_369_379" id="Expression_809_819" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;&gt;&gt;</span> [<a href="#Expression_369_379" id="Expression_826_836" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  
  <a href="#Expression_1619_1629" id="Expression_851_861" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Lt_1670_1672" id="Lt_862_864" title="Referenced at ../Disambiguation.sdf3 line 81">Lt</a></span>   = [[<a href="#Expression_369_379" id="Expression_871_881" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&lt;</span> [<a href="#Expression_369_379" id="Expression_886_896" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_908_918" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Gt_1689_1691" id="Gt_919_921" title="Referenced at ../Disambiguation.sdf3 line 82">Gt</a></span>   = [[<a href="#Expression_369_379" id="Expression_928_938" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;</span> [<a href="#Expression_369_379" id="Expression_943_953" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_965_975" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#LtEq_1708_1712" id="LtEq_976_980" title="Referenced at ../Disambiguation.sdf3 line 83">LtEq</a></span> = [[<a href="#Expression_369_379" id="Expression_985_995" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&lt;=</span> [<a href="#Expression_369_379" id="Expression_1001_1011" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_1023_1033" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#GtEq_1729_1733" id="GtEq_1034_1038" title="Referenced at ../Disambiguation.sdf3 line 84">GtEq</a></span> = [[<a href="#Expression_369_379" id="Expression_1043_1053" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;=</span> [<a href="#Expression_369_379" id="Expression_1059_1069" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_1081_1091" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#InstanceOf_1643_1653" id="InstanceOf_1092_1102" title="Referenced at ../Disambiguation.sdf3 line 80">InstanceOf</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_1107_1117" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">instanceof</span> &lt;<a href="../../types/ReferenceTypes.sdf3#ReferenceType_218_231" id="ReferenceType_1131_1144" title="Defined at ../../types/ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;&gt;
  
  <a href="#Expression_1619_1629" id="Expression_1152_1162" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Eq_1763_1765" id="Eq_1163_1165" title="Referenced at ../Disambiguation.sdf3 line 86">Eq</a></span>    = &lt;&lt;<a href="#Expression_369_379" id="Expression_1173_1183" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">==</span> &lt;<a href="#Expression_369_379" id="Expression_1189_1199" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_1211_1221" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#NotEq_1782_1787" id="NotEq_1222_1227" title="Referenced at ../Disambiguation.sdf3 line 87">NotEq</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_1232_1242" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">!=</span> &lt;<a href="#Expression_369_379" id="Expression_1248_1258" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_1619_1629" id="Expression_1273_1283" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#And_1805_1808" id="And_1284_1287" title="Referenced at ../Disambiguation.sdf3 line 88">And</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_1292_1302" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">&amp;</span> &lt;<a href="#Expression_369_379" id="Expression_1307_1317" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_1329_1339" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Xor_1824_1827" id="Xor_1340_1343" title="Referenced at ../Disambiguation.sdf3 line 89">Xor</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_1348_1358" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">^</span> &lt;<a href="#Expression_369_379" id="Expression_1363_1373" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_1385_1395" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Or_1843_1845" id="Or_1396_1398" title="Referenced at ../Disambiguation.sdf3 line 90">Or</a></span>  = &lt;&lt;<a href="#Expression_369_379" id="Expression_1404_1414" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">|</span> &lt;<a href="#Expression_369_379" id="Expression_1419_1429" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_1619_1629" id="Expression_1444_1454" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#LazyAnd_1861_1868" id="LazyAnd_1455_1462" title="Referenced at ../Disambiguation.sdf3 line 91">LazyAnd</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_1467_1477" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">&amp;&amp;</span> &lt;<a href="#Expression_369_379" id="Expression_1483_1493" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_1619_1629" id="Expression_1505_1515" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#LazyOr_1884_1890" id="LazyOr_1516_1522" title="Referenced at ../Disambiguation.sdf3 line 92">LazyOr</a></span>  = &lt;&lt;<a href="#Expression_369_379" id="Expression_1528_1538" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">||</span> &lt;<a href="#Expression_369_379" id="Expression_1544_1554" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_1619_1629" id="Expression_1569_1579" title="Referenced at line 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Cond_1906_1910" id="Cond_1580_1584" title="Referenced at ../Disambiguation.sdf3 line 93">Cond</a></span> = &lt;&lt;<a href="#Expression_369_379" id="Expression_1589_1599" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">?</span> &lt;<a href="#Expression_369_379" id="Expression_1604_1614" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">:</span> &lt;<a href="#Expression_369_379" id="Expression_1619_1629" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">right</span>}
  
  
  
  
</code></pre></td></tr></tbody></table></div>