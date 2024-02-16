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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/classes/MethodDeclarations_1_8" title="a definition with multiple references" data-urls="../ClassDeclarations.sdf3/#java/classes/MethodDeclarations line 11_3; ../ConstructorDeclarations.sdf3/#java/classes/MethodDeclarations line 9_3; ../Main.sdf3/#java/classes/MethodDeclarations line 8_3; ../../expressions/LambdaExpressions.sdf3/#java/classes/MethodDeclarations line 8_3; ../../interfaces/InterfaceMethodDeclarations.sdf3/#java/classes/MethodDeclarations line 7_3; ../../statements/LocalVariableDeclarations.sdf3/#java/classes/MethodDeclarations line 7_3; ../../statements/Statements.sdf3/#java/classes/MethodDeclarations line 7_3">java/classes/MethodDeclarations</button>

<span class="layout">// 8.4. Method Declarations</span>
<span class="keyword">imports</span>
  <a href="../FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_5_3" title="a reference to a single-file definition">java/classes/FieldDeclarations</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../ClassDeclarations.sdf3/#java/classes/ClassDeclarations_1_8" id="java/classes/ClassDeclarations_7_3" title="a reference to a single-file definition">java/classes/ClassDeclarations</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_8_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_9_3" title="a reference to a single-file definition">java/lexical/Modifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_10_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>
  <a href="../../statements/Blocks.sdf3/#java/statements/Blocks_1_8" id="java/statements/Blocks_11_3" title="a reference to a single-file definition">java/statements/Blocks</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#MethodDeclaration_64_28" id="MethodDeclaration_15_3" title="a definition with a single reference">MethodDeclaration</a>
  <button class="modal-open" id="MethodHeader_16_3" title="a definition with multiple references" data-urls="#MethodHeader line 31_28; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodHeader line 18_37">MethodHeader</button>
  <button class="modal-open" id="Result_17_3" title="a definition with multiple references" data-urls="#Result line 34_4, 37_41">Result</button>
  <button class="modal-open" id="Throws_18_3" title="a definition with multiple references" data-urls="#Throws line 34_55, 37_71; ../ConstructorDeclarations.sdf3/#Throws line 25_72">Throws</button>
  <a href="#ExceptionType_42_32" id="ExceptionType_19_3" title="a definition with a single reference">ExceptionType</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_20_3" title="a definition with a single reference">MethodModifier</a>
  <button class="modal-open" id="MethodBody_21_3" title="a definition with multiple references" data-urls="#MethodBody line 31_43; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodBody line 18_52">MethodBody</button>
  <button class="modal-open" id="ReceiverParam_22_3" title="a definition with multiple references" data-urls="#ReceiverParam line 63_36, 66_38">ReceiverParam</button>
  <button class="modal-open" id="FormalParams_23_3" title="a definition with multiple references" data-urls="#FormalParams line 34_18, 37_55; ../ConstructorDeclarations.sdf3/#FormalParams line 25_56; ../../expressions/LambdaExpressions.sdf3/#FormalParams line 20_45">FormalParams</button>
  <button class="modal-open" id="LastFormalParam_24_3" title="a definition with multiple references" data-urls="#LastFormalParam line 64_36, 65_60, 66_77">LastFormalParam</button>
  <button class="modal-open" id="FormalParam_25_3" title="a definition with multiple references" data-urls="#FormalParam line 65_39, 66_56, 68_28">FormalParam</button>
  <button class="modal-open" id="VariableModifier_26_3" title="a definition with multiple references" data-urls="#VariableModifier line 69_38, 71_32; ../../statements/LocalVariableDeclarations.sdf3/#VariableModifier line 19_5; ../../statements/Statements.sdf3/#VariableModifier line 42_30, 45_25, 106_40, 128_26">VariableModifier</button>

