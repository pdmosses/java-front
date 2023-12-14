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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/classes/MethodDeclarations_1_8" title="Multi-file references" data-urls="../ClassDeclarations.sdf3/#java/classes/MethodDeclarations_11_3 line 11; ../ConstructorDeclarations.sdf3/#java/classes/MethodDeclarations_9_3 line 9; ../Main.sdf3/#java/classes/MethodDeclarations_8_3 line 8; ../../expressions/LambdaExpressions.sdf3/#java/classes/MethodDeclarations_8_3 line 8; ../../interfaces/InterfaceMethodDeclarations.sdf3/#java/classes/MethodDeclarations_7_3 line 7; ../../statements/LocalVariableDeclarations.sdf3/#java/classes/MethodDeclarations_7_3 line 7; ../../statements/Statements.sdf3/#java/classes/MethodDeclarations_7_3 line 7">java/classes/MethodDeclarations</button>

<span class="layout">// 8.4. Method Declarations</span>
<span class="keyword">imports</span>
  <a href="../FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_5_3" title="Defined at ../FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../ClassDeclarations.sdf3/#java/classes/ClassDeclarations_1_8" id="java/classes/ClassDeclarations_7_3" title="Defined at ../ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_8_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_9_3" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_10_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../statements/Blocks.sdf3/#java/statements/Blocks_1_8" id="java/statements/Blocks_11_3" title="Defined at ../../statements/Blocks.sdf3 line 1">java/statements/Blocks</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#MethodDeclaration_64_28" id="MethodDeclaration_15_3" title="Referenced at ../ClassDeclarations.sdf3 line 64">MethodDeclaration</a>
  <button class="modal-open" id="MethodHeader_16_3" title="Multi-file references" data-urls="#MethodHeader_31_28 line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodHeader_18_37 line 18">MethodHeader</button>
  <a href="#Result_34_4" id="Result_17_3" title="Referenced at line 34, 37">Result</a>
  <button class="modal-open" id="Throws_18_3" title="Multi-file references" data-urls="#Throws_34_55 line 34, 37; ../ConstructorDeclarations.sdf3/#Throws_25_72 line 25">Throws</button>
  <a href="#ExceptionType_42_32" id="ExceptionType_19_3" title="Referenced at line 42">ExceptionType</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_20_3" title="Referenced at line 31">MethodModifier</a>
  <button class="modal-open" id="MethodBody_21_3" title="Multi-file references" data-urls="#MethodBody_31_43 line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodBody_18_52 line 18">MethodBody</button>
  <a href="#ReceiverParam_63_36" id="ReceiverParam_22_3" title="Referenced at line 63, 66">ReceiverParam</a>
  <button class="modal-open" id="FormalParams_23_3" title="Multi-file references" data-urls="#FormalParams_34_18 line 34, 37; ../ConstructorDeclarations.sdf3/#FormalParams_25_56 line 25; ../../expressions/LambdaExpressions.sdf3/#FormalParams_20_45 line 20">FormalParams</button>
  <a href="#LastFormalParam_64_36" id="LastFormalParam_24_3" title="Referenced at line 64, 65, 66">LastFormalParam</a>
  <a href="#FormalParam_65_39" id="FormalParam_25_3" title="Referenced at line 65, 66, 68">FormalParam</a>
  <button class="modal-open" id="VariableModifier_26_3" title="Multi-file references" data-urls="#VariableModifier_69_38 line 69, 71; ../../statements/LocalVariableDeclarations.sdf3/#VariableModifier_19_5 line 19; ../../statements/Statements.sdf3/#VariableModifier_42_30 line 42, 45, 106, 128">VariableModifier</button>

