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
<td class="code"><pre><code><span class="keyword">module</span> <span id="Java_StrategoMix_7_23" title="Not referenced locally, nor via imports">Java_StrategoMix</span>

<span class="keyword">imports</span>
  <a href="../java/packages/CompilationUnits.sdf3#java/packages/CompilationUnits_7_37" id="java/packages/CompilationUnits_35_65" title="Defined at ../java/packages/CompilationUnits.sdf3 line 1">java/packages/CompilationUnits</a>

  StrategoLang/import-namespaced
  StrategoLang/sugar/terms-namespaced
  StrategoLang/core/identifiers-namespaced

<span class="keyword">context-free start-symbols</span>

  <a href="#Module_243_249" id="Module_212_218" title="Defined at line 16">Module</a>

<span class="keyword">context-free syntax</span>

  <a href="#Module_212_218" id="Module_243_249" title="Referenced at line 12">Module</a> = StrategoLang-Module

<span class="layout">///</span>
<span class="layout">// Quotations for CompilationUnit</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_337_354" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_355_365" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java:compilation-unit"</span> <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3#CompilationUnit_202_217" id="CompilationUnit_397_412" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_420_437" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_438_448" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =      <span class="cons_Lit">"compilation-unit"</span> <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3#CompilationUnit_202_217" id="CompilationUnit_480_495" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_503_520" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_521_531" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>                  <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3#CompilationUnit_202_217" id="CompilationUnit_563_578" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_586_603" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_604_614" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =                         <span class="cons_Lit">"|["</span> <a href="../java/packages/CompilationUnits.sdf3#CompilationUnit_202_217" id="CompilationUnit_646_661" title="Defined at ../java/packages/CompilationUnits.sdf3 line 12, 17">CompilationUnit</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Variables for Formal Parameters</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#FormalParam_2193_2204" id="FormalParam_723_734" title="Referenced at line 63">FormalParam</a>  = <span class="cons_Lit">"param"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <a href="#FormalParam_2193_2204" id="FormalParam_776_787" title="Referenced at line 63">FormalParam</a>  = <span class="cons_Lit">"param_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <span id="FormalParams_829_841" title="Not referenced locally, nor via imports">FormalParams</span> = <span class="cons_Lit">"params"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <span id="FormalParams_882_894" title="Not referenced locally, nor via imports">FormalParams</span> = <span class="cons_Lit">"params_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]*     {<span class="keyword">prefer</span>}
  <span id="FormalParams_935_947" title="Not referenced locally, nor via imports">FormalParams</span> = <span class="cons_Lit">"param"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}
  <span id="FormalParams_988_1000" title="Not referenced locally, nor via imports">FormalParams</span> = <span class="cons_Lit">"param_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>]* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}