<span class="keyword">context-free syntax</span>
  
  <a href="../ClassDeclarations.sdf3/#MethodDeclaration_64_28" id="MethodDeclaration_30_3" title="a definition with a single reference">MethodDeclaration</a>.<span class="cons_Constructor"><span id="MethodDecl_30_21" title="a definition with no references">MethodDecl</span></span> = &lt;
  &lt;{<a href="#MethodModifier_20_3" id="MethodModifier_31_5" title="a reference to a single-file definition">MethodModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#MethodHeader_16_3" id="MethodHeader_31_28" title="a reference to a single-file definition">MethodHeader</a>&gt; &lt;<a href="#MethodBody_21_3" id="MethodBody_31_43" title="a reference to a single-file definition">MethodBody</a>&gt;&gt;
  
  <button class="modal-open" id="MethodHeader_33_3" title="a definition with multiple references" data-urls="#MethodHeader line 31_28; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodHeader line 18_37">MethodHeader</button>.<span class="cons_Constructor"><span id="MethodHeader_33_16" title="a definition with no references">MethodHeader</span></span> = &lt;
  &lt;<a href="#Result_17_3" id="Result_34_4" title="a reference to a single-file definition">Result</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_34_13" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">(</span>&lt;<a href="#FormalParams_23_3" id="FormalParams_34_18" title="a reference to a single-file definition">FormalParams</a>&gt;<span class="cons_String">)</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDimsEmpty_18_3" id="AnnotatedDimsEmpty_34_34" title="a reference to a single-file definition">AnnotatedDimsEmpty</a>&gt; &lt;<a href="#Throws_18_3" id="Throws_34_55" title="a reference to a single-file definition">Throws</a>?&gt;&gt;
  
  <button class="modal-open" id="MethodHeader_36_3" title="a definition with multiple references" data-urls="#MethodHeader line 31_28; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodHeader line 18_37">MethodHeader</button>.<span class="cons_Constructor"><span id="MethodHeaderTypeParameters_36_16" title="a definition with no references">MethodHeaderTypeParameters</span></span> = &lt;
  &lt;<a href="../ClassDeclarations.sdf3/#TypeParameters_25_3" id="TypeParameters_37_4" title="a reference to a single-file definition">TypeParameters</a>&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_37_22" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#Result_17_3" id="Result_37_41" title="a reference to a single-file definition">Result</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_37_50" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">(</span>&lt;<a href="#FormalParams_23_3" id="FormalParams_37_55" title="a reference to a single-file definition">FormalParams</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Throws_18_3" id="Throws_37_71" title="a reference to a single-file definition">Throws</a>?&gt;&gt;
  
  <button class="modal-open" id="Result_39_3" title="a definition with multiple references" data-urls="#Result line 34_4, 37_41">Result</button> = <a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_39_12" title="a reference to a single-file definition">UnannType</a>
  <button class="modal-open" id="Result_40_3" title="a definition with multiple references" data-urls="#Result line 34_4, 37_41">Result</button>.<span class="cons_Constructor"><span id="Void_40_10" title="a definition with no references">Void</span></span> = <span class="cons_Lit">"void"</span>
  
  <button class="modal-open" id="Throws_42_3" title="a definition with multiple references" data-urls="#Throws line 34_55, 37_71; ../ConstructorDeclarations.sdf3/#Throws line 25_72">Throws</button>.<span class="cons_Constructor"><span id="ThrowsDec_42_10" title="a definition with no references">ThrowsDec</span></span> = &lt;<span class="cons_String">throws</span> &lt;{<a href="#ExceptionType_19_3" id="ExceptionType_42_32" title="a reference to a single-file definition">ExceptionType</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  <a href="#ExceptionType_42_32" id="ExceptionType_43_3" title="a definition with a single reference">ExceptionType</a>    = <a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_43_22" title="a reference to a single-file definition">ClassType</a>
  
  <a href="#MethodModifier_31_5" id="MethodModifier_45_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_45_20" title="a reference to a single-file definition">Annotation</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_46_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_46_20" title="a reference to a single-file definition">Public</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_47_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Protected_13_3" id="Protected_47_20" title="a reference to a single-file definition">Protected</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_48_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Private_12_3" id="Private_48_20" title="a reference to a single-file definition">Private</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_49_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Abstract_8_3" id="Abstract_49_20" title="a reference to a single-file definition">Abstract</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_50_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_50_20" title="a reference to a single-file definition">Static</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_51_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_51_20" title="a reference to a single-file definition">Final</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_52_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Synchronized_17_3" id="Synchronized_52_20" title="a reference to a single-file definition">Synchronized</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_53_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Native_11_3" id="Native_53_20" title="a reference to a single-file definition">Native</a>
  <a href="#MethodModifier_31_5" id="MethodModifier_54_3" title="a definition with a single reference">MethodModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Strictfp_16_3" id="Strictfp_54_20" title="a reference to a single-file definition">Strictfp</a>
  
  <button class="modal-open" id="MethodBody_56_3" title="a definition with multiple references" data-urls="#MethodBody line 31_43; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodBody line 18_52">MethodBody</button>         = <a href="../../statements/Blocks.sdf3/#Block_12_3" id="Block_56_24" title="a reference to a single-file definition">Block</a>
  <button class="modal-open" id="MethodBody_57_3" title="a definition with multiple references" data-urls="#MethodBody line 31_43; ../../interfaces/InterfaceMethodDeclarations.sdf3/#MethodBody line 18_52">MethodBody</button>.<span class="cons_Constructor"><span id="NoMethodBody_57_14" title="a definition with no references">NoMethodBody</span></span> = <span class="cons_Lit">";"</span>
  
  <button class="modal-open" id="ReceiverParam_59_3" title="a definition with multiple references" data-urls="#ReceiverParam line 63_36, 66_38">ReceiverParam</button>.<span class="cons_Constructor"><span id="ReceiverParamQual_59_17" title="a definition with no references">ReceiverParamQual</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_59_40" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_59_59" title="a reference to a single-file definition">UnannType</a>&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_59_71" title="a reference to a single-file definition">Id</a>&gt;<span class="cons_String">.this</span>&gt;
  <button class="modal-open" id="ReceiverParam_60_3" title="a definition with multiple references" data-urls="#ReceiverParam line 63_36, 66_38">ReceiverParam</button>.<span class="cons_Constructor"><span id="ReceiverParam_60_17" title="a definition with no references">ReceiverParam</span></span>     = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_60_40" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_60_59" title="a reference to a single-file definition">UnannType</a>&gt; <span class="cons_String">this</span>&gt;

  <button class="modal-open" id="FormalParams_62_3" title="a definition with multiple references" data-urls="#FormalParams line 34_18, 37_55; ../ConstructorDeclarations.sdf3/#FormalParams line 25_56; ../../expressions/LambdaExpressions.sdf3/#FormalParams line 20_45">FormalParams</button>.<span class="cons_Constructor"><span id="NoParams_62_16" title="a definition with no references">NoParams</span></span>          = 
  <button class="modal-open" id="FormalParams_63_3" title="a definition with multiple references" data-urls="#FormalParams line 34_18, 37_55; ../ConstructorDeclarations.sdf3/#FormalParams line 25_56; ../../expressions/LambdaExpressions.sdf3/#FormalParams line 20_45">FormalParams</button>                   = <a href="#ReceiverParam_22_3" id="ReceiverParam_63_36" title="a reference to a single-file definition">ReceiverParam</a>
  <button class="modal-open" id="FormalParams_64_3" title="a definition with multiple references" data-urls="#FormalParams line 34_18, 37_55; ../ConstructorDeclarations.sdf3/#FormalParams line 25_56; ../../expressions/LambdaExpressions.sdf3/#FormalParams line 20_45">FormalParams</button>.<span class="cons_Constructor"><span id="SingleParam_64_16" title="a definition with no references">SingleParam</span></span>       = <a href="#LastFormalParam_24_3" id="LastFormalParam_64_36" title="a reference to a single-file definition">LastFormalParam</a>
  <button class="modal-open" id="FormalParams_65_3" title="a definition with multiple references" data-urls="#FormalParams line 34_18, 37_55; ../ConstructorDeclarations.sdf3/#FormalParams line 25_56; ../../expressions/LambdaExpressions.sdf3/#FormalParams line 20_45">FormalParams</button>.<span class="cons_Constructor"><span id="ParamList_65_16" title="a definition with no references">ParamList</span></span>         = &lt;&lt;{<a href="#FormalParam_25_3" id="FormalParam_65_39" title="a reference to a single-file definition">FormalParam</a> <span class="cons_Lit">","</span>}+&gt;<span class="cons_String">,</span> &lt;<a href="#LastFormalParam_24_3" id="LastFormalParam_65_60" title="a reference to a single-file definition">LastFormalParam</a>&gt;&gt;
  <button class="modal-open" id="FormalParams_66_3" title="a definition with multiple references" data-urls="#FormalParams line 34_18, 37_55; ../ConstructorDeclarations.sdf3/#FormalParams line 25_56; ../../expressions/LambdaExpressions.sdf3/#FormalParams line 20_45">FormalParams</button>.<span class="cons_Constructor"><span id="ReceiverParamList_66_16" title="a definition with no references">ReceiverParamList</span></span> = &lt;&lt;<a href="#ReceiverParam_22_3" id="ReceiverParam_66_38" title="a reference to a single-file definition">ReceiverParam</a>&gt;<span class="cons_String">,</span> &lt;{<a href="#FormalParam_25_3" id="FormalParam_66_56" title="a reference to a single-file definition">FormalParam</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> &lt;<a href="#LastFormalParam_24_3" id="LastFormalParam_66_77" title="a reference to a single-file definition">LastFormalParam</a>&gt;&gt;
  
  <button class="modal-open" id="LastFormalParam_68_3" title="a definition with multiple references" data-urls="#LastFormalParam line 64_36, 65_60, 66_77">LastFormalParam</button>        = <a href="#FormalParam_25_3" id="FormalParam_68_28" title="a reference to a single-file definition">FormalParam</a>
  <button class="modal-open" id="LastFormalParam_69_3" title="a definition with multiple references" data-urls="#LastFormalParam line 64_36, 65_60, 66_77">LastFormalParam</button>.<span class="cons_Constructor"><span id="VarArityParam_69_19" title="a definition with no references">VarArityParam</span></span> = &lt;&lt;{<a href="#VariableModifier_26_3" id="VariableModifier_69_38" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_69_63" title="a reference to a single-file definition">UnannType</a>&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_69_76" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">...</span> &lt;<a href="../FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_69_99" title="a reference to a single-file definition">VarDeclId</a>&gt;&gt;
    
  <button class="modal-open" id="FormalParam_71_3" title="a definition with multiple references" data-urls="#FormalParam line 65_39, 66_56, 68_28">FormalParam</button>.<span class="cons_Constructor"><span id="FormalParam_71_15" title="a definition with no references">FormalParam</span></span> = &lt;&lt;{<a href="#VariableModifier_26_3" id="VariableModifier_71_32" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_71_57" title="a reference to a single-file definition">UnannType</a>&gt; &lt;<a href="../FieldDeclarations.sdf3/#VarDeclId_18_3" id="VarDeclId_71_69" title="a reference to a single-file definition">VarDeclId</a>&gt;&gt;
  
  <button class="modal-open" id="VariableModifier_73_3" title="a definition with multiple references" data-urls="#VariableModifier line 69_38, 71_32; ../../statements/LocalVariableDeclarations.sdf3/#VariableModifier line 19_5; ../../statements/Statements.sdf3/#VariableModifier line 42_30, 45_25, 106_40, 128_26">VariableModifier</button> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_73_22" title="a reference to a single-file definition">Annotation</a>
  <button class="modal-open" id="VariableModifier_74_3" title="a definition with multiple references" data-urls="#VariableModifier line 69_38, 71_32; ../../statements/LocalVariableDeclarations.sdf3/#VariableModifier line 19_5; ../../statements/Statements.sdf3/#VariableModifier line 42_30, 45_25, 106_40, 128_26">VariableModifier</button> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_74_22" title="a reference to a single-file definition">Final</a>
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