<span class="keyword">context-free syntax</span>
  
  <a href="../ClassDeclarations.sdf3/#MethodDeclaration_64_28" id="MethodDeclaration_30_3" title="Referenced at ../ClassDeclarations.sdf3 line 64">MethodDeclaration</a>.<span class="cons_Constructor"><span id="MethodDecl_30_21" title="Not referenced">MethodDecl</span></span> = &lt;
  &lt;{<a href="#MethodModifier_20_3" id="MethodModifier_31_5" title="Defined at line 20, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54">MethodModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#MethodHeader_16_3" id="MethodHeader_31_28" title="Defined at line 16, 33, 36">MethodHeader</a>&gt; &lt;<a href="#MethodBody_21_3" id="MethodBody_31_43" title="Defined at line 21, 56, 57">MethodBody</a>&gt;&gt;
  
  <button class="modal-open" id="MethodHeader_33_3" title="Multi-file references" data-urls="#MethodHeader_31_28 line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodHeader_18_37 line 18">MethodHeader</button>.<span class="cons_Constructor"><span id="MethodHeader_33_16" title="Not referenced">MethodHeader</span></span> = &lt;
  &lt;<a href="#Result_17_3" id="Result_34_4" title="Defined at line 17, 39, 40">Result</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_34_13" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;<a href="#FormalParams_23_3" id="FormalParams_34_18" title="Defined at line 23, 62, 63, 64, 65, 66">FormalParams</a>&gt;<span class="cons_String">)</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDimsEmpty_18_3" id="AnnotatedDimsEmpty_34_34" title="Defined at ../../types/ReferenceTypes.sdf3 line 18, 40">AnnotatedDimsEmpty</a>&gt; &lt;<a href="#Throws_18_3" id="Throws_34_55" title="Defined at line 18, 42">Throws</a>?&gt;&gt;
  
  <button class="modal-open" id="MethodHeader_36_3" title="Multi-file references" data-urls="#MethodHeader_31_28 line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodHeader_18_37 line 18">MethodHeader</button>.<span class="cons_Constructor"><span id="MethodHeaderTypeParameters_36_16" title="Not referenced">MethodHeaderTypeParameters</span></span> = &lt;
  &lt;<a href="../ClassDeclarations.sdf3/#TypeParameters_25_3" id="TypeParameters_37_4" title="Defined at ../ClassDeclarations.sdf3 line 25, 50">TypeParameters</a>&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_37_22" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#Result_17_3" id="Result_37_41" title="Defined at line 17, 39, 40">Result</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_37_50" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">(</span>&lt;<a href="#FormalParams_23_3" id="FormalParams_37_55" title="Defined at line 23, 62, 63, 64, 65, 66">FormalParams</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Throws_18_3" id="Throws_37_71" title="Defined at line 18, 42">Throws</a>?&gt;&gt;
  
  <a href="#Result_34_4" id="Result_39_3" title="Referenced at line 34, 37">Result</a> = <a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_39_12" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>
  <a href="#Result_34_4" id="Result_40_3" title="Referenced at line 34, 37">Result</a>.<span class="cons_Constructor"><span id="Void_40_10" title="Not referenced">Void</span></span> = <span class="cons_Lit">"void"</span>
  
  <button class="modal-open" id="Throws_42_3" title="Multi-file references" data-urls="#Throws_34_55 line 34, 37; ../ConstructorDeclarations.sdf3/#Throws_25_72 line 25">Throws</button>.<span class="cons_Constructor"><span id="ThrowsDec_42_10" title="Not referenced">ThrowsDec</span></span> = &lt;<span class="cons_String">throws</span> &lt;{<a href="#ExceptionType_19_3" id="ExceptionType_42_32" title="Defined at line 19, 43">ExceptionType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  <a href="#ExceptionType_42_32" id="ExceptionType_43_3" title="Referenced at line 42">ExceptionType</a>    = <a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_43_22" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>
  
  <a href="#MethodModifier_31_5" id="MethodModifier_45_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_45_20" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_46_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_46_20" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_47_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Protected_13_3" id="Protected_47_20" title="Defined at ../../lexical/Modifiers.sdf3 line 13, 28">Protected</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_48_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Private_12_3" id="Private_48_20" title="Defined at ../../lexical/Modifiers.sdf3 line 12, 27">Private</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_49_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Abstract_8_3" id="Abstract_49_20" title="Defined at ../../lexical/Modifiers.sdf3 line 8, 23">Abstract</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_50_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_50_20" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_51_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_51_20" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_52_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Synchronized_17_3" id="Synchronized_52_20" title="Defined at ../../lexical/Modifiers.sdf3 line 17, 34">Synchronized</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_53_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Native_11_3" id="Native_53_20" title="Defined at ../../lexical/Modifiers.sdf3 line 11, 26">Native</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_54_3" title="Referenced at line 31">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Strictfp_16_3" id="Strictfp_54_20" title="Defined at ../../lexical/Modifiers.sdf3 line 16, 31">Strictfp</a>
  
  <button class="modal-open" id="MethodBody_56_3" title="Multi-file references" data-urls="#MethodBody_31_43 line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodBody_18_52 line 18">MethodBody</button>         = <a href="../../statements/Blocks.sdf3/#Block_12_3" id="Block_56_24" title="Defined at ../../statements/Blocks.sdf3 line 12, 17">Block</a>
  <button class="modal-open" id="MethodBody_57_3" title="Multi-file references" data-urls="#MethodBody_31_43 line 31; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodBody_18_52 line 18">MethodBody</button>.<span class="cons_Constructor"><span id="NoMethodBody_57_14" title="Not referenced">NoMethodBody</span></span> = <span class="cons_Lit">";"</span>
  
  <a href="#ReceiverParam_63_36" id="ReceiverParam_59_3" title="Referenced at line 63, 66">ReceiverParam</a>.<span class="cons_Constructor"><span id="ReceiverParamQual_59_17" title="Not referenced">ReceiverParamQual</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_59_40" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_59_59" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_59_71" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;<span class="cons_String">.this</span>&gt;
  <a href="#ReceiverParam_63_36" id="ReceiverParam_60_3" title="Referenced at line 63, 66">ReceiverParam</a>.<span class="cons_Constructor"><span id="ReceiverParam_60_17" title="Not referenced">ReceiverParam</span></span>     = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_60_40" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_60_59" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; <span class="cons_String">this</span>&gt;

  <button class="modal-open" id="FormalParams_62_3" title="Multi-file references" data-urls="#FormalParams_34_18 line 34, 37; ../ConstructorDeclarations.sdf3/#FormalParams_25_56 line 25; ../../expressions/LambdaExpressions.sdf3/#FormalParams_20_45 line 20">FormalParams</button>.<span class="cons_Constructor"><span id="NoParams_62_16" title="Not referenced">NoParams</span></span>          = 
  <button class="modal-open" id="FormalParams_63_3" title="Multi-file references" data-urls="#FormalParams_34_18 line 34, 37; ../ConstructorDeclarations.sdf3/#FormalParams_25_56 line 25; ../../expressions/LambdaExpressions.sdf3/#FormalParams_20_45 line 20">FormalParams</button>                   = <a href="#ReceiverParam_22_3" id="ReceiverParam_63_36" title="Defined at line 22, 59, 60">ReceiverParam</a>
  <button class="modal-open" id="FormalParams_64_3" title="Multi-file references" data-urls="#FormalParams_34_18 line 34, 37; ../ConstructorDeclarations.sdf3/#FormalParams_25_56 line 25; ../../expressions/LambdaExpressions.sdf3/#FormalParams_20_45 line 20">FormalParams</button>.<span class="cons_Constructor"><span id="SingleParam_64_16" title="Not referenced">SingleParam</span></span>       = <a href="#LastFormalParam_24_3" id="LastFormalParam_64_36" title="Defined at line 24, 68, 69">LastFormalParam</a>
  <button class="modal-open" id="FormalParams_65_3" title="Multi-file references" data-urls="#FormalParams_34_18 line 34, 37; ../ConstructorDeclarations.sdf3/#FormalParams_25_56 line 25; ../../expressions/LambdaExpressions.sdf3/#FormalParams_20_45 line 20">FormalParams</button>.<span class="cons_Constructor"><span id="ParamList_65_16" title="Not referenced">ParamList</span></span>         = &lt;&lt;{<a href="#FormalParam_25_3" id="FormalParam_65_39" title="Defined at line 25, 71">FormalParam</a> <span class="cons_Lit">","</span>}+&gt;<span class="cons_String">,</span> &lt;<a href="#LastFormalParam_24_3" id="LastFormalParam_65_60" title="Defined at line 24, 68, 69">LastFormalParam</a>&gt;&gt;
  <button class="modal-open" id="FormalParams_66_3" title="Multi-file references" data-urls="#FormalParams_34_18 line 34, 37; ../ConstructorDeclarations.sdf3/#FormalParams_25_56 line 25; ../../expressions/LambdaExpressions.sdf3/#FormalParams_20_45 line 20">FormalParams</button>.<span class="cons_Constructor"><span id="ReceiverParamList_66_16" title="Not referenced">ReceiverParamList</span></span> = &lt;&lt;<a href="#ReceiverParam_22_3" id="ReceiverParam_66_38" title="Defined at line 22, 59, 60">ReceiverParam</a>&gt;<span class="cons_String">,</span> &lt;{<a href="#FormalParam_25_3" id="FormalParam_66_56" title="Defined at line 25, 71">FormalParam</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> &lt;<a href="#LastFormalParam_24_3" id="LastFormalParam_66_77" title="Defined at line 24, 68, 69">LastFormalParam</a>&gt;&gt;
  
  <a href="#LastFormalParam_64_36" id="LastFormalParam_68_3" title="Referenced at line 64, 65, 66">LastFormalParam</a>        = <a href="#FormalParam_25_3" id="FormalParam_68_28" title="Defined at line 25, 71">FormalParam</a>
  <a href="#LastFormalParam_64_36" id="LastFormalParam_69_3" title="Referenced at line 64, 65, 66">LastFormalParam</a>.<span class="cons_Constructor"><span id="VarArityParam_69_19" title="Not referenced">VarArityParam</span></span> = &lt;&lt;{<a href="#VariableModifier_26_3" id="VariableModifier_69_38" title="Defined at line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_69_63" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_69_76" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">...</span> &lt;<a href="../FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_69_99" title="Defined at ../FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt;&gt;
    
  <a href="#FormalParam_65_39" id="FormalParam_71_3" title="Referenced at line 65, 66, 68">FormalParam</a>.<span class="cons_Constructor"><span id="FormalParam_71_15" title="Not referenced">FormalParam</span></span> = &lt;&lt;{<a href="#VariableModifier_26_3" id="VariableModifier_71_32" title="Defined at line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_71_57" title="Defined at ../FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;<a href="../FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_71_69" title="Defined at ../FieldDeclarations.sdf3 line 18, 31, 32">VarDeclId</a>&gt;&gt;
  
  <button class="modal-open" id="VariableModifier_73_3" title="Multi-file references" data-urls="#VariableModifier_69_38 line 69, 71; ../../statements/LocalVariableDeclarations.sdf3/#VariableModifier_19_5 line 19; ../../statements/Statements.sdf3/#VariableModifier_42_30 line 42, 45, 106, 128">VariableModifier</button> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_73_22" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <button class="modal-open" id="VariableModifier_74_3" title="Multi-file references" data-urls="#VariableModifier_69_38 line 69, 71; ../../statements/LocalVariableDeclarations.sdf3/#VariableModifier_19_5 line 19; ../../statements/Statements.sdf3/#VariableModifier_42_30 line 42, 45, 106, 128">VariableModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_74_22" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