<span class="layout">///</span>
<span class="layout">// Quotations for Formal Parameters</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1106_1123" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1124_1134" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =             <span class="cons_Lit">"param"</span>  <span class="cons_Lit">"|["</span> <a href="#FormalParam_723_734" id="FormalParam_1163_1174" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1182_1199" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1200_1210" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =        <span class="cons_Lit">"java:param"</span>  <span class="cons_Lit">"|["</span> <a href="#FormalParam_723_734" id="FormalParam_1239_1250" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1259_1276" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1277_1287" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =             <span class="cons_Lit">"param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_723_734" id="FormalParam_1317_1328" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1342_1359" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1360_1370" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =        <span class="cons_Lit">"java:param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_723_734" id="FormalParam_1400_1411" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1426_1443" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1444_1454" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =  <span class="cons_Lit">"java:formal-param"</span> <span class="cons_Lit">"|["</span> <a href="#FormalParam_723_734" id="FormalParam_1483_1494" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1502_1519" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1520_1530" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =       <span class="cons_Lit">"formal-param"</span> <span class="cons_Lit">"|["</span> <a href="#FormalParam_723_734" id="FormalParam_1559_1570" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1578_1595" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1596_1606" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =  <span class="cons_Lit">"java"</span>              <span class="cons_Lit">"|["</span> <a href="#FormalParam_723_734" id="FormalParam_1635_1646" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1654_1671" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1672_1682" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =                      <span class="cons_Lit">"|["</span> <a href="#FormalParam_723_734" id="FormalParam_1711_1722" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1731_1748" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1749_1759" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java:formal-param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_723_734" id="FormalParam_1789_1800" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1814_1831" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1832_1842" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =      <span class="cons_Lit">"formal-param*"</span> <span class="cons_Lit">"|["</span> {<a href="#FormalParam_723_734" id="FormalParam_1872_1883" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1897_1914" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1915_1925" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>               <span class="cons_Lit">"|["</span> {<a href="#FormalParam_723_734" id="FormalParam_1955_1966" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_1980_1997" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_1998_2008" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =                      <span class="cons_Lit">"|["</span> {<a href="#FormalParam_723_734" id="FormalParam_2038_2049" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}* <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Formal Parameters</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
   <a href="#FormalParam_2193_2204" id="FormalParam_2134_2145" title="Referenced at line 63">FormalParam</a>.<span class="cons_Constructor"><span id="FromMetaExpr_2146_2158" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>       = <span class="cons_Lit">"~"</span>  <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_2172_2189" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  {<a href="#FormalParam_723_734" id="FormalParam_2193_2204" title="Defined at line 31, 32, 62">FormalParam</a> <span class="cons_Lit">","</span>}*.<span class="cons_Constructor">FromMetaExpr</span> = <span class="cons_Lit">"~*"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_2231_2248" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Anti-Quotation for Types</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2308_2325" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2326_2336" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =         <span class="cons_Lit">"t"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_2825_2834" id="UnannType_2356_2365" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2373_2390" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2391_2401" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =        <span class="cons_Lit">"ty"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_2825_2834" id="UnannType_2421_2430" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2439_2456" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2457_2467" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java:type"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_2825_2834" id="UnannType_2487_2496" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2504_2521" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2522_2532" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =      <span class="cons_Lit">"type"</span> <span class="cons_Lit">"|["</span> <a href="#UnannType_2825_2834" id="UnannType_2552_2561" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2569_2586" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2587_2597" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>      <span class="cons_Lit">"|["</span> <a href="#UnannType_2825_2834" id="UnannType_2617_2626" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2634_2651" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2652_2662" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =             <span class="cons_Lit">"|["</span> <a href="#UnannType_2825_2834" id="UnannType_2682_2691" title="Defined at line 82, 83, 92">UnannType</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_2699_2716" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_2717_2727" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =     <span class="cons_Lit">"rtype"</span> <span class="cons_Lit">"|["</span> <a href="#ReferenceType_2946_2959" id="ReferenceType_2747_2760" title="Defined at line 85, 86, 94">ReferenceType</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti-Quotation for Types</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#UnannType_2682_2691" id="UnannType_2825_2834" title="Referenced at line 75">UnannType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_2835_2847" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>     = <span class="cons_Lit">"~"</span>        <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_2865_2882" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#UnannType_2682_2691" id="UnannType_2885_2894" title="Referenced at line 75">UnannType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_2895_2907" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>     = <span class="cons_Lit">"~type:"</span>   <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_2925_2942" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

  <a href="#ReferenceType_2747_2760" id="ReferenceType_2946_2959" title="Referenced at line 76">ReferenceType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_2960_2972" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~refType"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_2986_3003" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#ReferenceType_2747_2760" id="ReferenceType_3006_3019" title="Referenced at line 76">ReferenceType</a>.<span class="cons_Constructor"><span id="FromMetaExpr_3020_3032" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~rtype:"</span>  <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_3046_3063" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Variables for Types</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#UnannType_2682_2691" id="UnannType_3108_3117" title="Referenced at line 75">UnannType</a>     = <a href="#MetaTypeVar_3254_3265" id="MetaTypeVar_3124_3135" title="Defined at line 97, 98, 99, 100">MetaTypeVar</a> {<span class="keyword">prefer</span>}
  <span id="PrimitiveType_3147_3160" title="Not referenced locally, nor via imports">PrimitiveType</span> = <a href="#MetaPrimTypeVar_3439_3454" id="MetaPrimTypeVar_3163_3178" title="Defined at line 102, 103, 104, 105">MetaPrimTypeVar</a> {<span class="keyword">prefer</span>}
  <a href="#ReferenceType_2747_2760" id="ReferenceType_3190_3203" title="Referenced at line 76">ReferenceType</a> = <a href="#MetaReferenceTypeVar_3640_3660" id="MetaReferenceTypeVar_3206_3226" title="Defined at line 107, 108, 109, 110">MetaReferenceTypeVar</a> {<span class="keyword">prefer</span>}

