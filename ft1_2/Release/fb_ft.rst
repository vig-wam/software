                              1 ;--------------------------------------------------------
                              2 ; File Created by SDCC : free open source ANSI-C Compiler
                              3 ; Version 3.1.4 #7479 (Mar 23 2012) (MINGW32)
                              4 ; This file was generated Fri Oct 26 20:36:30 2012
                              5 ;--------------------------------------------------------
                              6 	.module fb_ft
                              7 	.optsdcc -mmcs51 --model-small
                              8 	
                              9 ;--------------------------------------------------------
                             10 ; Public variables in this module
                             11 ;--------------------------------------------------------
                             12 	.globl _main
                             13 	.globl _watchdog_start
                             14 	.globl _watchdog_feed
                             15 	.globl _watchdog_init
                             16 	.globl _restart_app
                             17 	.globl _ft_process_telegram
                             18 	.globl _ft_process_fix_frame
                             19 	.globl _ft_process_var_frame
                             20 	.globl _restart_hw
                             21 	.globl _P3_1
                             22 	.globl _P3_0
                             23 	.globl _P1_7
                             24 	.globl _P1_6
                             25 	.globl _P1_5
                             26 	.globl _P1_4
                             27 	.globl _P1_3
                             28 	.globl _P1_2
                             29 	.globl _P1_1
                             30 	.globl _P1_0
                             31 	.globl _P0_7
                             32 	.globl _P0_6
                             33 	.globl _P0_5
                             34 	.globl _P0_4
                             35 	.globl _P0_3
                             36 	.globl _P0_2
                             37 	.globl _P0_1
                             38 	.globl _P0_0
                             39 	.globl _I2CON_0
                             40 	.globl _I2CON_2
                             41 	.globl _I2CON_3
                             42 	.globl _I2CON_4
                             43 	.globl _I2CON_5
                             44 	.globl _I2CON_6
                             45 	.globl _SCON_7
                             46 	.globl _SCON_6
                             47 	.globl _SCON_5
                             48 	.globl _SCON_4
                             49 	.globl _SCON_3
                             50 	.globl _SCON_2
                             51 	.globl _SCON_1
                             52 	.globl _SCON_0
                             53 	.globl _IP0_0
                             54 	.globl _IP0_1
                             55 	.globl _IP0_2
                             56 	.globl _IP0_3
                             57 	.globl _IP0_4
                             58 	.globl _IP0_5
                             59 	.globl _IP0_6
                             60 	.globl _IP1_0
                             61 	.globl _IP1_1
                             62 	.globl _IP1_2
                             63 	.globl _IP1_6
                             64 	.globl _IEN1_0
                             65 	.globl _IEN1_1
                             66 	.globl _IEN1_2
                             67 	.globl _IEN0_0
                             68 	.globl _IEN0_1
                             69 	.globl _IEN0_2
                             70 	.globl _IEN0_3
                             71 	.globl _IEN0_4
                             72 	.globl _IEN0_5
                             73 	.globl _IEN0_6
                             74 	.globl _IEN0_7
                             75 	.globl _TCON_0
                             76 	.globl _TCON_1
                             77 	.globl _TCON_2
                             78 	.globl _TCON_3
                             79 	.globl _TCON_4
                             80 	.globl _TCON_5
                             81 	.globl _TCON_6
                             82 	.globl _TCON_7
                             83 	.globl _PSW_7
                             84 	.globl _PSW_6
                             85 	.globl _PSW_5
                             86 	.globl _PSW_4
                             87 	.globl _PSW_3
                             88 	.globl _PSW_2
                             89 	.globl _PSW_1
                             90 	.globl _PSW_0
                             91 	.globl _IEN1
                             92 	.globl _IP0H
                             93 	.globl _WFEED2
                             94 	.globl _WFEED1
                             95 	.globl _WDL
                             96 	.globl _WDCON
                             97 	.globl _TRIM
                             98 	.globl _TAMOD
                             99 	.globl _SSTAT
                            100 	.globl _RTCL
                            101 	.globl _RTCH
                            102 	.globl _RTCCON
                            103 	.globl _RSTSRC
                            104 	.globl _PT0AD
                            105 	.globl _PCONA
                            106 	.globl _P3M2
                            107 	.globl _P3M1
                            108 	.globl _P1M2
                            109 	.globl _P1M1
                            110 	.globl _P0M2
                            111 	.globl _P0M1
                            112 	.globl _KBPATN
                            113 	.globl _KBMASK
                            114 	.globl _KBCON
                            115 	.globl _IP1H
                            116 	.globl _IP1
                            117 	.globl _I2STAT
                            118 	.globl _I2SCLL
                            119 	.globl _I2SCLH
                            120 	.globl _I2DAT
                            121 	.globl _I2CON
                            122 	.globl _I2ADR
                            123 	.globl _FMDATA
                            124 	.globl _FMCON
                            125 	.globl _FMADRL
                            126 	.globl _FMADRH
                            127 	.globl _DIVM
                            128 	.globl _CMP2
                            129 	.globl _CMP1
                            130 	.globl _BRGCON
                            131 	.globl _BRGR1
                            132 	.globl _BRGR0
                            133 	.globl _SADEN
                            134 	.globl _SADDR
                            135 	.globl _AUXR1
                            136 	.globl _SBUF
                            137 	.globl _SCON
                            138 	.globl _IP0
                            139 	.globl _IEN0
                            140 	.globl _TH1
                            141 	.globl _TH0
                            142 	.globl _TL1
                            143 	.globl _TL0
                            144 	.globl _TMOD
                            145 	.globl _TCON
                            146 	.globl _PCON
                            147 	.globl _DPH
                            148 	.globl _DPL
                            149 	.globl _SP
                            150 	.globl _B
                            151 	.globl _ACC
                            152 	.globl _PSW
                            153 	.globl _P3
                            154 	.globl _P1
                            155 	.globl _P0
                            156 ;--------------------------------------------------------
                            157 ; special function registers
                            158 ;--------------------------------------------------------
                            159 	.area RSEG    (ABS,DATA)
   0000                     160 	.org 0x0000
                    0080    161 _P0	=	0x0080
                    0090    162 _P1	=	0x0090
                    00B0    163 _P3	=	0x00b0
                    00D0    164 _PSW	=	0x00d0
                    00E0    165 _ACC	=	0x00e0
                    00F0    166 _B	=	0x00f0
                    0081    167 _SP	=	0x0081
                    0082    168 _DPL	=	0x0082
                    0083    169 _DPH	=	0x0083
                    0087    170 _PCON	=	0x0087
                    0088    171 _TCON	=	0x0088
                    0089    172 _TMOD	=	0x0089
                    008A    173 _TL0	=	0x008a
                    008B    174 _TL1	=	0x008b
                    008C    175 _TH0	=	0x008c
                    008D    176 _TH1	=	0x008d
                    00A8    177 _IEN0	=	0x00a8
                    00B8    178 _IP0	=	0x00b8
                    0098    179 _SCON	=	0x0098
                    0099    180 _SBUF	=	0x0099
                    00A2    181 _AUXR1	=	0x00a2
                    00A9    182 _SADDR	=	0x00a9
                    00B9    183 _SADEN	=	0x00b9
                    00BE    184 _BRGR0	=	0x00be
                    00BF    185 _BRGR1	=	0x00bf
                    00BD    186 _BRGCON	=	0x00bd
                    00AC    187 _CMP1	=	0x00ac
                    00AD    188 _CMP2	=	0x00ad
                    0095    189 _DIVM	=	0x0095
                    00E7    190 _FMADRH	=	0x00e7
                    00E6    191 _FMADRL	=	0x00e6
                    00E4    192 _FMCON	=	0x00e4
                    00E5    193 _FMDATA	=	0x00e5
                    00DB    194 _I2ADR	=	0x00db
                    00D8    195 _I2CON	=	0x00d8
                    00DA    196 _I2DAT	=	0x00da
                    00DD    197 _I2SCLH	=	0x00dd
                    00DC    198 _I2SCLL	=	0x00dc
                    00D9    199 _I2STAT	=	0x00d9
                    00F8    200 _IP1	=	0x00f8
                    00F7    201 _IP1H	=	0x00f7
                    0094    202 _KBCON	=	0x0094
                    0086    203 _KBMASK	=	0x0086
                    0093    204 _KBPATN	=	0x0093
                    0084    205 _P0M1	=	0x0084
                    0085    206 _P0M2	=	0x0085
                    0091    207 _P1M1	=	0x0091
                    0092    208 _P1M2	=	0x0092
                    00B1    209 _P3M1	=	0x00b1
                    00B2    210 _P3M2	=	0x00b2
                    00B5    211 _PCONA	=	0x00b5
                    00F6    212 _PT0AD	=	0x00f6
                    00DF    213 _RSTSRC	=	0x00df
                    00D1    214 _RTCCON	=	0x00d1
                    00D2    215 _RTCH	=	0x00d2
                    00D3    216 _RTCL	=	0x00d3
                    00BA    217 _SSTAT	=	0x00ba
                    008F    218 _TAMOD	=	0x008f
                    0096    219 _TRIM	=	0x0096
                    00A7    220 _WDCON	=	0x00a7
                    00C1    221 _WDL	=	0x00c1
                    00C2    222 _WFEED1	=	0x00c2
                    00C3    223 _WFEED2	=	0x00c3
                    00B7    224 _IP0H	=	0x00b7
                    00E8    225 _IEN1	=	0x00e8
                            226 ;--------------------------------------------------------
                            227 ; special function bits
                            228 ;--------------------------------------------------------
                            229 	.area RSEG    (ABS,DATA)
   0000                     230 	.org 0x0000
                    00D0    231 _PSW_0	=	0x00d0
                    00D1    232 _PSW_1	=	0x00d1
                    00D2    233 _PSW_2	=	0x00d2
                    00D3    234 _PSW_3	=	0x00d3
                    00D4    235 _PSW_4	=	0x00d4
                    00D5    236 _PSW_5	=	0x00d5
                    00D6    237 _PSW_6	=	0x00d6
                    00D7    238 _PSW_7	=	0x00d7
                    008F    239 _TCON_7	=	0x008f
                    008E    240 _TCON_6	=	0x008e
                    008D    241 _TCON_5	=	0x008d
                    008C    242 _TCON_4	=	0x008c
                    008B    243 _TCON_3	=	0x008b
                    008A    244 _TCON_2	=	0x008a
                    0089    245 _TCON_1	=	0x0089
                    0088    246 _TCON_0	=	0x0088
                    00AF    247 _IEN0_7	=	0x00af
                    00AE    248 _IEN0_6	=	0x00ae
                    00AD    249 _IEN0_5	=	0x00ad
                    00AC    250 _IEN0_4	=	0x00ac
                    00AB    251 _IEN0_3	=	0x00ab
                    00AA    252 _IEN0_2	=	0x00aa
                    00A9    253 _IEN0_1	=	0x00a9
                    00A8    254 _IEN0_0	=	0x00a8
                    00EA    255 _IEN1_2	=	0x00ea
                    00E9    256 _IEN1_1	=	0x00e9
                    00E8    257 _IEN1_0	=	0x00e8
                    00FE    258 _IP1_6	=	0x00fe
                    00FA    259 _IP1_2	=	0x00fa
                    00F9    260 _IP1_1	=	0x00f9
                    00F8    261 _IP1_0	=	0x00f8
                    00BE    262 _IP0_6	=	0x00be
                    00BD    263 _IP0_5	=	0x00bd
                    00BC    264 _IP0_4	=	0x00bc
                    00BB    265 _IP0_3	=	0x00bb
                    00BA    266 _IP0_2	=	0x00ba
                    00B9    267 _IP0_1	=	0x00b9
                    00B8    268 _IP0_0	=	0x00b8
                    0098    269 _SCON_0	=	0x0098
                    0099    270 _SCON_1	=	0x0099
                    009A    271 _SCON_2	=	0x009a
                    009B    272 _SCON_3	=	0x009b
                    009C    273 _SCON_4	=	0x009c
                    009D    274 _SCON_5	=	0x009d
                    009E    275 _SCON_6	=	0x009e
                    009F    276 _SCON_7	=	0x009f
                    00DE    277 _I2CON_6	=	0x00de
                    00DD    278 _I2CON_5	=	0x00dd
                    00DC    279 _I2CON_4	=	0x00dc
                    00DB    280 _I2CON_3	=	0x00db
                    00DA    281 _I2CON_2	=	0x00da
                    00D8    282 _I2CON_0	=	0x00d8
                    0080    283 _P0_0	=	0x0080
                    0081    284 _P0_1	=	0x0081
                    0082    285 _P0_2	=	0x0082
                    0083    286 _P0_3	=	0x0083
                    0084    287 _P0_4	=	0x0084
                    0085    288 _P0_5	=	0x0085
                    0086    289 _P0_6	=	0x0086
                    0087    290 _P0_7	=	0x0087
                    0090    291 _P1_0	=	0x0090
                    0091    292 _P1_1	=	0x0091
                    0092    293 _P1_2	=	0x0092
                    0093    294 _P1_3	=	0x0093
                    0094    295 _P1_4	=	0x0094
                    0095    296 _P1_5	=	0x0095
                    0096    297 _P1_6	=	0x0096
                    0097    298 _P1_7	=	0x0097
                    00B0    299 _P3_0	=	0x00b0
                    00B1    300 _P3_1	=	0x00b1
                            301 ;--------------------------------------------------------
                            302 ; overlayable register banks
                            303 ;--------------------------------------------------------
                            304 	.area REG_BANK_0	(REL,OVR,DATA)
   0000                     305 	.ds 8
                            306 ;--------------------------------------------------------
                            307 ; internal ram data
                            308 ;--------------------------------------------------------
                            309 	.area DSEG    (DATA)
                            310 ;--------------------------------------------------------
                            311 ; overlayable items in internal ram 
                            312 ;--------------------------------------------------------
                            313 ;--------------------------------------------------------
                            314 ; Stack segment in internal ram 
                            315 ;--------------------------------------------------------
                            316 	.area	SSEG	(DATA)
   0077                     317 __start__stack:
   0077                     318 	.ds	1
                            319 
                            320 ;--------------------------------------------------------
                            321 ; indirectly addressable internal ram data
                            322 ;--------------------------------------------------------
                            323 	.area ISEG    (DATA)
                            324 ;--------------------------------------------------------
                            325 ; absolute internal ram data
                            326 ;--------------------------------------------------------
                            327 	.area IABS    (ABS,DATA)
                            328 	.area IABS    (ABS,DATA)
                            329 ;--------------------------------------------------------
                            330 ; bit data
                            331 ;--------------------------------------------------------
                            332 	.area BSEG    (BIT)
                            333 ;--------------------------------------------------------
                            334 ; paged external ram data
                            335 ;--------------------------------------------------------
                            336 	.area PSEG    (PAG,XDATA)
                            337 ;--------------------------------------------------------
                            338 ; external ram data
                            339 ;--------------------------------------------------------
                            340 	.area XSEG    (XDATA)
                            341 ;--------------------------------------------------------
                            342 ; absolute external ram data
                            343 ;--------------------------------------------------------
                            344 	.area XABS    (ABS,XDATA)
                            345 ;--------------------------------------------------------
                            346 ; external initialized ram data
                            347 ;--------------------------------------------------------
                            348 	.area XISEG   (XDATA)
                            349 	.area HOME    (CODE)
                            350 	.area GSINIT0 (CODE)
                            351 	.area GSINIT1 (CODE)
                            352 	.area GSINIT2 (CODE)
                            353 	.area GSINIT3 (CODE)
                            354 	.area GSINIT4 (CODE)
                            355 	.area GSINIT5 (CODE)
                            356 	.area GSINIT  (CODE)
                            357 	.area GSFINAL (CODE)
                            358 	.area CSEG    (CODE)
                            359 ;--------------------------------------------------------
                            360 ; interrupt vector 
                            361 ;--------------------------------------------------------
                            362 	.area HOME    (CODE)
   0000                     363 __interrupt_vect:
   0000 02 00 2B            364 	ljmp	__sdcc_gsinit_startup
   0003 32                  365 	reti
   0004                     366 	.ds	7
   000B 32                  367 	reti
   000C                     368 	.ds	7
   0013 02 0A 57            369 	ljmp	_X1_int
   0016                     370 	.ds	5
   001B 02 0A 87            371 	ljmp	_T1_int
   001E                     372 	.ds	5
   0023 02 08 92            373 	ljmp	_serial_int
                            374 ;--------------------------------------------------------
                            375 ; global & static initialisations
                            376 ;--------------------------------------------------------
                            377 	.area HOME    (CODE)
                            378 	.area GSINIT  (CODE)
                            379 	.area GSFINAL (CODE)
                            380 	.area GSINIT  (CODE)
                            381 	.globl __sdcc_gsinit_startup
                            382 	.globl __sdcc_program_startup
                            383 	.globl __start__stack
                            384 	.globl __mcs51_genXINIT
                            385 	.globl __mcs51_genXRAMCLEAR
                            386 	.globl __mcs51_genRAMCLEAR
                            387 	.area GSFINAL (CODE)
   0084 02 00 26            388 	ljmp	__sdcc_program_startup
                            389 ;--------------------------------------------------------
                            390 ; Home
                            391 ;--------------------------------------------------------
                            392 	.area HOME    (CODE)
                            393 	.area HOME    (CODE)
   0026                     394 __sdcc_program_startup:
   0026 12 09 C0            395 	lcall	_main
                            396 ;	return from main will lock up
   0029 80 FE               397 	sjmp .
                            398 ;--------------------------------------------------------
                            399 ; code
                            400 ;--------------------------------------------------------
                            401 	.area CSEG    (CODE)
                            402 ;------------------------------------------------------------
                            403 ;Allocation info for local variables in function 'main'
                            404 ;------------------------------------------------------------
                            405 ;n                         Allocated to registers r7 
                            406 ;wduf                      Allocated to registers 
                            407 ;------------------------------------------------------------
                            408 ;	../fb_ft.c:33: void main(void)
                            409 ;	-----------------------------------------
                            410 ;	 function main
                            411 ;	-----------------------------------------
   09C0                     412 _main:
                    0007    413 	ar7 = 0x07
                    0006    414 	ar6 = 0x06
                    0005    415 	ar5 = 0x05
                    0004    416 	ar4 = 0x04
                    0003    417 	ar3 = 0x03
                    0002    418 	ar2 = 0x02
                    0001    419 	ar1 = 0x01
                    0000    420 	ar0 = 0x00
                            421 ;	../fb_ft.c:38: wduf=WDCON&0x02;
   09C0 E5 A7               422 	mov	a,_WDCON
                            423 ;	../fb_ft.c:41: restart_hw();				// Hardware zurücksetzen
   09C2 12 0E B3            424 	lcall	_restart_hw
                            425 ;	../fb_ft.c:42: for (n=0;n<50;n++) {		// Warten bis Bus stabil, nach Busspannungswiederkehr
   09C5 7F 00               426 	mov	r7,#0x00
   09C7                     427 00113$:
   09C7 BF 32 00            428 	cjne	r7,#0x32,00136$
   09CA                     429 00136$:
   09CA 50 1A               430 	jnc	00116$
                            431 ;	../fb_ft.c:43: TR0=0;					// Timer 0 anhalten
   09CC C2 8C               432 	clr	_TCON_4
                            433 ;	../fb_ft.c:44: TH0=eeprom[ADDRTAB+1];	// Timer 0 setzen mit phys. Adr. damit Geräte unterschiedlich beginnen zu senden
   09CE 90 1D 17            434 	mov	dptr,#(_eeprom + 0x0017)
   09D1 E4                  435 	clr	a
   09D2 93                  436 	movc	a,@a+dptr
   09D3 F5 8C               437 	mov	_TH0,a
                            438 ;	../fb_ft.c:45: TL0=eeprom[ADDRTAB+2];
   09D5 90 1D 18            439 	mov	dptr,#(_eeprom + 0x0018)
   09D8 E4                  440 	clr	a
   09D9 93                  441 	movc	a,@a+dptr
   09DA F5 8A               442 	mov	_TL0,a
                            443 ;	../fb_ft.c:46: TF0=0;					// Überlauf-Flag zurücksetzen
   09DC C2 8D               444 	clr	_TCON_5
                            445 ;	../fb_ft.c:47: TR0=1;					// Timer 0 starten
   09DE D2 8C               446 	setb	_TCON_4
                            447 ;	../fb_ft.c:48: while(!TF0);
   09E0                     448 00101$:
   09E0 30 8D FD            449 	jnb	_TCON_5,00101$
                            450 ;	../fb_ft.c:42: for (n=0;n<50;n++) {		// Warten bis Bus stabil, nach Busspannungswiederkehr
   09E3 0F                  451 	inc	r7
   09E4 80 E1               452 	sjmp	00113$
   09E6                     453 00116$:
                            454 ;	../fb_ft.c:50: restart_app();			// Anwendungsspezifische Einstellungen zurücksetzen
   09E6 12 09 90            455 	lcall	_restart_app
                            456 ;	../fb_ft.c:52: watchdog_init();
   09E9 12 0A 0F            457 	lcall	_watchdog_init
                            458 ;	../fb_ft.c:53: watchdog_start();
   09EC 12 0A 2B            459 	lcall	_watchdog_start
                            460 ;	../fb_ft.c:55: do  {
   09EF                     461 00110$:
                            462 ;	../fb_ft.c:56: watchdog_feed();
   09EF 12 0A 20            463 	lcall	_watchdog_feed
                            464 ;	../fb_ft.c:57: n = rsin_stat;
   09F2 AF 46               465 	mov	r7,_rsin_stat
                            466 ;	../fb_ft.c:58: rsin_stat = RSIN_NONE;
   09F4 75 46 00            467 	mov	_rsin_stat,#0x00
                            468 ;	../fb_ft.c:59: if ( n == RSIN_VARFRAME ) ft_process_var_frame();
   09F7 BF 01 07            469 	cjne	r7,#0x01,00105$
   09FA C0 07               470 	push	ar7
   09FC 12 00 87            471 	lcall	_ft_process_var_frame
   09FF D0 07               472 	pop	ar7
   0A01                     473 00105$:
                            474 ;	../fb_ft.c:60: if ( n == RSIN_FIXFRAME ) ft_process_fix_frame();
   0A01 BF 02 03            475 	cjne	r7,#0x02,00107$
   0A04 12 04 E3            476 	lcall	_ft_process_fix_frame
   0A07                     477 00107$:
                            478 ;	../fb_ft.c:61: if (tel_arrived) ft_process_telegram();
   0A07 30 09 E5            479 	jnb	_tel_arrived,00110$
   0A0A 12 06 16            480 	lcall	_ft_process_telegram
                            481 ;	../fb_ft.c:62: } while(1);
   0A0D 80 E0               482 	sjmp	00110$
                            483 	.area CSEG    (CODE)
                            484 	.area CONST   (CODE)
                            485 	.area XINIT   (CODE)
                            486 	.area CABS    (ABS,CODE)
