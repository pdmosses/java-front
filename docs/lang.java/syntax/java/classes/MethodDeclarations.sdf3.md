---
title: MethodDeclarations.sdf3
hide:
  - toc
---

# `MethodDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/classes/MethodDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/classes/MethodDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/classes/MethodDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../ClassDeclarations.sdf3/#java/classes/MethodDeclarations_215_246" id="java/classes/MethodDeclarations_7_38" title="Referenced at ../ClassDeclarations.sdf3 line 11; ../ConstructorDeclarations.sdf3 line 9; ../Main.sdf3 line 8; ../../expressions/LambdaExpressions.sdf3 line 8; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 7; ../../statements/LocalVariableDeclarations.sdf3 line 7; ../../statements/Statements.sdf3 line 7">java/classes/MethodDeclarations</a>

<span class="layout">// 8.4. Method Declarations</span>
<span class="keyword">imports</span>
  <a href="../FieldDeclarations.sdf3/#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_78_108" title="Defined at ../FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_111_136" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../ClassDeclarations.sdf3/#java/classes/ClassDeclarations_7_37" id="java/classes/ClassDeclarations_139_169" title="Defined at ../ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_172_196" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_199_221" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_224_251" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../statements/Blocks.sdf3/#java/statements/Blocks_7_29" id="java/statements/Blocks_254_276" title="Defined at ../../statements/Blocks.sdf3 line 1">java/statements/Blocks</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#MethodDeclaration_1692_1709" id="MethodDeclaration_300_317" title="Referenced at ../ClassDeclarations.sdf3 line 64">MethodDeclaration</a>
  <a href="#MethodHeader_565_577" id="MethodHeader_320_332" title="Referenced at line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 18">MethodHeader</a>
  <a href="#Result_631_637" id="Result_335_341" title="Referenced at line 34, 37">Result</a>
  <a href="#Throws_682_688" id="Throws_344_350" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25">Throws</a>
  <a href="#ExceptionType_902_915" id="ExceptionType_353_366" title="Referenced at line 42">ExceptionType</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_369_383" title="Referenced at line 31">MethodModifier</a>
  <a href="#MethodBody_580_590" id="MethodBody_386_396" title="Referenced at line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 18">MethodBody</a>
  <a href="#ReceiverParam_1530_1543" id="ReceiverParam_399_412" title="Referenced at line 63, 66">ReceiverParam</a>
  <a href="#FormalParams_645_657" id="FormalParams_415_427" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25; ../../expressions/LambdaExpressions.sdf3 line 20">FormalParams</a>
  <a href="#LastFormalParam_1579_1594" id="LastFormalParam_430_445" title="Referenced at line 64, 65, 66">LastFormalParam</a>
  <a href="#FormalParam_1633_1644" id="FormalParam_448_459" title="Referenced at line 65, 66, 68">FormalParam</a>
  <a href="#VariableModifier_1845_1861" id="VariableModifier_462_478" title="Referenced at line 69, 71; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 42, 45, 106, 128">VariableModifier</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../ClassDeclarations.sdf3/#MethodDeclaration_1692_1709" id="MethodDeclaration_505_522" title="Referenced at ../ClassDeclarations.sdf3 line 64">MethodDeclaration</a>.<span class="cons_Constructor"><span id="MethodDecl_523_533" title="Not referenced locally, nor via imports">MethodDecl</span></span> = &lt;
  &lt;{<a href="#MethodModifier_369_383" id="MethodModifier_542_556" title="Defined at line 20, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54">MethodModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#MethodHeader_320_332" id="MethodHeader_565_577" title="Defined at line 16, 33, 36">MethodHeader</a>&gt; &lt;<a href="#MethodBody_386_396" id="MethodBody_580_590" title="Defined at line 21, 56, 57">MethodBody</a>&gt;&gt;
  
  <a href="#MethodHeader_565_577" id="MethodHeader_598_610" title="Referenced at line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 18">MethodHeader</a>.<span class="cons_Constructor"><span id="MethodHeader_611_623" title="Not referenced locally, nor via imports">MethodHeader</span></span> = &lt;
  &lt;<a href="#Result_335_341" id="Result_631_637" title="Defined at line 17, 39, 40">Result</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_640_642" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;<a href="#FormalParams_415_427" id="FormalParams_645_657" title="Defined at line 23, 62, 63, 64, 65, 66">FormalParams</a>&gt;<span class="cons_String">)</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDimsEmpty_289_307" id="AnnotatedDimsEmpty_661_679" title="Defined at ../../types/ReferenceTypes.sdf3 line 18, 40">AnnotatedDimsEmpty</a>&gt; &lt;<a href="#Throws_344_350" id="Throws_682_688" title="Defined at line 18, 42">Throws</a>?&gt;&gt;
  
  <a href="#MethodHeader_565_577" id="MethodHeader_697_709" title="Referenced at line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 18">MethodHeader</a>.<span class="cons_Constructor"><span id="MethodHeaderTypeParameters_710_736" title="Not referenced locally, nor via imports">MethodHeaderTypeParameters</span></span> = &lt;
  &lt;<a href="../ClassDeclarations.sdf3/#TypeParameters_567_581" id="TypeParameters_744_758" title="Defined at ../ClassDeclarations.sdf3 line 25, 50">TypeParameters</a>&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_762_772" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#Result_335_341" id="Result_781_787" title="Defined at line 17, 39, 40">Result</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_790_792" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;<a href="#FormalParams_415_427" id="FormalParams_795_807" title="Defined at line 23, 62, 63, 64, 65, 66">FormalParams</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Throws_344_350" id="Throws_811_817" title="Defined at line 18, 42">Throws</a>?&gt;&gt;
  
  <a href="#Result_631_637" id="Result_826_832" title="Referenced at line 34, 37">Result</a> = <a href="../FieldDeclarations.sdf3/#UnannType_403_412" id="UnannType_835_844" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>
  <a href="#Result_631_637" id="Result_847_853" title="Referenced at line 34, 37">Result</a>.<span class="cons_Constructor"><span id="Void_854_858" title="Not referenced locally, nor via imports">Void</span></span> = <span class="cons_Lit">"void"</span>
  
  <a href="#Throws_682_688" id="Throws_873_879" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25">Throws</a>.<span class="cons_Constructor"><span id="ThrowsDec_880_889" title="Not referenced locally, nor via imports">ThrowsDec</span></span> = &lt;<span class="cons_String">throws</span> &lt;{<a href="#ExceptionType_353_366" id="ExceptionType_902_915" title="Defined at line 19, 43">ExceptionType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  <a href="#ExceptionType_902_915" id="ExceptionType_927_940" title="Referenced at line 42">ExceptionType</a>    = <a href="../../types/ReferenceTypes.sdf3/#ClassType_234_243" id="ClassType_946_955" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>
  
  <a href="#MethodModifier_542_556" id="MethodModifier_961_975" title="Referenced at line 31">MethodModifier</a> = <a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_978_988" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_991_1005" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_201_207" id="Public_1008_1014" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1017_1031" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Protected_189_198" id="Protected_1034_1043" title="Defined at ../../lexical/Modifiers.sdf3 line 13, 28">Protected</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1046_1060" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Private_179_186" id="Private_1063_1070" title="Defined at ../../lexical/Modifiers.sdf3 line 12, 27">Private</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1073_1087" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Abstract_141_149" id="Abstract_1090_1098" title="Defined at ../../lexical/Modifiers.sdf3 line 8, 23">Abstract</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1101_1115" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_210_216" id="Static_1118_1124" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1127_1141" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_162_167" id="Final_1144_1149" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1152_1166" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Synchronized_230_242" id="Synchronized_1169_1181" title="Defined at ../../lexical/Modifiers.sdf3 line 17, 34">Synchronized</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1184_1198" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Native_170_176" id="Native_1201_1207" title="Defined at ../../lexical/Modifiers.sdf3 line 11, 26">Native</a>
  <a href="#MethodModifier_542_556" id="MethodModifier_1210_1224" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Strictfp_219_227" id="Strictfp_1227_1235" title="Defined at ../../lexical/Modifiers.sdf3 line 16, 31">Strictfp</a>
  
  <a href="#MethodBody_580_590" id="MethodBody_1241_1251" title="Referenced at line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 18">MethodBody</a>         = <a href="../../statements/Blocks.sdf3/#Block_185_190" id="Block_1262_1267" title="Defined at ../../statements/Blocks.sdf3 line 12, 17">Block</a>
  <a href="#MethodBody_580_590" id="MethodBody_1270_1280" title="Referenced at line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3 line 18">MethodBody</a>.<span class="cons_Constructor"><span id="NoMethodBody_1281_1293" title="Not referenced locally, nor via imports">NoMethodBody</span></span> = <span class="cons_Lit">";"</span>
  
  <a href="#ReceiverParam_1530_1543" id="ReceiverParam_1305_1318" title="Referenced at line 63, 66">ReceiverParam</a>.<span class="cons_Constructor"><span id="ReceiverParamQual_1319_1336" title="Not referenced locally, nor via imports">ReceiverParamQual</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_1342_1352" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_403_412" id="UnannType_1361_1370" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_1373_1375" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">.this</span>&gt;
  <a href="#ReceiverParam_1530_1543" id="ReceiverParam_1385_1398" title="Referenced at line 63, 66">ReceiverParam</a>.<span class="cons_Constructor"><span id="ReceiverParam_1399_1412" title="Not referenced locally, nor via imports">ReceiverParam</span></span>     = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_1422_1432" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_403_412" id="UnannType_1441_1450" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; <span class="cons_String">this</span>&gt;

  <a href="#FormalParams_645_657" id="FormalParams_1461_1473" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25; ../../expressions/LambdaExpressions.sdf3 line 20">FormalParams</a>.<span class="cons_Constructor"><span id="NoParams_1474_1482" title="Not referenced locally, nor via imports">NoParams</span></span>          = 
  <a href="#FormalParams_645_657" id="FormalParams_1497_1509" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25; ../../expressions/LambdaExpressions.sdf3 line 20">FormalParams</a>                   = <a href="#ReceiverParam_399_412" id="ReceiverParam_1530_1543" title="Defined at line 22, 59, 60">ReceiverParam</a>
  <a href="#FormalParams_645_657" id="FormalParams_1546_1558" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25; ../../expressions/LambdaExpressions.sdf3 line 20">FormalParams</a>.<span class="cons_Constructor"><span id="SingleParam_1559_1570" title="Not referenced locally, nor via imports">SingleParam</span></span>       = <a href="#LastFormalParam_430_445" id="LastFormalParam_1579_1594" title="Defined at line 24, 68, 69">LastFormalParam</a>
  <a href="#FormalParams_645_657" id="FormalParams_1597_1609" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25; ../../expressions/LambdaExpressions.sdf3 line 20">FormalParams</a>.<span class="cons_Constructor"><span id="ParamList_1610_1619" title="Not referenced locally, nor via imports">ParamList</span></span>         = &lt;&lt;{<a href="#FormalParam_448_459" id="FormalParam_1633_1644" title="Defined at line 25, 71">FormalParam</a> <span class="cons_Lit">","</span>}+&gt;<span class="cons_String">,</span> &lt;<a href="#LastFormalParam_430_445" id="LastFormalParam_1654_1669" title="Defined at line 24, 68, 69">LastFormalParam</a>&gt;&gt;
  <a href="#FormalParams_645_657" id="FormalParams_1674_1686" title="Referenced at line 34, 37; ../ConstructorDeclarations.sdf3 line 25; ../../expressions/LambdaExpressions.sdf3 line 20">FormalParams</a>.<span class="cons_Constructor"><span id="ReceiverParamList_1687_1704" title="Not referenced locally, nor via imports">ReceiverParamList</span></span> = &lt;&lt;<a href="#ReceiverParam_399_412" id="ReceiverParam_1709_1722" title="Defined at line 22, 59, 60">ReceiverParam</a>&gt;<span class="cons_String">,</span> &lt;{<a href="#FormalParam_448_459" id="FormalParam_1727_1738" title="Defined at line 25, 71">FormalParam</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> &lt;<a href="#LastFormalParam_430_445" id="LastFormalParam_1748_1763" title="Defined at line 24, 68, 69">LastFormalParam</a>&gt;&gt;
  
  <a href="#LastFormalParam_1579_1594" id="LastFormalParam_1771_1786" title="Referenced at line 64, 65, 66">LastFormalParam</a>        = <a href="#FormalParam_448_459" id="FormalParam_1796_1807" title="Defined at line 25, 71">FormalParam</a>
  <a href="#LastFormalParam_1579_1594" id="LastFormalParam_1810_1825" title="Referenced at line 64, 65, 66">LastFormalParam</a>.<span class="cons_Constructor"><span id="VarArityParam_1826_1839" title="Not referenced locally, nor via imports">VarArityParam</span></span> = &lt;&lt;{<a href="#VariableModifier_462_478" id="VariableModifier_1845_1861" title="Defined at line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_403_412" id="UnannType_1870_1879" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_1883_1893" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">...</span> &lt;<a href="../FieldDeclarations.sdf3/#VarDeclId_343_352" id="VarDeclId_1906_1915" title="Defined at ../FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt;&gt;
    
  <a href="#FormalParam_1633_1644" id="FormalParam_1925_1936" title="Referenced at line 65, 66, 68">FormalParam</a>.<span class="cons_Constructor"><span id="FormalParam_1937_1948" title="Not referenced locally, nor via imports">FormalParam</span></span> = &lt;&lt;{<a href="#VariableModifier_462_478" id="VariableModifier_1954_1970" title="Defined at line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_403_412" id="UnannType_1979_1988" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../FieldDeclarations.sdf3/#VarDeclId_343_352" id="VarDeclId_1991_2000" title="Defined at ../FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt;&gt;
  
  <a href="#VariableModifier_1845_1861" id="VariableModifier_2008_2024" title="Referenced at line 69, 71; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 42, 45, 106, 128">VariableModifier</a> = <a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_2027_2037" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#VariableModifier_1845_1861" id="VariableModifier_2040_2056" title="Referenced at line 69, 71; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 42, 45, 106, 128">VariableModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_162_167" id="Final_2059_2064" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  
  
</code></pre></td></tr></tbody></table></div>