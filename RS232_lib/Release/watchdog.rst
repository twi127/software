                              1 ;--------------------------------------------------------
                              2 ; File Created by SDCC : free open source ANSI-C Compiler
                              3 ; Version 3.1.0 #7066 (Nov 22 2011) (MINGW32)
                              4 ; This file was generated Mon Nov 19 22:13:55 2012
                              5 ;--------------------------------------------------------
                              6 	.module watchdog
                              7 	.optsdcc -mmcs51 --model-small
                              8 	
                              9 ;--------------------------------------------------------
                             10 ; Public variables in this module
                             11 ;--------------------------------------------------------
                             12 	.globl _P3_1
                             13 	.globl _P3_0
                             14 	.globl _P1_7
                             15 	.globl _P1_6
                             16 	.globl _P1_5
                             17 	.globl _P1_4
                             18 	.globl _P1_3
                             19 	.globl _P1_2
                             20 	.globl _P1_1
                             21 	.globl _P1_0
                             22 	.globl _P0_7
                             23 	.globl _P0_6
                             24 	.globl _P0_5
                             25 	.globl _P0_4
                             26 	.globl _P0_3
                             27 	.globl _P0_2
                             28 	.globl _P0_1
                             29 	.globl _P0_0
                             30 	.globl _I2CON_0
                             31 	.globl _I2CON_2
                             32 	.globl _I2CON_3
                             33 	.globl _I2CON_4
                             34 	.globl _I2CON_5
                             35 	.globl _I2CON_6
                             36 	.globl _SCON_7
                             37 	.globl _SCON_6
                             38 	.globl _SCON_5
                             39 	.globl _SCON_4
                             40 	.globl _SCON_3
                             41 	.globl _SCON_2
                             42 	.globl _SCON_1
                             43 	.globl _SCON_0
                             44 	.globl _IP0_0
                             45 	.globl _IP0_1
                             46 	.globl _IP0_2
                             47 	.globl _IP0_3
                             48 	.globl _IP0_4
                             49 	.globl _IP0_5
                             50 	.globl _IP0_6
                             51 	.globl _IP1_0
                             52 	.globl _IP1_1
                             53 	.globl _IP1_2
                             54 	.globl _IP1_6
                             55 	.globl _IEN1_0
                             56 	.globl _IEN1_1
                             57 	.globl _IEN1_2
                             58 	.globl _IEN0_0
                             59 	.globl _IEN0_1
                             60 	.globl _IEN0_2
                             61 	.globl _IEN0_3
                             62 	.globl _IEN0_4
                             63 	.globl _IEN0_5
                             64 	.globl _IEN0_6
                             65 	.globl _IEN0_7
                             66 	.globl _TCON_0
                             67 	.globl _TCON_1
                             68 	.globl _TCON_2
                             69 	.globl _TCON_3
                             70 	.globl _TCON_4
                             71 	.globl _TCON_5
                             72 	.globl _TCON_6
                             73 	.globl _TCON_7
                             74 	.globl _PSW_7
                             75 	.globl _PSW_6
                             76 	.globl _PSW_5
                             77 	.globl _PSW_4
                             78 	.globl _PSW_3
                             79 	.globl _PSW_2
                             80 	.globl _PSW_1
                             81 	.globl _PSW_0
                             82 	.globl _IEN1
                             83 	.globl _IP0H
                             84 	.globl _WFEED2
                             85 	.globl _WFEED1
                             86 	.globl _WDL
                             87 	.globl _WDCON
                             88 	.globl _TRIM
                             89 	.globl _TAMOD
                             90 	.globl _SSTAT
                             91 	.globl _RTCL
                             92 	.globl _RTCH
                             93 	.globl _RTCCON
                             94 	.globl _RSTSRC
                             95 	.globl _PT0AD
                             96 	.globl _PCONA
                             97 	.globl _P3M2
                             98 	.globl _P3M1
                             99 	.globl _P1M2
                            100 	.globl _P1M1
                            101 	.globl _P0M2
                            102 	.globl _P0M1
                            103 	.globl _KBPATN
                            104 	.globl _KBMASK
                            105 	.globl _KBCON
                            106 	.globl _IP1H
                            107 	.globl _IP1
                            108 	.globl _I2STAT
                            109 	.globl _I2SCLL
                            110 	.globl _I2SCLH
                            111 	.globl _I2DAT
                            112 	.globl _I2CON
                            113 	.globl _I2ADR
                            114 	.globl _FMDATA
                            115 	.globl _FMCON
                            116 	.globl _FMADRL
                            117 	.globl _FMADRH
                            118 	.globl _DIVM
                            119 	.globl _CMP2
                            120 	.globl _CMP1
                            121 	.globl _BRGCON
                            122 	.globl _BRGR1
                            123 	.globl _BRGR0
                            124 	.globl _SADEN
                            125 	.globl _SADDR
                            126 	.globl _AUXR1
                            127 	.globl _SBUF
                            128 	.globl _SCON
                            129 	.globl _IP0
                            130 	.globl _IEN0
                            131 	.globl _TH1
                            132 	.globl _TH0
                            133 	.globl _TL1
                            134 	.globl _TL0
                            135 	.globl _TMOD
                            136 	.globl _TCON
                            137 	.globl _PCON
                            138 	.globl _DPH
                            139 	.globl _DPL
                            140 	.globl _SP
                            141 	.globl _B
                            142 	.globl _ACC
                            143 	.globl _PSW
                            144 	.globl _P3
                            145 	.globl _P1
                            146 	.globl _P0
                            147 	.globl _watchdog_init
                            148 	.globl _watchdog_feed
                            149 	.globl _watchdog_start
                            150 	.globl _watchdog_stop
                            151 ;--------------------------------------------------------
                            152 ; special function registers
                            153 ;--------------------------------------------------------
                            154 	.area RSEG    (ABS,DATA)
   0000                     155 	.org 0x0000
                    0080    156 _P0	=	0x0080
                    0090    157 _P1	=	0x0090
                    00B0    158 _P3	=	0x00b0
                    00D0    159 _PSW	=	0x00d0
                    00E0    160 _ACC	=	0x00e0
                    00F0    161 _B	=	0x00f0
                    0081    162 _SP	=	0x0081
                    0082    163 _DPL	=	0x0082
                    0083    164 _DPH	=	0x0083
                    0087    165 _PCON	=	0x0087
                    0088    166 _TCON	=	0x0088
                    0089    167 _TMOD	=	0x0089
                    008A    168 _TL0	=	0x008a
                    008B    169 _TL1	=	0x008b
                    008C    170 _TH0	=	0x008c
                    008D    171 _TH1	=	0x008d
                    00A8    172 _IEN0	=	0x00a8
                    00B8    173 _IP0	=	0x00b8
                    0098    174 _SCON	=	0x0098
                    0099    175 _SBUF	=	0x0099
                    00A2    176 _AUXR1	=	0x00a2
                    00A9    177 _SADDR	=	0x00a9
                    00B9    178 _SADEN	=	0x00b9
                    00BE    179 _BRGR0	=	0x00be
                    00BF    180 _BRGR1	=	0x00bf
                    00BD    181 _BRGCON	=	0x00bd
                    00AC    182 _CMP1	=	0x00ac
                    00AD    183 _CMP2	=	0x00ad
                    0095    184 _DIVM	=	0x0095
                    00E7    185 _FMADRH	=	0x00e7
                    00E6    186 _FMADRL	=	0x00e6
                    00E4    187 _FMCON	=	0x00e4
                    00E5    188 _FMDATA	=	0x00e5
                    00DB    189 _I2ADR	=	0x00db
                    00D8    190 _I2CON	=	0x00d8
                    00DA    191 _I2DAT	=	0x00da
                    00DD    192 _I2SCLH	=	0x00dd
                    00DC    193 _I2SCLL	=	0x00dc
                    00D9    194 _I2STAT	=	0x00d9
                    00F8    195 _IP1	=	0x00f8
                    00F7    196 _IP1H	=	0x00f7
                    0094    197 _KBCON	=	0x0094
                    0086    198 _KBMASK	=	0x0086
                    0093    199 _KBPATN	=	0x0093
                    0084    200 _P0M1	=	0x0084
                    0085    201 _P0M2	=	0x0085
                    0091    202 _P1M1	=	0x0091
                    0092    203 _P1M2	=	0x0092
                    00B1    204 _P3M1	=	0x00b1
                    00B2    205 _P3M2	=	0x00b2
                    00B5    206 _PCONA	=	0x00b5
                    00F6    207 _PT0AD	=	0x00f6
                    00DF    208 _RSTSRC	=	0x00df
                    00D1    209 _RTCCON	=	0x00d1
                    00D2    210 _RTCH	=	0x00d2
                    00D3    211 _RTCL	=	0x00d3
                    00BA    212 _SSTAT	=	0x00ba
                    008F    213 _TAMOD	=	0x008f
                    0096    214 _TRIM	=	0x0096
                    00A7    215 _WDCON	=	0x00a7
                    00C1    216 _WDL	=	0x00c1
                    00C2    217 _WFEED1	=	0x00c2
                    00C3    218 _WFEED2	=	0x00c3
                    00B7    219 _IP0H	=	0x00b7
                    00E8    220 _IEN1	=	0x00e8
                            221 ;--------------------------------------------------------
                            222 ; special function bits
                            223 ;--------------------------------------------------------
                            224 	.area RSEG    (ABS,DATA)
   0000                     225 	.org 0x0000
                    00D0    226 _PSW_0	=	0x00d0
                    00D1    227 _PSW_1	=	0x00d1
                    00D2    228 _PSW_2	=	0x00d2
                    00D3    229 _PSW_3	=	0x00d3
                    00D4    230 _PSW_4	=	0x00d4
                    00D5    231 _PSW_5	=	0x00d5
                    00D6    232 _PSW_6	=	0x00d6
                    00D7    233 _PSW_7	=	0x00d7
                    008F    234 _TCON_7	=	0x008f
                    008E    235 _TCON_6	=	0x008e
                    008D    236 _TCON_5	=	0x008d
                    008C    237 _TCON_4	=	0x008c
                    008B    238 _TCON_3	=	0x008b
                    008A    239 _TCON_2	=	0x008a
                    0089    240 _TCON_1	=	0x0089
                    0088    241 _TCON_0	=	0x0088
                    00AF    242 _IEN0_7	=	0x00af
                    00AE    243 _IEN0_6	=	0x00ae
                    00AD    244 _IEN0_5	=	0x00ad
                    00AC    245 _IEN0_4	=	0x00ac
                    00AB    246 _IEN0_3	=	0x00ab
                    00AA    247 _IEN0_2	=	0x00aa
                    00A9    248 _IEN0_1	=	0x00a9
                    00A8    249 _IEN0_0	=	0x00a8
                    00EA    250 _IEN1_2	=	0x00ea
                    00E9    251 _IEN1_1	=	0x00e9
                    00E8    252 _IEN1_0	=	0x00e8
                    00FE    253 _IP1_6	=	0x00fe
                    00FA    254 _IP1_2	=	0x00fa
                    00F9    255 _IP1_1	=	0x00f9
                    00F8    256 _IP1_0	=	0x00f8
                    00BE    257 _IP0_6	=	0x00be
                    00BD    258 _IP0_5	=	0x00bd
                    00BC    259 _IP0_4	=	0x00bc
                    00BB    260 _IP0_3	=	0x00bb
                    00BA    261 _IP0_2	=	0x00ba
                    00B9    262 _IP0_1	=	0x00b9
                    00B8    263 _IP0_0	=	0x00b8
                    0098    264 _SCON_0	=	0x0098
                    0099    265 _SCON_1	=	0x0099
                    009A    266 _SCON_2	=	0x009a
                    009B    267 _SCON_3	=	0x009b
                    009C    268 _SCON_4	=	0x009c
                    009D    269 _SCON_5	=	0x009d
                    009E    270 _SCON_6	=	0x009e
                    009F    271 _SCON_7	=	0x009f
                    00DE    272 _I2CON_6	=	0x00de
                    00DD    273 _I2CON_5	=	0x00dd
                    00DC    274 _I2CON_4	=	0x00dc
                    00DB    275 _I2CON_3	=	0x00db
                    00DA    276 _I2CON_2	=	0x00da
                    00D8    277 _I2CON_0	=	0x00d8
                    0080    278 _P0_0	=	0x0080
                    0081    279 _P0_1	=	0x0081
                    0082    280 _P0_2	=	0x0082
                    0083    281 _P0_3	=	0x0083
                    0084    282 _P0_4	=	0x0084
                    0085    283 _P0_5	=	0x0085
                    0086    284 _P0_6	=	0x0086
                    0087    285 _P0_7	=	0x0087
                    0090    286 _P1_0	=	0x0090
                    0091    287 _P1_1	=	0x0091
                    0092    288 _P1_2	=	0x0092
                    0093    289 _P1_3	=	0x0093
                    0094    290 _P1_4	=	0x0094
                    0095    291 _P1_5	=	0x0095
                    0096    292 _P1_6	=	0x0096
                    0097    293 _P1_7	=	0x0097
                    00B0    294 _P3_0	=	0x00b0
                    00B1    295 _P3_1	=	0x00b1
                            296 ;--------------------------------------------------------
                            297 ; overlayable register banks
                            298 ;--------------------------------------------------------
                            299 	.area REG_BANK_0	(REL,OVR,DATA)
   0000                     300 	.ds 8
                            301 ;--------------------------------------------------------
                            302 ; overlayable bit register bank
                            303 ;--------------------------------------------------------
                            304 	.area BIT_BANK	(REL,OVR,DATA)
   0023                     305 bits:
   0023                     306 	.ds 1
                    8000    307 	b0 = bits[0]
                    8100    308 	b1 = bits[1]
                    8200    309 	b2 = bits[2]
                    8300    310 	b3 = bits[3]
                    8400    311 	b4 = bits[4]
                    8500    312 	b5 = bits[5]
                    8600    313 	b6 = bits[6]
                    8700    314 	b7 = bits[7]
                            315 ;--------------------------------------------------------
                            316 ; internal ram data
                            317 ;--------------------------------------------------------
                            318 	.area DSEG    (DATA)
                            319 ;--------------------------------------------------------
                            320 ; overlayable items in internal ram 
                            321 ;--------------------------------------------------------
                            322 	.area OSEG    (OVR,DATA)
                            323 ;--------------------------------------------------------
                            324 ; indirectly addressable internal ram data
                            325 ;--------------------------------------------------------
                            326 	.area ISEG    (DATA)
                            327 ;--------------------------------------------------------
                            328 ; absolute internal ram data
                            329 ;--------------------------------------------------------
                            330 	.area IABS    (ABS,DATA)
                            331 	.area IABS    (ABS,DATA)
                            332 ;--------------------------------------------------------
                            333 ; bit data
                            334 ;--------------------------------------------------------
                            335 	.area BSEG    (BIT)
                            336 ;--------------------------------------------------------
                            337 ; paged external ram data
                            338 ;--------------------------------------------------------
                            339 	.area PSEG    (PAG,XDATA)
                            340 ;--------------------------------------------------------
                            341 ; external ram data
                            342 ;--------------------------------------------------------
                            343 	.area XSEG    (XDATA)
                            344 ;--------------------------------------------------------
                            345 ; absolute external ram data
                            346 ;--------------------------------------------------------
                            347 	.area XABS    (ABS,XDATA)
                            348 ;--------------------------------------------------------
                            349 ; external initialized ram data
                            350 ;--------------------------------------------------------
                            351 	.area XISEG   (XDATA)
                            352 	.area HOME    (CODE)
                            353 	.area GSINIT0 (CODE)
                            354 	.area GSINIT1 (CODE)
                            355 	.area GSINIT2 (CODE)
                            356 	.area GSINIT3 (CODE)
                            357 	.area GSINIT4 (CODE)
                            358 	.area GSINIT5 (CODE)
                            359 	.area GSINIT  (CODE)
                            360 	.area GSFINAL (CODE)
                            361 	.area CSEG    (CODE)
                            362 ;--------------------------------------------------------
                            363 ; global & static initialisations
                            364 ;--------------------------------------------------------
                            365 	.area HOME    (CODE)
                            366 	.area GSINIT  (CODE)
                            367 	.area GSFINAL (CODE)
                            368 	.area GSINIT  (CODE)
                            369 ;--------------------------------------------------------
                            370 ; Home
                            371 ;--------------------------------------------------------
                            372 	.area HOME    (CODE)
                            373 	.area HOME    (CODE)
                            374 ;--------------------------------------------------------
                            375 ; code
                            376 ;--------------------------------------------------------
                            377 	.area CSEG    (CODE)
                            378 ;------------------------------------------------------------
                            379 ;Allocation info for local variables in function 'watchdog_init'
                            380 ;------------------------------------------------------------
                            381 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:34: void watchdog_init(void)
                            382 ;	-----------------------------------------
                            383 ;	 function watchdog_init
                            384 ;	-----------------------------------------
   15C4                     385 _watchdog_init:
                    0007    386 	ar7 = 0x07
                    0006    387 	ar6 = 0x06
                    0005    388 	ar5 = 0x05
                    0004    389 	ar4 = 0x04
                    0003    390 	ar3 = 0x03
                    0002    391 	ar2 = 0x02
                    0001    392 	ar1 = 0x01
                    0000    393 	ar0 = 0x00
                            394 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:41: WDL = 0xFF;
   15C4 75 C1 FF            395 	mov	_WDL,#0xFF
                            396 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:43: EA = 0;
   15C7 C2 AF               397 	clr	_IEN0_7
                            398 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:44: WDCON = 0xE5;
   15C9 75 A7 E5            399 	mov	_WDCON,#0xE5
                            400 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:45: WFEED1 = 0xA5;
   15CC 75 C2 A5            401 	mov	_WFEED1,#0xA5
                            402 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:46: WFEED2 = 0x5A;
   15CF 75 C3 5A            403 	mov	_WFEED2,#0x5A
                            404 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:48: EA=1;
   15D2 D2 AF               405 	setb	_IEN0_7
   15D4 22                  406 	ret
                            407 ;------------------------------------------------------------
                            408 ;Allocation info for local variables in function 'watchdog_feed'
                            409 ;------------------------------------------------------------
                            410 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:56: void watchdog_feed(void)
                            411 ;	-----------------------------------------
                            412 ;	 function watchdog_feed
                            413 ;	-----------------------------------------
   15D5                     414 _watchdog_feed:
                            415 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:62: EA = 0;
   15D5 C2 AF               416 	clr	_IEN0_7
                            417 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:64: WFEED1 = 0xA5;
   15D7 75 C2 A5            418 	mov	_WFEED1,#0xA5
                            419 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:65: WFEED2 = 0x5A;
   15DA 75 C3 5A            420 	mov	_WFEED2,#0x5A
                            421 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:68: EA=1;
   15DD D2 AF               422 	setb	_IEN0_7
   15DF 22                  423 	ret
                            424 ;------------------------------------------------------------
                            425 ;Allocation info for local variables in function 'watchdog_start'
                            426 ;------------------------------------------------------------
                            427 ;eacopy                    Allocated to registers b0 
                            428 ;------------------------------------------------------------
                            429 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:76: void watchdog_start(void)
                            430 ;	-----------------------------------------
                            431 ;	 function watchdog_start
                            432 ;	-----------------------------------------
   15E0                     433 _watchdog_start:
                            434 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:81: eacopy = EA;
   15E0 A2 AF               435 	mov	c,_IEN0_7
   15E2 92 18               436 	mov	b0,c
                            437 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:82: EA = 0;
   15E4 C2 AF               438 	clr	_IEN0_7
                            439 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:84: WDCON |= 0x04;
   15E6 43 A7 04            440 	orl	_WDCON,#0x04
                            441 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:86: WFEED1 = 0xA5;
   15E9 75 C2 A5            442 	mov	_WFEED1,#0xA5
                            443 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:87: WFEED2 = 0x5A;
   15EC 75 C3 5A            444 	mov	_WFEED2,#0x5A
                            445 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:89: EA = eacopy;
   15EF A2 18               446 	mov	c,b0
   15F1 92 AF               447 	mov	_IEN0_7,c
   15F3 22                  448 	ret
                            449 ;------------------------------------------------------------
                            450 ;Allocation info for local variables in function 'watchdog_stop'
                            451 ;------------------------------------------------------------
                            452 ;eacopy                    Allocated to registers b0 
                            453 ;------------------------------------------------------------
                            454 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:97: void watchdog_stop(void)
                            455 ;	-----------------------------------------
                            456 ;	 function watchdog_stop
                            457 ;	-----------------------------------------
   15F4                     458 _watchdog_stop:
                            459 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:102: eacopy = EA;
   15F4 A2 AF               460 	mov	c,_IEN0_7
   15F6 92 18               461 	mov	b0,c
                            462 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:103: EA = 0;
   15F8 C2 AF               463 	clr	_IEN0_7
                            464 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:105: WDCON &= ~0x04;
   15FA AF A7               465 	mov	r7,_WDCON
   15FC 53 07 FB            466 	anl	ar7,#0xFB
   15FF 8F A7               467 	mov	_WDCON,r7
                            468 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:107: WFEED1 = 0xA5;
   1601 75 C2 A5            469 	mov	_WFEED1,#0xA5
                            470 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:108: WFEED2 = 0x5A;
   1604 75 C3 5A            471 	mov	_WFEED2,#0x5A
                            472 ;	C:/Freebus/C_Programme/oldisprogramm/com/watchdog.c:110: EA = eacopy;
   1607 A2 18               473 	mov	c,b0
   1609 92 AF               474 	mov	_IEN0_7,c
   160B 22                  475 	ret
                            476 	.area CSEG    (CODE)
                            477 	.area CONST   (CODE)
                            478 	.area XINIT   (CODE)
                            479 	.area CABS    (ABS,CODE)