<span class="keyword">lexical syntax</span>
  <a href="#MetaTypeVar_4317_4328" id="MetaTypeVar_3254_3265" title="Referenced at line 128">MetaTypeVar</a>          = <span class="cons_Lit">"t"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaTypeVar_4317_4328" id="MetaTypeVar_3300_3311" title="Referenced at line 128">MetaTypeVar</a>          = <span class="cons_Lit">"t_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaTypeVar_4317_4328" id="MetaTypeVar_3346_3357" title="Referenced at line 128">MetaTypeVar</a>          = <span class="cons_Lit">"ty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaTypeVar_4317_4328" id="MetaTypeVar_3392_3403" title="Referenced at line 128">MetaTypeVar</a>          = <span class="cons_Lit">"ty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*

  <a href="#MetaPrimTypeVar_4362_4377" id="MetaPrimTypeVar_3439_3454" title="Referenced at line 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaPrimTypeVar_4362_4377" id="MetaPrimTypeVar_3489_3504" title="Referenced at line 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaPrimTypeVar_4362_4377" id="MetaPrimTypeVar_3539_3554" title="Referenced at line 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaPrimTypeVar_4362_4377" id="MetaPrimTypeVar_3589_3604" title="Referenced at line 129">MetaPrimTypeVar</a>      = <span class="cons_Lit">"primty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*

  <a href="#MetaReferenceTypeVar_4407_4427" id="MetaReferenceTypeVar_3640_3660" title="Referenced at line 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaReferenceTypeVar_4407_4427" id="MetaReferenceTypeVar_3687_3707" title="Referenced at line 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaReferenceTypeVar_4407_4427" id="MetaReferenceTypeVar_3734_3754" title="Referenced at line 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*
  <a href="#MetaReferenceTypeVar_4407_4427" id="MetaReferenceTypeVar_3781_3801" title="Referenced at line 130">MetaReferenceTypeVar</a> = <span class="cons_Lit">"rty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*

  <a href="#ID_8522_8524" id="ID_3829_3831" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"t"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_3866_3868" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"t_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_3903_3905" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"ty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_3940_3942" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"ty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

  <a href="#ID_8522_8524" id="ID_3978_3980" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_4019_4021" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_4060_4062" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_4101_4103" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"primty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

  <a href="#ID_8522_8524" id="ID_4143_4145" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rt"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_4181_4183" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rt_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_4219_4221" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rty"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_4257_4259" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"rty_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

