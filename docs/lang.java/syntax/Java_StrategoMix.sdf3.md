---
title: Java_StrategoMix.sdf3
hide:
  - toc
---

# `Java_StrategoMix.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/Java_StrategoMix.sdf3]

[pdmosses/java-front/lang.java/syntax/Java_StrategoMix.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/Java_StrategoMix.sdf3 "The source file on GitHub"

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
137
138
139
140
141
142
143
144
145
146
147
148
149
150
151
152
153
154
155
156
157
158
159
160
161
162
163
164
165
166
167
168
169
170
171
172
173
174
175
176
177
178
179
180
181
182
183
184
185
186
187
188
189
190
191
192
193
194
195
196
197
198
199
200
201
202
203
204
205
206
207
208
209
210
211
212
213
214
215
216
217
218
219
220
221
222
223
224
225
226
227
228
229
230
231
232
233
234
235
236
237
238
239
240
241
242
243
244
245
246
247
248
249
250
251
252
253
254
255
256
257
258
259
260
261
262
263
264
265
266
267
268
269
270
271
272
273
274
275
276
277
278
279
280
281
282
283
284
285
286
287
288
289
290
291
292
293
294
295
296
297
298
299
300
301
302
303
304
305
306
307
308
309
310
311
312
313
314
315
316
317
318
319
320
321
322
323
324
325
326
327
328
329
330
331
332
333
334
335
336
337
338
339
340
341
342
343
344
345
346
347
348
349
350
351
352
353
354
355
356
357
358
359
360
361
362
363
364
365
366
367
368
369
370
371
372
373
374
375
376
377
378
379
380
381
382
383
384
385
386
387
388
389
390
391
392
393
394
395
396
397
398
399
400
401
402
403
404
405
406
407
408
409
410
411
412
413
414
415
416
417
418
419
420
421
422
423
424
425
426
427
428
429
430
431
432
433
434
435
436
437
438
439
440
441
442
443
444
445
446
447
448
449
450
451
452
453
454
455
456
457
458
459
460
461
462
463
464
465
466
467
468
469
470
471
472
473
474
475
476
477
478
479
480
481
482
483
484
485
486
487
488
489
490
491
492
493
494
495
496
497
498
499
500
501
502
503
504
505
506
507
508
509
510
511
512
513
514
515
516
517
518
519
520
521
522
523
524
525
526
527
528
529
530
531
532
533
534
535
536
537
538
539
540
541
542
543
544
545
546
547
548
549
550
551
552
553
554
555
556
557
558
559
560
561
562
563
564
565
566
567
568
569
570
571
572
573
574
575
576
577
578
579
580
581
582
583
584
585
586
587
588
589
590
591
592
593
594
595
596
597
598
599
600
601
602
603
604
605
606
607
608
609
610
611
612
613
614
615
616
617
618
619
620
621
622
623
624
625
626
627
628
629
630
631
632
633
634
635
636
637
638
639
640
641
642
643
644
645
646
647
648
649
650
651
652
653
654
655
656
657
658
659
660
661
662
663
664
665
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <span id="Java_StrategoMix_1_8" title="Not referenced">Java_StrategoMix</span>

<span class="keyword">imports</span>
  <a href="../java/packages/CompilationUnits.sdf3/#java/packages/CompilationUnits_1_8" id="java/packages/CompilationUnits_4_3" title="Defined at ../java/packages/CompilationUnits.sdf3 line 1">java/packages/CompilationUnits</a>

  StrategoLang/import-namespaced
  StrategoLang/sugar/terms-namespaced
  StrategoLang/core/identifiers-namespaced

<span class="keyword">context-free start-symbols</span>

  <a href="#Module_16_3" id="Module_12_3" title="Defined at line 16">Module</a>

<span class="keyword">context-free syntax</span>

  <a href="#Module_12_3" id="Module_16_3" title="Referenced at line 12">Module</a> = StrategoLang-Module

<span class="layout">///</span>
<span class="layout">// Quotations for CompilationUnit</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_22_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_22_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java:compilation-unit"</span> <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3/#CompilationUnit_12_3" id="CompilationUnit_22_63" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_23_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_23_21" title="Not referenced">ToMetaExpr</span></span> =      <span class="cons_Lit">"compilation-unit"</span> <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3/#CompilationUnit_12_3" id="CompilationUnit_23_63" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_24_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_24_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>                  <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3/#CompilationUnit_12_3" id="CompilationUnit_24_63" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_25_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_25_21" title="Not referenced">ToMetaExpr</span></span> =                         <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3/#CompilationUnit_12_3" id="CompilationUnit_25_63" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Variables for Formal Parameters</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#FormalParam_42_60" id="FormalParam_31_3" title="Referenced at line 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 63">FormalParam</a>  = <span class="cons_Lit">"param"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <a href="#FormalParam_42_60" id="FormalParam_32_3" title="Referenced at line 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 63">FormalParam</a>  = <span class="cons_Lit">"param_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <span id="FormalParams_33_3" title="Not referenced">FormalParams</span> = <span class="cons_Lit">"params"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <span id="FormalParams_34_3" title="Not referenced">FormalParams</span> = <span class="cons_Lit">"params_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <span id="FormalParams_35_3" title="Not referenced">FormalParams</span> = <span class="cons_Lit">"param"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}
  <span id="FormalParams_36_3" title="Not referenced">FormalParams</span> = <span class="cons_Lit">"param_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}

<span class="layout">///</span>
<span class="layout">// Quotations for Formal Parameters</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_42_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_42_21" title="Not referenced">ToMetaExpr</span></span> =             <span class="cons_Lit">"param"</span>  <span class="cons_Lit">"|["</span> <a href="#FormalParam_31_3" id="FormalParam_42_60" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_43_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_43_21" title="Not referenced">ToMetaExpr</span></span> =        <span class="cons_Lit">"java:param"</span>  <span class="cons_Lit">"|["</span> <a href="#FormalParam_31_3" id="FormalParam_43_60" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_45_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_45_21" title="Not referenced">ToMetaExpr</span></span> =             <span class="cons_Lit">"param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_31_3" id="FormalParam_45_61" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_46_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_46_21" title="Not referenced">ToMetaExpr</span></span> =        <span class="cons_Lit">"java:param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_31_3" id="FormalParam_46_61" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_48_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_48_21" title="Not referenced">ToMetaExpr</span></span> =  <span class="cons_Lit">"java:formal-param"</span> <span class="cons_Lit">"|["</span> <a href="#FormalParam_31_3" id="FormalParam_48_60" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_49_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_49_21" title="Not referenced">ToMetaExpr</span></span> =       <span class="cons_Lit">"formal-param"</span> <span class="cons_Lit">"|["</span> <a href="#FormalParam_31_3" id="FormalParam_49_60" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_50_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_50_21" title="Not referenced">ToMetaExpr</span></span> =  <span class="cons_Lit">"java"</span>              <span class="cons_Lit">"|["</span> <a href="#FormalParam_31_3" id="FormalParam_50_60" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_51_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_51_21" title="Not referenced">ToMetaExpr</span></span> =                      <span class="cons_Lit">"|["</span> <a href="#FormalParam_31_3" id="FormalParam_51_60" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_53_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_53_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java:formal-param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_31_3" id="FormalParam_53_61" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_54_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_54_21" title="Not referenced">ToMetaExpr</span></span> =      <span class="cons_Lit">"formal-param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_31_3" id="FormalParam_54_61" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_55_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_55_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>               <span class="cons_Lit">"|["</span> {<a href="#FormalParam_31_3" id="FormalParam_55_61" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_56_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_56_21" title="Not referenced">ToMetaExpr</span></span> =                      <span class="cons_Lit">"|["</span> {<a href="#FormalParam_31_3" id="FormalParam_56_61" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Formal Parameters</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
   <a href="#FormalParam_42_60" id="FormalParam_62_4" title="Referenced at line 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 63">FormalParam</a>.<span class="cons_Constructor"><span id="FromMetaExpr_62_16" title="Not referenced">FromMetaExpr</span></span>       = <span class="cons_Lit">"~"</span>  <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_62_42" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  {<a href="#FormalParam_31_3" id="FormalParam_63_4" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}*.<span class="cons_Constructor">FromMetaExpr</span> = <span class="cons_Lit">"~*"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_63_42" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Anti-Quotation for Types</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_69_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_69_21" title="Not referenced">ToMetaExpr</span></span> =         <span class="cons_Lit">"t"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_82_3" id="UnannType_69_51" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_70_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_70_21" title="Not referenced">ToMetaExpr</span></span> =        <span class="cons_Lit">"ty"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_82_3" id="UnannType_70_51" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_72_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_72_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java:type"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_82_3" id="UnannType_72_51" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_73_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_73_21" title="Not referenced">ToMetaExpr</span></span> =      <span class="cons_Lit">"type"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_82_3" id="UnannType_73_51" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_74_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_74_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>      <span class="cons_Lit">"|["</span> <a href="#UnannType_82_3" id="UnannType_74_51" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_75_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_75_21" title="Not referenced">ToMetaExpr</span></span> =             <span class="cons_Lit">"|["</span> <a href="#UnannType_82_3" id="UnannType_75_51" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_76_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_76_21" title="Not referenced">ToMetaExpr</span></span> =     <span class="cons_Lit">"rtype"</span> <span class="cons_Lit">"|["</span> <a href="#ReferenceType_85_3" id="ReferenceType_76_51" title="Defined at line 85, 86, 94">ReferenceType</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti-Quotation for Types</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#UnannType_69_51" id="UnannType_82_3" title="Referenced at line 69, 70, 72, 73, 74, 75">UnannType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_82_13" title="Not referenced">FromMetaExpr</span></span>     = <span class="cons_Lit">"~"</span>        <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_82_43" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#UnannType_69_51" id="UnannType_83_3" title="Referenced at line 69, 70, 72, 73, 74, 75">UnannType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_83_13" title="Not referenced">FromMetaExpr</span></span>     = <span class="cons_Lit">"~type:"</span>   <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_83_43" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

  <a href="#ReferenceType_76_51" id="ReferenceType_85_3" title="Referenced at line 76">ReferenceType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_85_17" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~refType"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_85_43" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#ReferenceType_76_51" id="ReferenceType_86_3" title="Referenced at line 76">ReferenceType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_86_17" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~rtype:"</span>  <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_86_43" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Variables for Types</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#UnannType_69_51" id="UnannType_92_3" title="Referenced at line 69, 70, 72, 73, 74, 75">UnannType</a>     = <a href="#MetaTypeVar_97_3" id="MetaTypeVar_92_19" title="Defined at line 97, 98, 99, 100">MetaTypeVar</a> {<span class="keyword">prefer</span>}
  <span id="PrimitiveType_93_3" title="Not referenced">PrimitiveType</span> = <a href="#MetaPrimTypeVar_102_3" id="MetaPrimTypeVar_93_19" title="Defined at line 102, 103, 104, 105">MetaPrimTypeVar</a> {<span class="keyword">prefer</span>}
  <a href="#ReferenceType_76_51" id="ReferenceType_94_3" title="Referenced at line 76">ReferenceType</a> = <a href="#MetaReferenceTypeVar_107_3" id="MetaReferenceTypeVar_94_19" title="Defined at line 107, 108, 109, 110">MetaReferenceTypeVar</a> {<span class="keyword">prefer</span>}

<span class="keyword">lexical syntax</span>
  <a href="#MetaTypeVar_92_19" id="MetaTypeVar_97_3" title="Referenced at line 92, 128">MetaTypeVar</a>          = <span class="cons_Lit">"t"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaTypeVar_92_19" id="MetaTypeVar_98_3" title="Referenced at line 92, 128">MetaTypeVar</a>          = <span class="cons_Lit">"t_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaTypeVar_92_19" id="MetaTypeVar_99_3" title="Referenced at line 92, 128">MetaTypeVar</a>          = <span class="cons_Lit">"ty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaTypeVar_92_19" id="MetaTypeVar_100_3" title="Referenced at line 92, 128">MetaTypeVar</a>          = <span class="cons_Lit">"ty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*

  <a href="#MetaPrimTypeVar_93_19" id="MetaPrimTypeVar_102_3" title="Referenced at line 93, 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaPrimTypeVar_93_19" id="MetaPrimTypeVar_103_3" title="Referenced at line 93, 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaPrimTypeVar_93_19" id="MetaPrimTypeVar_104_3" title="Referenced at line 93, 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaPrimTypeVar_93_19" id="MetaPrimTypeVar_105_3" title="Referenced at line 93, 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*

  <a href="#MetaReferenceTypeVar_94_19" id="MetaReferenceTypeVar_107_3" title="Referenced at line 94, 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaReferenceTypeVar_94_19" id="MetaReferenceTypeVar_108_3" title="Referenced at line 94, 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaReferenceTypeVar_94_19" id="MetaReferenceTypeVar_109_3" title="Referenced at line 94, 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaReferenceTypeVar_94_19" id="MetaReferenceTypeVar_110_3" title="Referenced at line 94, 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*

  <a href="#ID_249_3" id="ID_112_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"t"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_113_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"t_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_114_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"ty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_115_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"ty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

  <a href="#ID_249_3" id="ID_117_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_118_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_119_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_120_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

  <a href="#ID_249_3" id="ID_122_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_123_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_124_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_125_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

<span class="keyword">lexical restrictions</span>
  <a href="#MetaTypeVar_97_3" id="MetaTypeVar_128_3" title="Defined at line 97, 98, 99, 100">MetaTypeVar</a>          -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$\']
  <a href="#MetaPrimTypeVar_102_3" id="MetaPrimTypeVar_129_3" title="Defined at line 102, 103, 104, 105">MetaPrimTypeVar</a>      -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$\']
  <a href="#MetaReferenceTypeVar_107_3" id="MetaReferenceTypeVar_130_3" title="Defined at line 107, 108, 109, 110">MetaReferenceTypeVar</a> -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$\']

<span class="layout">///</span>
<span class="layout">// Quotations for Statements</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_136_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_136_21" title="Not referenced">ToMetaExpr</span></span>     =        <span class="cons_Lit">"java:bstm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_136_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_137_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_137_21" title="Not referenced">ToMetaExpr</span></span>     =             <span class="cons_Lit">"bstm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_137_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_138_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_138_21" title="Not referenced">ToMetaExpr</span></span>     =        <span class="cons_Lit">"java"</span>       <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_138_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_139_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_139_21" title="Not referenced">ToMetaExpr</span></span>     =                     <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_139_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_141_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_141_21" title="Not referenced">ToMetaListExpr</span></span> =        <span class="cons_Lit">"java:bstm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_141_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_142_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_142_21" title="Not referenced">ToMetaListExpr</span></span> =             <span class="cons_Lit">"bstm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_142_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_144_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_144_21" title="Not referenced">ToMetaExpr</span></span>     =   <span class="cons_Lit">"java:block-stm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_144_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_145_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_145_21" title="Not referenced">ToMetaExpr</span></span>     =        <span class="cons_Lit">"block-stm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_145_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_146_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_146_21" title="Not referenced">ToMetaExpr</span></span>     =   <span class="cons_Lit">"java"</span>            <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_146_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_147_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_147_21" title="Not referenced">ToMetaExpr</span></span>     =                     <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_147_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_149_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_149_21" title="Not referenced">ToMetaListExpr</span></span> =   <span class="cons_Lit">"java:block-stm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_149_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_150_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_150_21" title="Not referenced">ToMetaListExpr</span></span> =        <span class="cons_Lit">"block-stm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_163_3" id="BlockStatement_150_63" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>


  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_153_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_153_21" title="Not referenced">ToMetaExpr</span></span>     =         <span class="cons_Lit">"java:stm"</span>  <span class="cons_Lit">"|["</span> <a href="#Statement_168_3" id="Statement_153_63" title="Defined at line 168, 169, 183, 184">Statement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_154_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_154_21" title="Not referenced">ToMetaExpr</span></span>     =              <span class="cons_Lit">"stm"</span>  <span class="cons_Lit">"|["</span> <a href="#Statement_168_3" id="Statement_154_63" title="Defined at line 168, 169, 183, 184">Statement</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_156_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_156_21" title="Not referenced">ToMetaListExpr</span></span> =      <span class="cons_Lit">"switch-group"</span> <span class="cons_Lit">"|["</span> <a href="#SwitchGroup_175_3" id="SwitchGroup_156_63" title="Defined at line 175, 176">SwitchGroup</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_157_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_157_21" title="Not referenced">ToMetaListExpr</span></span> = <span class="cons_Lit">"java:switch-group"</span> <span class="cons_Lit">"|["</span> <a href="#SwitchGroup_175_3" id="SwitchGroup_157_63" title="Defined at line 175, 176">SwitchGroup</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Statements</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#BlockStatement_136_63" id="BlockStatement_163_3" title="Referenced at line 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 165, 166, 187, 188">BlockStatement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_163_18" title="Not referenced">FromMetaExpr</span></span>  = <span class="cons_Lit">"~"</span>       <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_163_44" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#BlockStatement_136_63" id="BlockStatement_164_3" title="Referenced at line 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 165, 166, 187, 188">BlockStatement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_164_18" title="Not referenced">FromMetaExpr</span></span>  = <span class="cons_Lit">"~bstm:"</span>  <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_164_44" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#BlockStatement_163_3" id="BlockStatement_165_3" title="Defined at line 163, 164, 185, 186">BlockStatement</a>*.<span class="cons_Constructor">FromMetaExpr</span> = <span class="cons_Lit">"~*"</span>      <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_165_44" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#BlockStatement_163_3" id="BlockStatement_166_3" title="Defined at line 163, 164, 185, 186">BlockStatement</a>*.<span class="cons_Constructor">FromMetaExpr</span> = <span class="cons_Lit">"~bstm*:"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_166_44" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

  <a href="#Statement_153_63" id="Statement_168_3" title="Referenced at line 153, 154">Statement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_168_13" title="Not referenced">FromMetaExpr</span></span>       = <span class="cons_Lit">"~stm:"</span>   <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_168_44" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> {<span class="keyword">prefer</span>}
  <a href="#Statement_153_63" id="Statement_169_3" title="Referenced at line 153, 154">Statement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_169_13" title="Not referenced">FromMetaExpr</span></span>       = <span class="cons_Lit">"~"</span>       <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_169_44" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

  <a href="#SwitchGroup_175_3" id="SwitchGroup_171_3" title="Defined at line 175, 176">SwitchGroup</a>*.<span class="cons_Constructor">FromMetaExpr</span>    =   <span class="cons_Lit">"~*"</span>              <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_171_54" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#SwitchGroup_175_3" id="SwitchGroup_172_3" title="Defined at line 175, 176">SwitchGroup</a>*.<span class="cons_Constructor">FromMetaExpr</span>    =   <span class="cons_Lit">"~switch-group*:"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_172_54" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>


  <a href="#SwitchGroup_156_63" id="SwitchGroup_175_3" title="Referenced at line 156, 157, 171, 172">SwitchGroup</a>.<span class="cons_Constructor"><span id="FromMetaExpr_175_15" title="Not referenced">FromMetaExpr</span></span>     = <span class="cons_Lit">"~"</span>               <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_175_52" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#SwitchGroup_156_63" id="SwitchGroup_176_3" title="Referenced at line 156, 157, 171, 172">SwitchGroup</a>.<span class="cons_Constructor"><span id="FromMetaExpr_176_15" title="Not referenced">FromMetaExpr</span></span>     = <span class="cons_Lit">"~switch-group:"</span>  <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_176_52" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Variables for Statements</span>
<span class="layout">///</span>
<span class="keyword">variables</span>

  <a href="#Statement_153_63" id="Statement_183_3" title="Referenced at line 153, 154">Statement</a>       = <span class="cons_Lit">"stm"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#Statement_153_63" id="Statement_184_3" title="Referenced at line 153, 154">Statement</a>       = <span class="cons_Lit">"stm_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_136_63" id="BlockStatement_185_3" title="Referenced at line 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 165, 166, 187, 188">BlockStatement</a>  = <span class="cons_Lit">"bstm"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_136_63" id="BlockStatement_186_3" title="Referenced at line 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 165, 166, 187, 188">BlockStatement</a>  = <span class="cons_Lit">"bstm_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_163_3" id="BlockStatement_187_3" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* = <span class="cons_Lit">"bstm"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_163_3" id="BlockStatement_188_3" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* = <span class="cons_Lit">"bstm_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}

<span class="layout">///</span>
<span class="layout">// Quotations for Expressions</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_194_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_194_21" title="Not referenced">ToMetaExpr</span></span> =         <span class="cons_Lit">"e"</span> <span class="cons_Lit">"|["</span> <a href="#Expression_204_3" id="Expression_194_51" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_195_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_195_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java:expr"</span> <span class="cons_Lit">"|["</span> <a href="#Expression_204_3" id="Expression_195_51" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_196_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_196_21" title="Not referenced">ToMetaExpr</span></span> =      <span class="cons_Lit">"expr"</span> <span class="cons_Lit">"|["</span> <a href="#Expression_204_3" id="Expression_196_51" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_197_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_197_21" title="Not referenced">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>      <span class="cons_Lit">"|["</span> <a href="#Expression_204_3" id="Expression_197_51" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_198_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_198_21" title="Not referenced">ToMetaExpr</span></span> =             <span class="cons_Lit">"|["</span> <a href="#Expression_204_3" id="Expression_198_51" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Expressions</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#Expression_194_51" id="Expression_204_3" title="Referenced at line 194, 195, 196, 197, 198, 214, 215">Expression</a>.<span class="cons_Constructor"><span id="FromMetaExpr_204_14" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>      <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_204_38" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#Expression_194_51" id="Expression_205_3" title="Referenced at line 194, 195, 196, 197, 198, 214, 215">Expression</a>.<span class="cons_Constructor"><span id="FromMetaExpr_205_14" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~e:"</span>    <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_205_38" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> {<span class="keyword">prefer</span>}
  <a href="#Expression_194_51" id="Expression_206_3" title="Referenced at line 194, 195, 196, 197, 198, 214, 215">Expression</a>.<span class="cons_Constructor"><span id="FromMetaExpr_206_14" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~expr:"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_206_38" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> {<span class="keyword">prefer</span>}

<span class="layout">///</span>
<span class="layout">// Variables for Expressions</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#Expression_194_51" id="Expression_212_3" title="Referenced at line 194, 195, 196, 197, 198, 214, 215">Expression</a>        = <span class="cons_Lit">"e"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#Expression_194_51" id="Expression_213_3" title="Referenced at line 194, 195, 196, 197, 198, 214, 215">Expression</a>        = <span class="cons_Lit">"e_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  {<a href="#Expression_204_3" id="Expression_214_4" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">","</span>}* = <span class="cons_Lit">"e"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}
  {<a href="#Expression_204_3" id="Expression_215_4" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">","</span>}* = <span class="cons_Lit">"e_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}

<span class="keyword">lexical syntax</span>
  <a href="#ID_249_3" id="ID_218_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"e"</span>  [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*       {<span class="keyword">reject</span>}
  <a href="#ID_249_3" id="ID_219_3" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"e_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

<span class="layout">///</span>
<span class="layout">// Anti Quotations for LeftHandSide of Assignment</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <span id="LHS_225_3" title="Not referenced">LHS</span>.<span class="cons_Constructor"><span id="FromMetaExpr_225_7" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>     <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_225_30" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <span id="LHS_226_3" title="Not referenced">LHS</span>.<span class="cons_Constructor"><span id="FromMetaExpr_226_7" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~lhs:"</span>  <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_226_31" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Quotations for Id</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_62_42" id="StrategoLang-Term_232_3" title="Referenced at line 62, 63, 82, 83, 85, 86, 163, 164, 165, 166, 168, 169, 171, 172, 175, 176, 204, 205, 206, 225, 226, 237, 238, 239, 255, 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_232_21" title="Not referenced">ToMetaExpr</span></span>    = <span class="cons_Lit">"ident"</span> <span class="cons_Lit">"|["</span> Id <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for ID</span>
<span class="layout">///</span>
  <a href="#ID_249_3" id="ID_237_3" title="Referenced at line 249">ID</a>.<span class="cons_Constructor"><span id="FromMetaExpr_237_6" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>     <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_237_29" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#ID_249_3" id="ID_238_3" title="Referenced at line 249">ID</a>.<span class="cons_Constructor"><span id="FromMetaExpr_238_6" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~id:"</span>  <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_238_29" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#ID_249_3" id="ID_239_3" title="Referenced at line 249">ID</a>.<span class="cons_Constructor"><span id="FromMetaExpr_239_6" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~idd:"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_239_29" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> <span class="cons_Lit">":"</span>

<span class="layout">///</span>
<span class="layout">// Variables for ID</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#ID_249_3" id="ID_245_3" title="Referenced at line 249">ID</a> = [<span class="cons_Regular">x</span><span class="cons_Regular">y</span><span class="cons_Regular">z</span>]            [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">prefer</span>}
  <a href="#ID_249_3" id="ID_246_3" title="Referenced at line 249">ID</a> = [<span class="cons_Regular">x</span><span class="cons_Regular">y</span><span class="cons_Regular">z</span>] [\_] [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">prefer</span>}

<span class="keyword">context-free restrictions</span>
  <a href="#ID_112_3" id="ID_249_3" title="Defined at line 112, 113, 114, 115, 117, 118, 119, 120, 122, 123, 124, 125, 218, 219, 237, 238, 239, 245, 246">ID</a> -/- [\_<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Literal</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <span id="StringLit_255_3" title="Not referenced">StringLit</span>.<span class="cons_Constructor"><span id="FromMetaExpr_255_13" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>        <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_255_39" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <span id="StringLit_256_3" title="Not referenced">StringLit</span>.<span class="cons_Constructor"><span id="FromMetaExpr_256_13" title="Not referenced">FromMetaExpr</span></span> = <span class="cons_Lit">"~strlit:"</span> <a href="#StrategoLang-Term_22_3" id="StrategoLang-Term_256_39" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">//  SingleChar.FromMetaExpr =     "~" &lt;StrategoLang-Term-CF&gt; &lt;LAYOUT?-CF&gt;  {prefer}</span>

<span class="layout">//exports</span>
<span class="layout">//  variables</span>
<span class="layout">//  DeciLiteral =     [ij]  [0-9\']* {prefer}</span>
<span class="layout">//  DeciLiteral =     [ij]  [\_] [a-zA-Z0-9\']* {prefer}</span>

<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "var-init" "|[" VariableInitializer "]|"</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Statements</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Variables for Statements</span>
<span class="layout">//   ///</span>
<span class="layout">//  variables</span>
<span class="layout">//  Statement =     "stm"  [0-9\']*         {prefer}</span>
<span class="layout">//  Statement =     "stm_" [a-zA-Z0-9\']*         {prefer}</span>
<span class="layout">//  BlockStatement =     "bstm" [0-9\']*    {prefer}</span>
<span class="layout">//  BlockStatement =     "bstm_" [a-zA-Z0-9\']*    {prefer}</span>
<span class="layout">//  BlockStatement* =     "bstm" [0-9\']* "*"   {prefer}</span>
<span class="layout">//  BlockStatement* =     "bstm_" [a-zA-Z0-9\']* "*"   {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotations for Statements</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:bstm"  "|[" BlockStatement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "bstm"  "|[" BlockStatement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"       "|[" BlockStatement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                  "|[" BlockStatement "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =     "java:bstm*" "|[" BlockStatement* "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =          "bstm*" "|[" BlockStatement* "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:block-stm"  "|[" BlockStatement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "block-stm"  "|[" BlockStatement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"            "|[" BlockStatement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                       "|[" BlockStatement "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =     "java:block-stm*" "|[" BlockStatement* "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =          "block-stm*" "|[" BlockStatement* "]|"</span>
<span class="layout">//</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:stm"  "|[" Statement "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "stm"  "|[" Statement "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =          "switch-group" "|[" SwitchGroup "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =     "java:switch-group" "|[" SwitchGroup "]|"</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Anti Quotations for Statements</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  BlockStatement.FromMetaExpr =     "~"       StrategoLang-Term</span>
<span class="layout">//  BlockStatement.FromMetaExpr =     "~bstm:"  StrategoLang-Term</span>
<span class="layout">//  BlockStatement*.FromMetaExpr =     "~*"      StrategoLang-Term</span>
<span class="layout">//  BlockStatement*.FromMetaExpr =     "~bstm*:" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  Statement.FromMetaExpr =     "~stm:"   StrategoLang-Term {prefer}</span>
<span class="layout">//  Statement.FromMetaExpr =     "~"       StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  SwitchGroup*.FromMetaExpr =     "~*"              StrategoLang-Term</span>
<span class="layout">//  SwitchGroup*.FromMetaExpr =     "~switch-group*:" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  SwitchGroup.FromMetaExpr =     "~"               StrategoLang-Term</span>
<span class="layout">//  SwitchGroup.FromMetaExpr =     "~switch-group:"  StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Variable Declarations</span>
<span class="layout">// ///</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Variables for Variable Declarations</span>
<span class="layout">//   ///</span>
<span class="layout">//  variables</span>
<span class="layout">//  LocalVariableDeclaration =     "lvdec" [0-9]*    {prefer}</span>
<span class="layout">//  LocalVariableDeclaration =     "lvdec_" [a-zA-Z0-9]*    {prefer}</span>
<span class="layout">//  VarDecl =      "vdec" [0-9]*         {prefer}</span>
<span class="layout">//  VarDecl =      "vdec_" [a-zA-Z0-9]*         {prefer}</span>
<span class="layout">//     "vdec"  [0-9]* "*"       -&gt; {VarDecl ","}+  {prefer}</span>
<span class="layout">//     "vdec_" [a-zA-Z0-9]* "*" -&gt; {VarDecl ","}+  {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  lexical syntax</span>
<span class="layout">//  ID =     "lvdec" {reject}</span>
<span class="layout">//  ID =     "lvdec_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//  ID =      "vdec" {reject}</span>
<span class="layout">//  ID =      "vdec_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotations for Local Variable Declarations</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:lvdec"  "|[" LocalVariableDeclaration "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "lvdec"  "|[" LocalVariableDeclaration "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:vdec" "|[" VarDecl "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "vdec" "|[" VarDecl "]|"</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Anti Quotations for Local Variable Declarations</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // LeftHandSide of Assignment</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Variables for LeftHandSide of Assignment</span>
<span class="layout">//   ///</span>
<span class="layout">//  variables</span>
<span class="layout">//  LHS =     "lhs" [0-9\']* {prefer}</span>
<span class="layout">//  LHS =     "e"   [0-9\']* {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  lexical syntax</span>
<span class="layout">//  ID =     "lhs" [0-9\']* {reject}</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Types</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Variables for Types</span>
<span class="layout">//   ///</span>
<span class="layout">//  variables</span>
<span class="layout">//  Type =     MetaTypeVar     {prefer}</span>
<span class="layout">//  PrimType =     MetaPrimTypeVar {prefer}</span>
<span class="layout">//  RefType =     MetaRefTypeVar  {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  lexical syntax</span>
<span class="layout">//  MetaTypeVar =     "t"  [0-9\']*</span>
<span class="layout">//  MetaTypeVar =     "t_" [a-zA-Z0-9\']*</span>
<span class="layout">//  MetaTypeVar =     "ty" [0-9]*</span>
<span class="layout">//  MetaTypeVar =     "ty_" [a-zA-Z0-9\']*</span>
<span class="layout">//</span>
<span class="layout">//  MetaPrimTypeVar =     "primt"  [0-9]*</span>
<span class="layout">//  MetaPrimTypeVar =     "primt_" [a-zA-Z0-9]*</span>
<span class="layout">//  MetaPrimTypeVar =     "primty" [0-9]*</span>
<span class="layout">//  MetaPrimTypeVar =     "primty_" [a-zA-Z0-9]*</span>
<span class="layout">//  MetaRefTypeVar =     "reft"   [0-9]*</span>
<span class="layout">//  MetaRefTypeVar =     "reft_" [a-zA-Z0-9]*</span>
<span class="layout">//  MetaRefTypeVar =     "refty"  [0-9]*</span>
<span class="layout">//  MetaRefTypeVar =     "refty_" [a-zA-Z0-9]*</span>
<span class="layout">//</span>
<span class="layout">//  ID =     "t"  [0-9\']* {reject}</span>
<span class="layout">//  ID =     "t_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//  ID =     "ty" [0-9]* {reject}</span>
<span class="layout">//  ID =     "ty_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//  ID =     "primt"  [0-9]* {reject}</span>
<span class="layout">//  ID =     "primt_" [a-zA-Z0-9]*  {reject}</span>
<span class="layout">//  ID =     "primty" [0-9]* {reject}</span>
<span class="layout">//  ID =     "primty_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//  ID =     "reft"   [0-9]* {reject}</span>
<span class="layout">//  ID =     "reft_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//  ID =     "refty"  [0-9]* {reject}</span>
<span class="layout">//  ID =     "refty_" [a-zA-Z0-9]* {reject}</span>
<span class="layout">//</span>
<span class="layout">//  lexical restrictions</span>
<span class="layout">//    MetaTypeVar -/- [a-zA-Z0-9\_\$\']</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotation for Types</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =             "t" "|[" Type "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =            "ty" "|[" Type "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:type" "|[" Type "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "type" "|[" Type "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"      "|[" Type "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                 "|[" Type "]|"</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Anti-Quotation for Types</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  Type.FromMetaExpr =     "~"       StrategoLang-Term</span>
<span class="layout">//  Type.FromMetaExpr =     "~type:"  StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Names</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Variables for Names</span>
<span class="layout">//   ///</span>
<span class="layout">//  variables</span>
<span class="layout">//  AmbName =     "ambname"  [0-9]*    {prefer}</span>
<span class="layout">//  AmbName =     "ambname_" [a-zA-Z0-9]*    {prefer}</span>
<span class="layout">//  ExprName =     "ename"    [0-9]*   {prefer}</span>
<span class="layout">//  ExprName =     "ename_" [a-zA-Z0-9]*   {prefer}</span>
<span class="layout">//  MethodName =     "fname"    [0-9]* {prefer}</span>
<span class="layout">//  MethodName =     "fname_" [a-zA-Z0-9]* {prefer}</span>
<span class="layout">//  TypeName =     "tname"    [0-9]*   {prefer}</span>
<span class="layout">//  TypeName =     "tname_" [a-zA-Z0-9]*   {prefer}</span>
<span class="layout">//  PackageOrTypeName =     "pkgtname" [0-9]*  {prefer}</span>
<span class="layout">//  PackageOrTypeName =     "pkgtname_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//  PackageName =     "pkgname" [0-9]*  {prefer}</span>
<span class="layout">//  PackageName =     "pkgname_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotations for Names</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "ambname"  "|[" AmbName    "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "ename"    "|[" ExprName   "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "fname"    "|[" MethodName "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "tname"    "|[" TypeName   "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "pkgtname" "|[" PackageOrTypeName "]|"</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Modifiers</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Variables for Modifiers</span>
<span class="layout">//   ///</span>
<span class="layout">//  variables</span>
<span class="layout">//  MethodMod =      "mod" [0-9]*  {prefer}</span>
<span class="layout">//  MethodMod =      "mod_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//  (Annotation =      "mod" [0-9]* "*" | MethodMod)* {prefer}</span>
<span class="layout">//  (Annotation =      "mod_" [a-zA-Z0-9]* "*" | MethodMod)* {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  ClassMod =      "mod" [0-9]*  {prefer}</span>
<span class="layout">//  ClassMod =      "mod_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//  (Annotation | ClassMod)* {prefer} =      "mod" [0-9]* "*"</span>
<span class="layout">//  (Annotation | ClassMod)* {prefer} =      "mod_" [a-zA-Z0-9]* "*"</span>
<span class="layout">//</span>
<span class="layout">//  ConstrMod =      "mod" [0-9]*  {prefer}</span>
<span class="layout">//  ConstrMod =      "mod_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//  (Annotation | ConstrMod)* =      "mod" [0-9]* "*" {prefer}</span>
<span class="layout">//  (Annotation | ConstrMod)* =      "mod_" [a-zA-Z0-9]* "*" {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  VarMod =      "mod" [0-9]*  {prefer}</span>
<span class="layout">//  VarMod =      "mod_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//  (Annotation | VarMod)* =      "mod" [0-9]* "*" {prefer}</span>
<span class="layout">//  (Annotation | VarMod)* =      "mod_" [a-zA-Z0-9]* "*" {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  FieldMod =      "mod" [0-9]*  {prefer}</span>
<span class="layout">//  FieldMod =      "mod_" [a-zA-Z0-9]*  {prefer}</span>
<span class="layout">//  (Annotation | FieldMod)* =      "mod" [0-9]* "*" {prefer}</span>
<span class="layout">//  (Annotation | FieldMod)* =      "mod_" [a-zA-Z0-9]* "*" {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotations for Modifiers</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =            "|[" FieldModifier "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "mod"  "|[" FieldModifier "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "anno" "|[" Annotation "]|"</span>
<span class="layout">//</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Package Declarations</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotations</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:package-dec" "|[" PackageDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "package-dec" "|[" PackageDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                        "|[" PackageDec  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:package-dec?" "|[" PackageDec? "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "package-dec?" "|[" PackageDec? "]|"</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Anti Quotations</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  PackageDec.FromMetaExpr =     "~package-dec:"  StrategoLang-Term</span>
<span class="layout">//  PackageDec?.FromMetaExpr =     "~package-dec?:" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Import Declarations</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Quotations for Import Declarations</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:import-dec"  "|[" ImportDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "import-dec"  "|[" ImportDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                        "|[" ImportDec  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =     "java:import-dec*" "|[" ImportDec* "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =          "import-dec*" "|[" ImportDec* "]|"</span>
<span class="layout">//</span>
<span class="layout">//  ///</span>
<span class="layout">//   // Anti Quotations for Import Declarations</span>
<span class="layout">//   ///</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//</span>
<span class="layout">//  ImportDec.FromMetaExpr =     "~import-dec:"  StrategoLang-Term</span>
<span class="layout">//  ImportDec*.FromMetaExpr =     "~import-dec*:" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">/////</span>
<span class="layout">// // Must be cleaned up</span>
<span class="layout">// ///</span>
<span class="layout">//exports</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =             "e" "|[" Expr "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:expr" "|[" Expr "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "expr" "|[" Expr "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"      "|[" Expr "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                 "|[" Expr "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:compilation-unit" "|[" CompilationUnit "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "compilation-unit" "|[" CompilationUnit "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"                  "|[" CompilationUnit "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                             "|[" CompilationUnit "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:importdecl" "|[" ImportDec "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "importdecl" "|[" ImportDec "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"            "|[" ImportDec "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:type-dec" "|[" TypeDec "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "type-dec" "|[" TypeDec "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"          "|[" TypeDec "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                     "|[" TypeDec "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:class-body-dec" "|["  ClassBodyDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "class-body-dec" "|["  ClassBodyDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"                "|["  ClassBodyDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                           "|["  ClassBodyDec  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:interface-member-dec" "|[" InterfaceMemberDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "interface-member-dec" "|[" InterfaceMemberDec  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:constant-dec" "|[" ConstantDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "constant-dec" "|[" ConstantDec  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:class-body-dec*" "|[" ClassBodyDec* "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "class-body-dec*" "|[" ClassBodyDec* "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"                 "|[" ClassBodyDec* "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaListExpr =                            "|[" ClassBodyDec* "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:stm" "|["  Stm "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "stm" "|["  Stm "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:imember-dec" "|["  AbstractMethodDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "imember-dec" "|["  AbstractMethodDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"             "|["  AbstractMethodDec  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                        "|["  AbstractMethodDec  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java:imember-dec*" "|["  AbstractMethodDec*  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =          "imember-dec*" "|["  AbstractMethodDec*  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =     "java"              "|["  AbstractMethodDec*  "]|"</span>
<span class="layout">//  StrategoLang-Term.ToMetaExpr =                         "|["  AbstractMethodDec*  "]|"</span>
<span class="layout">//</span>
<span class="layout">//  // Anti-quotation</span>
<span class="layout">//  context-free syntax</span>
<span class="layout">//</span>
<span class="layout">//  Name.FromMetaExpr =     "~"      StrategoLang-Term</span>
<span class="layout">//  Name.FromMetaExpr =     "~name:" StrategoLang-Term</span>
<span class="layout">//  Name.FromMetaExpr =     "~*:"    StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  Id.FromMetaExpr =     "~"     StrategoLang-Term</span>
<span class="layout">//  Id.FromMetaExpr =     "~id:"  StrategoLang-Term</span>
<span class="layout">//  Id.FromMetaExpr =     "~idd:" StrategoLang-Term ":"</span>
<span class="layout">//</span>
<span class="layout">//  ID.FromMetaExpr =     "~x:" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  TypeParam.FromMetaExpr =     "~"  StrategoLang-Term</span>
<span class="layout">//  {TypeParam ","}+.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  {ExceptionType ","}*.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  Expr.FromMetaExpr =     "~"      StrategoLang-Term</span>
<span class="layout">//  Expr.FromMetaExpr =     "~e:"    StrategoLang-Term {prefer}</span>
<span class="layout">//  Expr.FromMetaExpr =     "~expr:" StrategoLang-Term {prefer}</span>
<span class="layout">//</span>
<span class="layout">//  {Expr ","}*.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//  {VarInit ","}*.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  TypeDec.FromMetaExpr =     "~"  StrategoLang-Term</span>
<span class="layout">//  TypeDec*.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  ClassBodyDec.FromMetaExpr =     "~"  StrategoLang-Term</span>
<span class="layout">//  ClassBodyDec*.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  InterfaceMemberDec.FromMetaExpr =     "~"  StrategoLang-Term</span>
<span class="layout">//  InterfaceMemberDec*.FromMetaExpr =     "~*" StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  DeciLiteral.FromMetaExpr =     "~i:"      StrategoLang-Term</span>
<span class="layout">//  DeciLiteral.FromMetaExpr =     "~deci:"   StrategoLang-Term</span>
<span class="layout">//  HexaLiteral.FromMetaExpr =     "~hexa:"   StrategoLang-Term</span>
<span class="layout">//  OctaLiteral.FromMetaExpr =     "~octa:"   StrategoLang-Term</span>
<span class="layout">//  FloatLiteral.FromMetaExpr =     "~float:"  StrategoLang-Term</span>
<span class="layout">//  StringLiteral.FromMetaExpr =     "~string:" StrategoLang-Term</span>
<span class="layout">//  CharLiteral.FromMetaExpr =     "~char:"   StrategoLang-Term</span>
<span class="layout">//</span>
<span class="layout">//  syntax</span>
<span class="layout">//  StringChars.FromMetaExpr =     "~" &lt;StrategoLang-Term-CF&gt; {prefer}</span>
<span class="layout">//  SingleChar.FromMetaExpr =     "~" &lt;StrategoLang-Term-CF&gt; &lt;LAYOUT?-CF&gt;  {prefer}</span>

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