<span class="keyword">lexical restrictions</span>
  <a href="#MetaTypeVar_3254_3265" id="MetaTypeVar_4317_4328" title="Defined at line 97, 98, 99, 100">MetaTypeVar</a>          -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$\']
  <a href="#MetaPrimTypeVar_3439_3454" id="MetaPrimTypeVar_4362_4377" title="Defined at line 102, 103, 104, 105">MetaPrimTypeVar</a>      -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$\']
  <a href="#MetaReferenceTypeVar_3640_3660" id="MetaReferenceTypeVar_4407_4427" title="Defined at line 107, 108, 109, 110">MetaReferenceTypeVar</a> -/- [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\_\$\']

<span class="layout">///</span>
<span class="layout">// Quotations for Statements</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_4510_4527" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_4528_4538" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =        <span class="cons_Lit">"java:bstm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_4570_4584" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_4592_4609" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_4610_4620" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =             <span class="cons_Lit">"bstm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_4652_4666" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_4674_4691" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_4692_4702" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =        <span class="cons_Lit">"java"</span>       <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_4734_4748" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_4756_4773" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_4774_4784" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =                     <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_4816_4830" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_4839_4856" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_4857_4871" title="Not referenced locally, nor via imports">ToMetaListExpr</span></span> =        <span class="cons_Lit">"java:bstm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_4899_4913" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_4922_4939" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_4940_4954" title="Not referenced locally, nor via imports">ToMetaListExpr</span></span> =             <span class="cons_Lit">"bstm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_4982_4996" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5006_5023" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_5024_5034" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =   <span class="cons_Lit">"java:block-stm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_5066_5080" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5088_5105" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_5106_5116" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =        <span class="cons_Lit">"block-stm"</span>  <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_5148_5162" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5170_5187" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_5188_5198" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =   <span class="cons_Lit">"java"</span>            <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_5230_5244" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5252_5269" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_5270_5280" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =                     <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_5312_5326" title="Defined at line 163, 164, 185, 186">BlockStatement</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5335_5352" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_5353_5367" title="Not referenced locally, nor via imports">ToMetaListExpr</span></span> =   <span class="cons_Lit">"java:block-stm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_5395_5409" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5418_5435" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_5436_5450" title="Not referenced locally, nor via imports">ToMetaListExpr</span></span> =        <span class="cons_Lit">"block-stm*"</span> <span class="cons_Lit">"|["</span> <a href="#BlockStatement_5879_5893" id="BlockStatement_5478_5492" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* <span class="cons_Lit">"]|"</span>


  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5503_5520" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_5521_5531" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =         <span class="cons_Lit">"java:stm"</span>  <span class="cons_Lit">"|["</span> <a href="#Statement_6124_6133" id="Statement_5563_5572" title="Defined at line 168, 169, 183, 184">Statement</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5580_5597" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_5598_5608" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>     =              <span class="cons_Lit">"stm"</span>  <span class="cons_Lit">"|["</span> <a href="#Statement_6124_6133" id="Statement_5640_5649" title="Defined at line 168, 169, 183, 184">Statement</a> <span class="cons_Lit">"]|"</span>

  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5658_5675" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_5676_5690" title="Not referenced locally, nor via imports">ToMetaListExpr</span></span> =      <span class="cons_Lit">"switch-group"</span> <span class="cons_Lit">"|["</span> <a href="#SwitchGroup_6400_6411" id="SwitchGroup_5718_5729" title="Defined at line 175, 176">SwitchGroup</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_5737_5754" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaListExpr_5755_5769" title="Not referenced locally, nor via imports">ToMetaListExpr</span></span> = <span class="cons_Lit">"java:switch-group"</span> <span class="cons_Lit">"|["</span> <a href="#SwitchGroup_6400_6411" id="SwitchGroup_5797_5808" title="Defined at line 175, 176">SwitchGroup</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Statements</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#BlockStatement_6866_6880" id="BlockStatement_5879_5893" title="Referenced at line 188">BlockStatement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_5894_5906" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>  = <span class="cons_Lit">"~"</span>       <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_5920_5937" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#BlockStatement_6866_6880" id="BlockStatement_5940_5954" title="Referenced at line 188">BlockStatement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_5955_5967" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>  = <span class="cons_Lit">"~bstm:"</span>  <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_5981_5998" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#BlockStatement_5879_5893" id="BlockStatement_6001_6015" title="Defined at line 163, 164, 185, 186">BlockStatement</a>*.<span class="cons_Constructor">FromMetaExpr</span> = <span class="cons_Lit">"~*"</span>      <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6042_6059" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#BlockStatement_5879_5893" id="BlockStatement_6062_6076" title="Defined at line 163, 164, 185, 186">BlockStatement</a>*.<span class="cons_Constructor">FromMetaExpr</span> = <span class="cons_Lit">"~bstm*:"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6103_6120" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

  <a href="#Statement_5640_5649" id="Statement_6124_6133" title="Referenced at line 154">Statement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_6134_6146" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>       = <span class="cons_Lit">"~stm:"</span>   <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6165_6182" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> {<span class="keyword">prefer</span>}
  <a href="#Statement_5640_5649" id="Statement_6194_6203" title="Referenced at line 154">Statement</a>.<span class="cons_Constructor"><span id="FromMetaExpr_6204_6216" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>       = <span class="cons_Lit">"~"</span>       <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6235_6252" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

  <a href="#SwitchGroup_6400_6411" id="SwitchGroup_6256_6267" title="Defined at line 175, 176">SwitchGroup</a>*.<span class="cons_Constructor">FromMetaExpr</span>    =   <span class="cons_Lit">"~*"</span>              <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6307_6324" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#SwitchGroup_6400_6411" id="SwitchGroup_6327_6338" title="Defined at line 175, 176">SwitchGroup</a>*.<span class="cons_Constructor">FromMetaExpr</span>    =   <span class="cons_Lit">"~switch-group*:"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6378_6395" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>


  <a href="#SwitchGroup_6327_6338" id="SwitchGroup_6400_6411" title="Referenced at line 172">SwitchGroup</a>.<span class="cons_Constructor"><span id="FromMetaExpr_6412_6424" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>     = <span class="cons_Lit">"~"</span>               <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6449_6466" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#SwitchGroup_6327_6338" id="SwitchGroup_6469_6480" title="Referenced at line 172">SwitchGroup</a>.<span class="cons_Constructor"><span id="FromMetaExpr_6481_6493" title="Not referenced locally, nor via imports">FromMetaExpr</span></span>     = <span class="cons_Lit">"~switch-group:"</span>  <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_6518_6535" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Variables for Statements</span>
<span class="layout">///</span>
<span class="keyword">variables</span>

  <a href="#Statement_5640_5649" id="Statement_6586_6595" title="Referenced at line 154">Statement</a>       = <span class="cons_Lit">"stm"</span>         [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#Statement_5640_5649" id="Statement_6642_6651" title="Referenced at line 154">Statement</a>       = <span class="cons_Lit">"stm_"</span>  [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_6866_6880" id="BlockStatement_6698_6712" title="Referenced at line 188">BlockStatement</a>  = <span class="cons_Lit">"bstm"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_6866_6880" id="BlockStatement_6754_6768" title="Referenced at line 188">BlockStatement</a>  = <span class="cons_Lit">"bstm_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_5879_5893" id="BlockStatement_6810_6824" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* = <span class="cons_Lit">"bstm"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}
  <a href="#BlockStatement_5879_5893" id="BlockStatement_6866_6880" title="Defined at line 163, 164, 185, 186">BlockStatement</a>* = <span class="cons_Lit">"bstm_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}

<span class="layout">///</span>
<span class="layout">// Quotations for Expressions</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_6981_6998" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_6999_7009" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =         <span class="cons_Lit">"e"</span> <span class="cons_Lit">"|["</span> <a href="#Expression_7375_7385" id="Expression_7029_7039" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_7047_7064" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_7065_7075" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java:expr"</span> <span class="cons_Lit">"|["</span> <a href="#Expression_7375_7385" id="Expression_7095_7105" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_7113_7130" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_7131_7141" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =      <span class="cons_Lit">"expr"</span> <span class="cons_Lit">"|["</span> <a href="#Expression_7375_7385" id="Expression_7161_7171" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_7179_7196" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_7197_7207" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> = <span class="cons_Lit">"java"</span>      <span class="cons_Lit">"|["</span> <a href="#Expression_7375_7385" id="Expression_7227_7237" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_7245_7262" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_7263_7273" title="Not referenced locally, nor via imports">ToMetaExpr</span></span> =             <span class="cons_Lit">"|["</span> <a href="#Expression_7375_7385" id="Expression_7293_7303" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Expressions</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#Expression_7772_7782" id="Expression_7375_7385" title="Referenced at line 215">Expression</a>.<span class="cons_Constructor"><span id="FromMetaExpr_7386_7398" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>      <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_7410_7427" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#Expression_7772_7782" id="Expression_7430_7440" title="Referenced at line 215">Expression</a>.<span class="cons_Constructor"><span id="FromMetaExpr_7441_7453" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~e:"</span>    <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_7465_7482" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> {<span class="keyword">prefer</span>}
  <a href="#Expression_7772_7782" id="Expression_7494_7504" title="Referenced at line 215">Expression</a>.<span class="cons_Constructor"><span id="FromMetaExpr_7505_7517" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~expr:"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_7529_7546" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> {<span class="keyword">prefer</span>}

<span class="layout">///</span>
<span class="layout">// Variables for Expressions</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#Expression_7772_7782" id="Expression_7606_7616" title="Referenced at line 215">Expression</a>        = <span class="cons_Lit">"e"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  <a href="#Expression_7772_7782" id="Expression_7661_7671" title="Referenced at line 215">Expression</a>        = <span class="cons_Lit">"e_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*     {<span class="keyword">prefer</span>}
  {<a href="#Expression_7375_7385" id="Expression_7717_7727" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">","</span>}* = <span class="cons_Lit">"e"</span>        [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}
  {<a href="#Expression_7375_7385" id="Expression_7772_7782" title="Defined at line 204, 205, 206, 212, 213">Expression</a> <span class="cons_Lit">","</span>}* = <span class="cons_Lit">"e_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* <span class="cons_Lit">"*"</span> {<span class="keyword">prefer</span>}

<span class="keyword">lexical syntax</span>
  <a href="#ID_8522_8524" id="ID_7842_7844" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"e"</span>  [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']*       {<span class="keyword">reject</span>}
  <a href="#ID_8522_8524" id="ID_7878_7880" title="Referenced at line 249">ID</a> = <span class="cons_Lit">"e_"</span> [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">reject</span>}

<span class="layout">///</span>
<span class="layout">// Anti Quotations for LeftHandSide of Assignment</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <span id="LHS_7993_7996" title="Not referenced locally, nor via imports">LHS</span>.<span class="cons_Constructor"><span id="FromMetaExpr_7997_8009" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>     <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8020_8037" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <span id="LHS_8040_8043" title="Not referenced locally, nor via imports">LHS</span>.<span class="cons_Constructor"><span id="FromMetaExpr_8044_8056" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~lhs:"</span>  <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8068_8085" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

<span class="layout">///</span>
<span class="layout">// Quotations for Id</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <a href="#StrategoLang-Term_8699_8716" id="StrategoLang-Term_8138_8155" title="Referenced at line 256">StrategoLang-Term</a>.<span class="cons_Constructor"><span id="ToMetaExpr_8156_8166" title="Not referenced locally, nor via imports">ToMetaExpr</span></span>    = <span class="cons_Lit">"ident"</span> <span class="cons_Lit">"|["</span> Id <span class="cons_Lit">"]|"</span>

<span class="layout">///</span>
<span class="layout">// Anti Quotations for ID</span>
<span class="layout">///</span>
  <a href="#ID_8522_8524" id="ID_8230_8232" title="Referenced at line 249">ID</a>.<span class="cons_Constructor"><span id="FromMetaExpr_8233_8245" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>     <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8256_8273" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#ID_8522_8524" id="ID_8276_8278" title="Referenced at line 249">ID</a>.<span class="cons_Constructor"><span id="FromMetaExpr_8279_8291" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~id:"</span>  <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8302_8319" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <a href="#ID_8522_8524" id="ID_8322_8324" title="Referenced at line 249">ID</a>.<span class="cons_Constructor"><span id="FromMetaExpr_8325_8337" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~idd:"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8348_8365" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a> <span class="cons_Lit">":"</span>

<span class="layout">///</span>
<span class="layout">// Variables for ID</span>
<span class="layout">///</span>
<span class="keyword">variables</span>
  <a href="#ID_8522_8524" id="ID_8411_8413" title="Referenced at line 249">ID</a> = [<span class="cons_Regular">x</span><span class="cons_Regular">y</span><span class="cons_Regular">z</span>]            [<span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">prefer</span>}
  <a href="#ID_8522_8524" id="ID_8453_8455" title="Referenced at line 249">ID</a> = [<span class="cons_Regular">x</span><span class="cons_Regular">y</span><span class="cons_Regular">z</span>] [\_] [<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']* {<span class="keyword">prefer</span>}

<span class="keyword">context-free restrictions</span>
  <a href="#ID_3829_3831" id="ID_8522_8524" title="Defined at line 112, 113, 114, 115, 117, 118, 119, 120, 122, 123, 124, 125, 218, 219, 237, 238, 239, 245, 246">ID</a> -/- [\_<span class="cons_Regular">a</span>-<span class="cons_Regular">z</span><span class="cons_Regular">A</span>-<span class="cons_Regular">Z</span><span class="cons_Regular">0</span>-<span class="cons_Regular">9</span>\']

<span class="layout">///</span>
<span class="layout">// Anti Quotations for Literal</span>
<span class="layout">///</span>
<span class="keyword">context-free syntax</span>
  <span id="StringLit_8607_8616" title="Not referenced locally, nor via imports">StringLit</span>.<span class="cons_Constructor"><span id="FromMetaExpr_8617_8629" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~"</span>        <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8643_8660" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>
  <span id="StringLit_8663_8672" title="Not referenced locally, nor via imports">StringLit</span>.<span class="cons_Constructor"><span id="FromMetaExpr_8673_8685" title="Not referenced locally, nor via imports">FromMetaExpr</span></span> = <span class="cons_Lit">"~strlit:"</span> <a href="#StrategoLang-Term_337_354" id="StrategoLang-Term_8699_8716" title="Defined at line 22, 23, 24, 25, 42, 43, 45, 46, 48, 49, 50, 51, 53, 54, 55, 56, 69, 70, 72, 73, 74, 75, 76, 136, 137, 138, 139, 141, 142, 144, 145, 146, 147, 149, 150, 153, 154, 156, 157, 194, 195, 196, 197, 198, 232">StrategoLang-Term</a>

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