***************************
HelloWorld 的objdump结果
***************************

.. code-block::

    HelloWorld：     文件格式 elf64-x86-64
    HelloWorld
    体系结构：i386:x86-64，标志 0x00000150：
    HAS_SYMS, DYNAMIC, D_PAGED
    起始地址 0x0000000000001080

    程序头：
        PHDR off    0x0000000000000040 vaddr 0x0000000000000040 paddr 0x0000000000000040 align 2**3
            filesz 0x0000000000000268 memsz 0x0000000000000268 flags r--
    INTERP off    0x00000000000002a8 vaddr 0x00000000000002a8 paddr 0x00000000000002a8 align 2**0
            filesz 0x000000000000001c memsz 0x000000000000001c flags r--
        LOAD off    0x0000000000000000 vaddr 0x0000000000000000 paddr 0x0000000000000000 align 2**12
            filesz 0x00000000000007c0 memsz 0x00000000000007c0 flags r--
        LOAD off    0x0000000000001000 vaddr 0x0000000000001000 paddr 0x0000000000001000 align 2**12
            filesz 0x000000000000026d memsz 0x000000000000026d flags r-x
        LOAD off    0x0000000000002000 vaddr 0x0000000000002000 paddr 0x0000000000002000 align 2**12
            filesz 0x00000000000001a8 memsz 0x00000000000001a8 flags r--
        LOAD off    0x0000000000002da0 vaddr 0x0000000000003da0 paddr 0x0000000000003da0 align 2**12
            filesz 0x00000000000002a8 memsz 0x00000000000003d8 flags rw-
    DYNAMIC off    0x0000000000002db8 vaddr 0x0000000000003db8 paddr 0x0000000000003db8 align 2**3
            filesz 0x0000000000000210 memsz 0x0000000000000210 flags rw-
        NOTE off    0x00000000000002c4 vaddr 0x00000000000002c4 paddr 0x00000000000002c4 align 2**2
            filesz 0x0000000000000044 memsz 0x0000000000000044 flags r--
    EH_FRAME off    0x0000000000002014 vaddr 0x0000000000002014 paddr 0x0000000000002014 align 2**2
            filesz 0x000000000000004c memsz 0x000000000000004c flags r--
    STACK off    0x0000000000000000 vaddr 0x0000000000000000 paddr 0x0000000000000000 align 2**4
            filesz 0x0000000000000000 memsz 0x0000000000000000 flags rw-
    RELRO off    0x0000000000002da0 vaddr 0x0000000000003da0 paddr 0x0000000000003da0 align 2**0
            filesz 0x0000000000000260 memsz 0x0000000000000260 flags r--

    动态节：
    NEEDED               libstdc++.so.6
    NEEDED               libm.so.6
    NEEDED               libgcc_s.so.1
    NEEDED               libc.so.6
    INIT                 0x0000000000001000
    FINI                 0x0000000000001264
    INIT_ARRAY           0x0000000000003da0
    INIT_ARRAYSZ         0x0000000000000010
    FINI_ARRAY           0x0000000000003db0
    FINI_ARRAYSZ         0x0000000000000008
    GNU_HASH             0x0000000000000308
    STRTAB               0x0000000000000468
    SYMTAB               0x0000000000000330
    STRSZ                0x000000000000017b
    SYMENT               0x0000000000000018
    DEBUG                0x0000000000000000
    PLTGOT               0x0000000000004000
    PLTRELSZ             0x0000000000000060
    PLTREL               0x0000000000000007
    JMPREL               0x0000000000000760
    RELA                 0x0000000000000640
    RELASZ               0x0000000000000120
    RELAENT              0x0000000000000018
    FLAGS_1              0x0000000008000000
    VERNEED              0x0000000000000600
    VERNEEDNUM           0x0000000000000002
    VERSYM               0x00000000000005e4
    RELACOUNT            0x0000000000000004

    版本引用：
    required from libstdc++.so.6:
        0x08922974 0x00 03 GLIBCXX_3.4
    required from libc.so.6:
        0x09691a75 0x00 02 GLIBC_2.2.5

    节：
    Idx Name          Size      VMA               LMA               File off  Algn
    0 .interp       0000001c  00000000000002a8  00000000000002a8  000002a8  2**0
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    1 .note.ABI-tag 00000020  00000000000002c4  00000000000002c4  000002c4  2**2
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    2 .note.gnu.build-id 00000024  00000000000002e4  00000000000002e4  000002e4  2**2
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    3 .gnu.hash     00000028  0000000000000308  0000000000000308  00000308  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    4 .dynsym       00000138  0000000000000330  0000000000000330  00000330  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    5 .dynstr       0000017b  0000000000000468  0000000000000468  00000468  2**0
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    6 .gnu.version  0000001a  00000000000005e4  00000000000005e4  000005e4  2**1
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    7 .gnu.version_r 00000040  0000000000000600  0000000000000600  00000600  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    8 .rela.dyn     00000120  0000000000000640  0000000000000640  00000640  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    9 .rela.plt     00000060  0000000000000760  0000000000000760  00000760  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    10 .init         00000017  0000000000001000  0000000000001000  00001000  2**2
                    CONTENTS, ALLOC, LOAD, READONLY, CODE
    11 .plt          00000050  0000000000001020  0000000000001020  00001020  2**4
                    CONTENTS, ALLOC, LOAD, READONLY, CODE
    12 .plt.got      00000008  0000000000001070  0000000000001070  00001070  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, CODE
    13 .text         000001e1  0000000000001080  0000000000001080  00001080  2**4
                    CONTENTS, ALLOC, LOAD, READONLY, CODE
    14 .fini         00000009  0000000000001264  0000000000001264  00001264  2**2
                    CONTENTS, ALLOC, LOAD, READONLY, CODE
    15 .rodata       00000011  0000000000002000  0000000000002000  00002000  2**2
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    16 .eh_frame_hdr 0000004c  0000000000002014  0000000000002014  00002014  2**2
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    17 .eh_frame     00000148  0000000000002060  0000000000002060  00002060  2**3
                    CONTENTS, ALLOC, LOAD, READONLY, DATA
    18 .init_array   00000010  0000000000003da0  0000000000003da0  00002da0  2**3
                    CONTENTS, ALLOC, LOAD, DATA
    19 .fini_array   00000008  0000000000003db0  0000000000003db0  00002db0  2**3
                    CONTENTS, ALLOC, LOAD, DATA
    20 .dynamic      00000210  0000000000003db8  0000000000003db8  00002db8  2**3
                    CONTENTS, ALLOC, LOAD, DATA
    21 .got          00000038  0000000000003fc8  0000000000003fc8  00002fc8  2**3
                    CONTENTS, ALLOC, LOAD, DATA
    22 .got.plt      00000038  0000000000004000  0000000000004000  00003000  2**3
                    CONTENTS, ALLOC, LOAD, DATA
    23 .data         00000010  0000000000004038  0000000000004038  00003038  2**3
                    CONTENTS, ALLOC, LOAD, DATA
    24 .bss          00000118  0000000000004060  0000000000004060  00003048  2**5
                    ALLOC
    25 .comment      0000001c  0000000000000000  0000000000000000  00003048  2**0
                    CONTENTS, READONLY
    SYMBOL TABLE:
    00000000000002a8 l    d  .interp	0000000000000000              .interp
    00000000000002c4 l    d  .note.ABI-tag	0000000000000000              .note.ABI-tag
    00000000000002e4 l    d  .note.gnu.build-id	0000000000000000              .note.gnu.build-id
    0000000000000308 l    d  .gnu.hash	0000000000000000              .gnu.hash
    0000000000000330 l    d  .dynsym	0000000000000000              .dynsym
    0000000000000468 l    d  .dynstr	0000000000000000              .dynstr
    00000000000005e4 l    d  .gnu.version	0000000000000000              .gnu.version
    0000000000000600 l    d  .gnu.version_r	0000000000000000              .gnu.version_r
    0000000000000640 l    d  .rela.dyn	0000000000000000              .rela.dyn
    0000000000000760 l    d  .rela.plt	0000000000000000              .rela.plt
    0000000000001000 l    d  .init	0000000000000000              .init
    0000000000001020 l    d  .plt	0000000000000000              .plt
    0000000000001070 l    d  .plt.got	0000000000000000              .plt.got
    0000000000001080 l    d  .text	0000000000000000              .text
    0000000000001264 l    d  .fini	0000000000000000              .fini
    0000000000002000 l    d  .rodata	0000000000000000              .rodata
    0000000000002014 l    d  .eh_frame_hdr	0000000000000000              .eh_frame_hdr
    0000000000002060 l    d  .eh_frame	0000000000000000              .eh_frame
    0000000000003da0 l    d  .init_array	0000000000000000              .init_array
    0000000000003db0 l    d  .fini_array	0000000000000000              .fini_array
    0000000000003db8 l    d  .dynamic	0000000000000000              .dynamic
    0000000000003fc8 l    d  .got	0000000000000000              .got
    0000000000004000 l    d  .got.plt	0000000000000000              .got.plt
    0000000000004038 l    d  .data	0000000000000000              .data
    0000000000004060 l    d  .bss	0000000000000000              .bss
    0000000000000000 l    d  .comment	0000000000000000              .comment
    0000000000000000 l    df *ABS*	0000000000000000              crtstuff.c
    00000000000010b0 l     F .text	0000000000000000              deregister_tm_clones
    00000000000010e0 l     F .text	0000000000000000              register_tm_clones
    0000000000001120 l     F .text	0000000000000000              __do_global_dtors_aux
    0000000000004170 l     O .bss	0000000000000001              completed.7325
    0000000000003db0 l     O .fini_array	0000000000000000              __do_global_dtors_aux_fini_array_entry
    0000000000001160 l     F .text	0000000000000000              frame_dummy
    0000000000003da0 l     O .init_array	0000000000000000              __frame_dummy_init_array_entry
    0000000000000000 l    df *ABS*	0000000000000000              HelloWorld.cpp
    0000000000002004 l     O .rodata	0000000000000001              _ZStL19piecewise_construct
    0000000000004171 l     O .bss	0000000000000001              _ZStL8__ioinit
    0000000000001198 l     F .text	0000000000000049              _Z41__static_initialization_and_destruction_0ii
    00000000000011e1 l     F .text	0000000000000015              _GLOBAL__sub_I_main
    0000000000000000 l    df *ABS*	0000000000000000              crtstuff.c
    00000000000021a4 l     O .eh_frame	0000000000000000              __FRAME_END__
    0000000000000000 l    df *ABS*	0000000000000000              
    0000000000002014 l       .eh_frame_hdr	0000000000000000              __GNU_EH_FRAME_HDR
    0000000000001000 l     F .init	0000000000000000              _init
    0000000000003db8 l     O .dynamic	0000000000000000              _DYNAMIC
    0000000000003db0 l       .init_array	0000000000000000              __init_array_end
    0000000000003da0 l       .init_array	0000000000000000              __init_array_start
    0000000000004000 l     O .got.plt	0000000000000000              _GLOBAL_OFFSET_TABLE_
    0000000000004048 g       .data	0000000000000000              _edata
    0000000000004038  w      .data	0000000000000000              data_start
    0000000000002000 g     O .rodata	0000000000000004              _IO_stdin_used
    0000000000000000  w    F *UND*	0000000000000000              __cxa_finalize@@GLIBC_2.2.5
    0000000000001165 g     F .text	0000000000000033              main
    0000000000000000       F *UND*	0000000000000000              _ZSt4endlIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_@@GLIBCXX_3.4
    0000000000004040 g     O .data	0000000000000000              .hidden __dso_handle
    0000000000001264 g     F .fini	0000000000000000              .hidden _fini
    0000000000000000       F *UND*	0000000000000000              __cxa_atexit@@GLIBC_2.2.5
    0000000000001080 g     F .text	000000000000002b              _start
    0000000000000000       F *UND*	0000000000000000              _ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@@GLIBCXX_3.4
    0000000000000000       F *UND*	0000000000000000              _ZNSolsEPFRSoS_E@@GLIBCXX_3.4
    0000000000004048 g     O .data	0000000000000000              .hidden __TMC_END__
    0000000000004060 g     O .bss	0000000000000110              _ZSt4cout@@GLIBCXX_3.4
    0000000000004038 g       .data	0000000000000000              __data_start
    0000000000004178 g       .bss	0000000000000000              _end
    0000000000004048 g       .bss	0000000000000000              __bss_start
    0000000000000000       F *UND*	0000000000000000              _ZNSt8ios_base4InitC1Ev@@GLIBCXX_3.4
    0000000000001200 g     F .text	000000000000005d              __libc_csu_init
    0000000000000000  w      *UND*	0000000000000000              _ITM_deregisterTMCloneTable
    0000000000001260 g     F .text	0000000000000001              __libc_csu_fini
    0000000000000000       F *UND*	0000000000000000              __libc_start_main@@GLIBC_2.2.5
    0000000000000000  w      *UND*	0000000000000000              __gmon_start__
    0000000000000000  w      *UND*	0000000000000000              _ITM_registerTMCloneTable
    0000000000000000       F *UND*	0000000000000000              _ZNSt8ios_base4InitD1Ev@@GLIBCXX_3.4


    Contents of section .interp:
    02a8 2f6c6962 36342f6c 642d6c69 6e75782d  /lib64/ld-linux-
    02b8 7838362d 36342e73 6f2e3200           x86-64.so.2.    
    Contents of section .note.ABI-tag:
    02c4 04000000 10000000 01000000 474e5500  ............GNU.
    02d4 00000000 03000000 02000000 00000000  ................
    Contents of section .note.gnu.build-id:
    02e4 04000000 14000000 03000000 474e5500  ............GNU.
    02f4 9f16c871 65c6f272 78c4123f a00647a7  ...qe..rx..?..G.
    0304 8c40c1ce                             .@..            
    Contents of section .gnu.hash:
    0308 02000000 0b000000 01000000 06000000  ................
    0318 00009100 01000000 0b000000 00000000  ................
    0328 d065ce6d 15980c43                    .e.m...C        
    Contents of section .dynsym:
    0330 00000000 00000000 00000000 00000000  ................
    0340 00000000 00000000 7e000000 12000000  ........~.......
    0350 00000000 00000000 00000000 00000000  ................
    0360 35010000 12000000 00000000 00000000  5...............
    0370 00000000 00000000 d1000000 12000000  ................
    0380 00000000 00000000 00000000 00000000  ................
    0390 6d000000 12000000 00000000 00000000  m...............
    03a0 00000000 00000000 b9000000 12000000  ................
    03b0 00000000 00000000 00000000 00000000  ................
    03c0 1f000000 20000000 00000000 00000000  .... ...........
    03d0 00000000 00000000 51010000 12000000  ........Q.......
    03e0 00000000 00000000 00000000 00000000  ................
    03f0 10000000 20000000 00000000 00000000  .... ...........
    0400 00000000 00000000 3b000000 20000000  ........;... ...
    0410 00000000 00000000 00000000 00000000  ................
    0420 55000000 12000000 00000000 00000000  U...............
    0430 00000000 00000000 42010000 22000000  ........B..."...
    0440 00000000 00000000 00000000 00000000  ................
    0450 09010000 11001900 60400000 00000000  ........`@......
    0460 10010000 00000000                    ........        
    Contents of section .dynstr:
    0468 006c6962 73746463 2b2b2e73 6f2e3600  .libstdc++.so.6.
    0478 5f5f676d 6f6e5f73 74617274 5f5f005f  __gmon_start__._
    0488 49544d5f 64657265 67697374 6572544d  ITM_deregisterTM
    0498 436c6f6e 65546162 6c65005f 49544d5f  CloneTable._ITM_
    04a8 72656769 73746572 544d436c 6f6e6554  registerTMCloneT
    04b8 61626c65 005f5a4e 53743869 6f735f62  able._ZNSt8ios_b
    04c8 61736534 496e6974 44314576 005f5a4e  ase4InitD1Ev._ZN
    04d8 536f6c73 45504652 536f535f 45005f5a  SolsEPFRSoS_E._Z
    04e8 53743465 6e646c49 63537431 31636861  St4endlIcSt11cha
    04f8 725f7472 61697473 49634545 52537431  r_traitsIcEERSt1
    0508 33626173 69635f6f 73747265 616d4954  3basic_ostreamIT
    0518 5f54305f 4553365f 005f5a4e 53743869  _T0_ES6_._ZNSt8i
    0528 6f735f62 61736534 496e6974 43314576  os_base4InitC1Ev
    0538 005f5a53 746c7349 53743131 63686172  ._ZStlsISt11char
    0548 5f747261 69747349 63454552 53743133  _traitsIcEERSt13
    0558 62617369 635f6f73 74726561 6d496354  basic_ostreamIcT
    0568 5f455335 5f504b63 005f5a53 7434636f  _ES5_PKc._ZSt4co
    0578 7574006c 69626d2e 736f2e36 006c6962  ut.libm.so.6.lib
    0588 6763635f 732e736f 2e31006c 6962632e  gcc_s.so.1.libc.
    0598 736f2e36 005f5f63 78615f61 74657869  so.6.__cxa_atexi
    05a8 74005f5f 6378615f 66696e61 6c697a65  t.__cxa_finalize
    05b8 005f5f6c 6962635f 73746172 745f6d61  .__libc_start_ma
    05c8 696e0047 4c494243 58585f33 2e340047  in.GLIBCXX_3.4.G
    05d8 4c494243 5f322e32 2e3500             LIBC_2.2.5.     
    Contents of section .gnu.version:
    05e4 00000300 02000300 03000300 00000200  ................
    05f4 00000000 03000200 0300               ..........      
    Contents of section .gnu.version_r:
    0600 01000100 01000000 10000000 20000000  ............ ...
    0610 74299208 00000300 63010000 00000000  t)......c.......
    0620 01000100 2b010000 10000000 00000000  ....+...........
    0630 751a6909 00000200 6f010000 00000000  u.i.....o.......
    Contents of section .rela.dyn:
    0640 a03d0000 00000000 08000000 00000000  .=..............
    0650 60110000 00000000 a83d0000 00000000  `........=......
    0660 08000000 00000000 e1110000 00000000  ................
    0670 b03d0000 00000000 08000000 00000000  .=..............
    0680 20110000 00000000 40400000 00000000   .......@@......
    0690 08000000 00000000 40400000 00000000  ........@@......
    06a0 c83f0000 00000000 06000000 0b000000  .?..............
    06b0 00000000 00000000 d03f0000 00000000  .........?......
    06c0 06000000 01000000 00000000 00000000  ................
    06d0 d83f0000 00000000 06000000 06000000  .?..............
    06e0 00000000 00000000 e03f0000 00000000  .........?......
    06f0 06000000 07000000 00000000 00000000  ................
    0700 e83f0000 00000000 06000000 08000000  .?..............
    0710 00000000 00000000 f03f0000 00000000  .........?......
    0720 06000000 09000000 00000000 00000000  ................
    0730 f83f0000 00000000 06000000 0a000000  .?..............
    0740 00000000 00000000 60400000 00000000  ........`@......
    0750 05000000 0c000000 00000000 00000000  ................
    Contents of section .rela.plt:
    0760 18400000 00000000 07000000 02000000  .@..............
    0770 00000000 00000000 20400000 00000000  ........ @......
    0780 07000000 03000000 00000000 00000000  ................
    0790 28400000 00000000 07000000 04000000  (@..............
    07a0 00000000 00000000 30400000 00000000  ........0@......
    07b0 07000000 05000000 00000000 00000000  ................
    Contents of section .init:
    1000 4883ec08 488b05dd 2f000048 85c07402  H...H.../..H..t.
    1010 ffd04883 c408c3                      ..H....         
    Contents of section .plt:
    1020 ff35e22f 0000ff25 e42f0000 0f1f4000  .5./...%./....@.
    1030 ff25e22f 00006800 000000e9 e0ffffff  .%./..h.........
    1040 ff25da2f 00006801 000000e9 d0ffffff  .%./..h.........
    1050 ff25d22f 00006802 000000e9 c0ffffff  .%./..h.........
    1060 ff25ca2f 00006803 000000e9 b0ffffff  .%./..h.........
    Contents of section .plt.got:
    1070 ff25522f 00006690                    .%R/..f.        
    Contents of section .text:
    1080 31ed4989 d15e4889 e24883e4 f050544c  1.I..^H..H...PTL
    1090 8d05ca01 0000488d 0d630100 00488d3d  ......H..c...H.=
    10a0 c1000000 ff15362f 0000f40f 1f440000  ......6/.....D..
    10b0 488d3d91 2f000048 8d058a2f 00004839  H.=./..H.../..H9
    10c0 f8741548 8b050e2f 00004885 c07409ff  .t.H.../..H..t..
    10d0 e00f1f80 00000000 c30f1f80 00000000  ................
    10e0 488d3d61 2f000048 8d355a2f 00004829  H.=a/..H.5Z/..H)
    10f0 fe48c1fe 034889f0 48c1e83f 4801c648  .H...H..H..?H..H
    1100 d1fe7414 488b05e5 2e000048 85c07408  ..t.H......H..t.
    1110 ffe0660f 1f440000 c30f1f80 00000000  ..f..D..........
    1120 803d4930 00000075 2f554883 3d962e00  .=I0...u/UH.=...
    1130 00004889 e5740c48 8b3d022f 0000e82d  ..H..t.H.=./...-
    1140 ffffffe8 68ffffff c6052130 0000015d  ....h.....!0...]
    1150 c30f1f80 00000000 c30f1f80 00000000  ................
    1160 e97bffff ff554889 e5488d35 950e0000  .{...UH..H.5....
    1170 488d3de9 2e0000e8 c4feffff 4889c248  H.=.........H..H
    1180 8b054a2e 00004889 c64889d7 e8bffeff  ..J...H..H......
    1190 ffb80000 00005dc3 554889e5 4883ec10  ......].UH..H...
    11a0 897dfc89 75f8837d fc017532 817df8ff  .}..u..}..u2.}..
    11b0 ff000075 29488d3d b52f0000 e89ffeff  ...u)H.=./......
    11c0 ff488d15 782e0000 488d35a2 2f000048  .H..x...H.5./..H
    11d0 8b05222e 00004889 c7e852fe ffff90c9  .."...H...R.....
    11e0 c3554889 e5beffff 0000bf01 000000e8  .UH.............
    11f0 a4ffffff 5dc3662e 0f1f8400 00000000  ....].f.........
    1200 41574989 d7415649 89f64155 4189fd41  AWI..AVI..AUA..A
    1210 544c8d25 882b0000 55488d2d 902b0000  TL.%.+..UH.-.+..
    1220 534c29e5 4883ec08 e8d3fdff ff48c1fd  SL).H........H..
    1230 03741b31 db0f1f00 4c89fa4c 89f64489  .t.1....L..L..D.
    1240 ef41ff14 dc4883c3 014839dd 75ea4883  .A...H...H9.u.H.
    1250 c4085b5d 415c415d 415e415f c30f1f00  ..[]A\A]A^A_....
    1260 c3                                   .               
    Contents of section .fini:
    1264 4883ec08 4883c408 c3                 H...H....       
    Contents of section .rodata:
    2000 01000200 0048656c 6c6f2057 6f726c64  .....Hello World
    2010 00                                   .               
    Contents of section .eh_frame_hdr:
    2014 011b033b 48000000 08000000 0cf0ffff  ...;H...........
    2024 94000000 5cf0ffff bc000000 6cf0ffff  ....\.......l...
    2034 64000000 51f1ffff d4000000 84f1ffff  d...Q...........
    2044 f4000000 cdf1ffff 14010000 ecf1ffff  ................
    2054 34010000 4cf2ffff 7c010000           4...L...|...    
    Contents of section .eh_frame:
    2060 14000000 00000000 017a5200 01781001  .........zR..x..
    2070 1b0c0708 90010710 14000000 1c000000  ................
    2080 00f0ffff 2b000000 00000000 00000000  ....+...........
    2090 14000000 00000000 017a5200 01781001  .........zR..x..
    20a0 1b0c0708 90010000 24000000 1c000000  ........$.......
    20b0 70efffff 50000000 000e1046 0e184a0f  p...P......F..J.
    20c0 0b770880 003f1a3b 2a332422 00000000  .w...?.;*3$"....
    20d0 14000000 44000000 98efffff 08000000  ....D...........
    20e0 00000000 00000000 1c000000 5c000000  ............\...
    20f0 75f0ffff 33000000 00410e10 8602430d  u...3....A....C.
    2100 066e0c07 08000000 1c000000 7c000000  .n..........|...
    2110 88f0ffff 49000000 00410e10 8602430d  ....I....A....C.
    2120 0602440c 07080000 1c000000 9c000000  ..D.............
    2130 b1f0ffff 15000000 00410e10 8602430d  .........A....C.
    2140 06500c07 08000000 44000000 bc000000  .P......D.......
    2150 b0f0ffff 5d000000 00420e10 8f02450e  ....]....B....E.
    2160 188e0345 0e208d04 450e288c 05480e30  ...E. ..E.(..H.0
    2170 8606480e 38830747 0e406a0e 38410e30  ..H.8..G.@j.8A.0
    2180 410e2842 0e20420e 18420e10 420e0800  A.(B. B..B..B...
    2190 10000000 04010000 c8f0ffff 01000000  ................
    21a0 00000000 00000000                    ........        
    Contents of section .init_array:
    3da0 60110000 00000000 e1110000 00000000  `...............
    Contents of section .fini_array:
    3db0 20110000 00000000                     .......        
    Contents of section .dynamic:
    3db8 01000000 00000000 01000000 00000000  ................
    3dc8 01000000 00000000 13010000 00000000  ................
    3dd8 01000000 00000000 1d010000 00000000  ................
    3de8 01000000 00000000 2b010000 00000000  ........+.......
    3df8 0c000000 00000000 00100000 00000000  ................
    3e08 0d000000 00000000 64120000 00000000  ........d.......
    3e18 19000000 00000000 a03d0000 00000000  .........=......
    3e28 1b000000 00000000 10000000 00000000  ................
    3e38 1a000000 00000000 b03d0000 00000000  .........=......
    3e48 1c000000 00000000 08000000 00000000  ................
    3e58 f5feff6f 00000000 08030000 00000000  ...o............
    3e68 05000000 00000000 68040000 00000000  ........h.......
    3e78 06000000 00000000 30030000 00000000  ........0.......
    3e88 0a000000 00000000 7b010000 00000000  ........{.......
    3e98 0b000000 00000000 18000000 00000000  ................
    3ea8 15000000 00000000 00000000 00000000  ................
    3eb8 03000000 00000000 00400000 00000000  .........@......
    3ec8 02000000 00000000 60000000 00000000  ........`.......
    3ed8 14000000 00000000 07000000 00000000  ................
    3ee8 17000000 00000000 60070000 00000000  ........`.......
    3ef8 07000000 00000000 40060000 00000000  ........@.......
    3f08 08000000 00000000 20010000 00000000  ........ .......
    3f18 09000000 00000000 18000000 00000000  ................
    3f28 fbffff6f 00000000 00000008 00000000  ...o............
    3f38 feffff6f 00000000 00060000 00000000  ...o............
    3f48 ffffff6f 00000000 02000000 00000000  ...o............
    3f58 f0ffff6f 00000000 e4050000 00000000  ...o............
    3f68 f9ffff6f 00000000 04000000 00000000  ...o............
    3f78 00000000 00000000 00000000 00000000  ................
    3f88 00000000 00000000 00000000 00000000  ................
    3f98 00000000 00000000 00000000 00000000  ................
    3fa8 00000000 00000000 00000000 00000000  ................
    3fb8 00000000 00000000 00000000 00000000  ................
    Contents of section .got:
    3fc8 00000000 00000000 00000000 00000000  ................
    3fd8 00000000 00000000 00000000 00000000  ................
    3fe8 00000000 00000000 00000000 00000000  ................
    3ff8 00000000 00000000                    ........        
    Contents of section .got.plt:
    4000 b83d0000 00000000 00000000 00000000  .=..............
    4010 00000000 00000000 36100000 00000000  ........6.......
    4020 46100000 00000000 56100000 00000000  F.......V.......
    4030 66100000 00000000                    f.......        
    Contents of section .data:
    4038 00000000 00000000 40400000 00000000  ........@@......
    Contents of section .comment:
    0000 4743433a 20284465 6269616e 20382e33  GCC: (Debian 8.3
    0010 2e302d36 2920382e 332e3000           .0-6) 8.3.0.    

    Disassembly of section .init:

    0000000000001000 <_init>:
        1000:	48 83 ec 08          	sub    $0x8,%rsp
        1004:	48 8b 05 dd 2f 00 00 	mov    0x2fdd(%rip),%rax        # 3fe8 <__gmon_start__>
        100b:	48 85 c0             	test   %rax,%rax
        100e:	74 02                	je     1012 <_init+0x12>
        1010:	ff d0                	callq  *%rax
        1012:	48 83 c4 08          	add    $0x8,%rsp
        1016:	c3                   	retq   

    Disassembly of section .plt:

    0000000000001020 <.plt>:
        1020:	ff 35 e2 2f 00 00    	pushq  0x2fe2(%rip)        # 4008 <_GLOBAL_OFFSET_TABLE_+0x8>
        1026:	ff 25 e4 2f 00 00    	jmpq   *0x2fe4(%rip)        # 4010 <_GLOBAL_OFFSET_TABLE_+0x10>
        102c:	0f 1f 40 00          	nopl   0x0(%rax)

    0000000000001030 <__cxa_atexit@plt>:
        1030:	ff 25 e2 2f 00 00    	jmpq   *0x2fe2(%rip)        # 4018 <__cxa_atexit@GLIBC_2.2.5>
        1036:	68 00 00 00 00       	pushq  $0x0
        103b:	e9 e0 ff ff ff       	jmpq   1020 <.plt>

    0000000000001040 <_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@plt>:
        1040:	ff 25 da 2f 00 00    	jmpq   *0x2fda(%rip)        # 4020 <_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@GLIBCXX_3.4>
        1046:	68 01 00 00 00       	pushq  $0x1
        104b:	e9 d0 ff ff ff       	jmpq   1020 <.plt>

    0000000000001050 <_ZNSolsEPFRSoS_E@plt>:
        1050:	ff 25 d2 2f 00 00    	jmpq   *0x2fd2(%rip)        # 4028 <_ZNSolsEPFRSoS_E@GLIBCXX_3.4>
        1056:	68 02 00 00 00       	pushq  $0x2
        105b:	e9 c0 ff ff ff       	jmpq   1020 <.plt>

    0000000000001060 <_ZNSt8ios_base4InitC1Ev@plt>:
        1060:	ff 25 ca 2f 00 00    	jmpq   *0x2fca(%rip)        # 4030 <_ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4>
        1066:	68 03 00 00 00       	pushq  $0x3
        106b:	e9 b0 ff ff ff       	jmpq   1020 <.plt>

    Disassembly of section .plt.got:

    0000000000001070 <__cxa_finalize@plt>:
        1070:	ff 25 52 2f 00 00    	jmpq   *0x2f52(%rip)        # 3fc8 <__cxa_finalize@GLIBC_2.2.5>
        1076:	66 90                	xchg   %ax,%ax

    Disassembly of section .text:

    0000000000001080 <_start>:
        1080:	31 ed                	xor    %ebp,%ebp
        1082:	49 89 d1             	mov    %rdx,%r9
        1085:	5e                   	pop    %rsi
        1086:	48 89 e2             	mov    %rsp,%rdx
        1089:	48 83 e4 f0          	and    $0xfffffffffffffff0,%rsp
        108d:	50                   	push   %rax
        108e:	54                   	push   %rsp
        108f:	4c 8d 05 ca 01 00 00 	lea    0x1ca(%rip),%r8        # 1260 <__libc_csu_fini>
        1096:	48 8d 0d 63 01 00 00 	lea    0x163(%rip),%rcx        # 1200 <__libc_csu_init>
        109d:	48 8d 3d c1 00 00 00 	lea    0xc1(%rip),%rdi        # 1165 <main>
        10a4:	ff 15 36 2f 00 00    	callq  *0x2f36(%rip)        # 3fe0 <__libc_start_main@GLIBC_2.2.5>
        10aa:	f4                   	hlt    
        10ab:	0f 1f 44 00 00       	nopl   0x0(%rax,%rax,1)

    00000000000010b0 <deregister_tm_clones>:
        10b0:	48 8d 3d 91 2f 00 00 	lea    0x2f91(%rip),%rdi        # 4048 <__TMC_END__>
        10b7:	48 8d 05 8a 2f 00 00 	lea    0x2f8a(%rip),%rax        # 4048 <__TMC_END__>
        10be:	48 39 f8             	cmp    %rdi,%rax
        10c1:	74 15                	je     10d8 <deregister_tm_clones+0x28>
        10c3:	48 8b 05 0e 2f 00 00 	mov    0x2f0e(%rip),%rax        # 3fd8 <_ITM_deregisterTMCloneTable>
        10ca:	48 85 c0             	test   %rax,%rax
        10cd:	74 09                	je     10d8 <deregister_tm_clones+0x28>
        10cf:	ff e0                	jmpq   *%rax
        10d1:	0f 1f 80 00 00 00 00 	nopl   0x0(%rax)
        10d8:	c3                   	retq   
        10d9:	0f 1f 80 00 00 00 00 	nopl   0x0(%rax)

    00000000000010e0 <register_tm_clones>:
        10e0:	48 8d 3d 61 2f 00 00 	lea    0x2f61(%rip),%rdi        # 4048 <__TMC_END__>
        10e7:	48 8d 35 5a 2f 00 00 	lea    0x2f5a(%rip),%rsi        # 4048 <__TMC_END__>
        10ee:	48 29 fe             	sub    %rdi,%rsi
        10f1:	48 c1 fe 03          	sar    $0x3,%rsi
        10f5:	48 89 f0             	mov    %rsi,%rax
        10f8:	48 c1 e8 3f          	shr    $0x3f,%rax
        10fc:	48 01 c6             	add    %rax,%rsi
        10ff:	48 d1 fe             	sar    %rsi
        1102:	74 14                	je     1118 <register_tm_clones+0x38>
        1104:	48 8b 05 e5 2e 00 00 	mov    0x2ee5(%rip),%rax        # 3ff0 <_ITM_registerTMCloneTable>
        110b:	48 85 c0             	test   %rax,%rax
        110e:	74 08                	je     1118 <register_tm_clones+0x38>
        1110:	ff e0                	jmpq   *%rax
        1112:	66 0f 1f 44 00 00    	nopw   0x0(%rax,%rax,1)
        1118:	c3                   	retq   
        1119:	0f 1f 80 00 00 00 00 	nopl   0x0(%rax)

    0000000000001120 <__do_global_dtors_aux>:
        1120:	80 3d 49 30 00 00 00 	cmpb   $0x0,0x3049(%rip)        # 4170 <completed.7325>
        1127:	75 2f                	jne    1158 <__do_global_dtors_aux+0x38>
        1129:	55                   	push   %rbp
        112a:	48 83 3d 96 2e 00 00 	cmpq   $0x0,0x2e96(%rip)        # 3fc8 <__cxa_finalize@GLIBC_2.2.5>
        1131:	00 
        1132:	48 89 e5             	mov    %rsp,%rbp
        1135:	74 0c                	je     1143 <__do_global_dtors_aux+0x23>
        1137:	48 8b 3d 02 2f 00 00 	mov    0x2f02(%rip),%rdi        # 4040 <__dso_handle>
        113e:	e8 2d ff ff ff       	callq  1070 <__cxa_finalize@plt>
        1143:	e8 68 ff ff ff       	callq  10b0 <deregister_tm_clones>
        1148:	c6 05 21 30 00 00 01 	movb   $0x1,0x3021(%rip)        # 4170 <completed.7325>
        114f:	5d                   	pop    %rbp
        1150:	c3                   	retq   
        1151:	0f 1f 80 00 00 00 00 	nopl   0x0(%rax)
        1158:	c3                   	retq   
        1159:	0f 1f 80 00 00 00 00 	nopl   0x0(%rax)

    0000000000001160 <frame_dummy>:
        1160:	e9 7b ff ff ff       	jmpq   10e0 <register_tm_clones>

    0000000000001165 <main>:
        1165:	55                   	push   %rbp
        1166:	48 89 e5             	mov    %rsp,%rbp
        1169:	48 8d 35 95 0e 00 00 	lea    0xe95(%rip),%rsi        # 2005 <_ZStL19piecewise_construct+0x1>
        1170:	48 8d 3d e9 2e 00 00 	lea    0x2ee9(%rip),%rdi        # 4060 <_ZSt4cout@@GLIBCXX_3.4>
        1177:	e8 c4 fe ff ff       	callq  1040 <_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@plt>
        117c:	48 89 c2             	mov    %rax,%rdx
        117f:	48 8b 05 4a 2e 00 00 	mov    0x2e4a(%rip),%rax        # 3fd0 <_ZSt4endlIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_@GLIBCXX_3.4>
        1186:	48 89 c6             	mov    %rax,%rsi
        1189:	48 89 d7             	mov    %rdx,%rdi
        118c:	e8 bf fe ff ff       	callq  1050 <_ZNSolsEPFRSoS_E@plt>
        1191:	b8 00 00 00 00       	mov    $0x0,%eax
        1196:	5d                   	pop    %rbp
        1197:	c3                   	retq   

    0000000000001198 <_Z41__static_initialization_and_destruction_0ii>:
        1198:	55                   	push   %rbp
        1199:	48 89 e5             	mov    %rsp,%rbp
        119c:	48 83 ec 10          	sub    $0x10,%rsp
        11a0:	89 7d fc             	mov    %edi,-0x4(%rbp)
        11a3:	89 75 f8             	mov    %esi,-0x8(%rbp)
        11a6:	83 7d fc 01          	cmpl   $0x1,-0x4(%rbp)
        11aa:	75 32                	jne    11de <_Z41__static_initialization_and_destruction_0ii+0x46>
        11ac:	81 7d f8 ff ff 00 00 	cmpl   $0xffff,-0x8(%rbp)
        11b3:	75 29                	jne    11de <_Z41__static_initialization_and_destruction_0ii+0x46>
        11b5:	48 8d 3d b5 2f 00 00 	lea    0x2fb5(%rip),%rdi        # 4171 <_ZStL8__ioinit>
        11bc:	e8 9f fe ff ff       	callq  1060 <_ZNSt8ios_base4InitC1Ev@plt>
        11c1:	48 8d 15 78 2e 00 00 	lea    0x2e78(%rip),%rdx        # 4040 <__dso_handle>
        11c8:	48 8d 35 a2 2f 00 00 	lea    0x2fa2(%rip),%rsi        # 4171 <_ZStL8__ioinit>
        11cf:	48 8b 05 22 2e 00 00 	mov    0x2e22(%rip),%rax        # 3ff8 <_ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4>
        11d6:	48 89 c7             	mov    %rax,%rdi
        11d9:	e8 52 fe ff ff       	callq  1030 <__cxa_atexit@plt>
        11de:	90                   	nop
        11df:	c9                   	leaveq 
        11e0:	c3                   	retq   

    00000000000011e1 <_GLOBAL__sub_I_main>:
        11e1:	55                   	push   %rbp
        11e2:	48 89 e5             	mov    %rsp,%rbp
        11e5:	be ff ff 00 00       	mov    $0xffff,%esi
        11ea:	bf 01 00 00 00       	mov    $0x1,%edi
        11ef:	e8 a4 ff ff ff       	callq  1198 <_Z41__static_initialization_and_destruction_0ii>
        11f4:	5d                   	pop    %rbp
        11f5:	c3                   	retq   
        11f6:	66 2e 0f 1f 84 00 00 	nopw   %cs:0x0(%rax,%rax,1)
        11fd:	00 00 00 

    0000000000001200 <__libc_csu_init>:
        1200:	41 57                	push   %r15
        1202:	49 89 d7             	mov    %rdx,%r15
        1205:	41 56                	push   %r14
        1207:	49 89 f6             	mov    %rsi,%r14
        120a:	41 55                	push   %r13
        120c:	41 89 fd             	mov    %edi,%r13d
        120f:	41 54                	push   %r12
        1211:	4c 8d 25 88 2b 00 00 	lea    0x2b88(%rip),%r12        # 3da0 <__frame_dummy_init_array_entry>
        1218:	55                   	push   %rbp
        1219:	48 8d 2d 90 2b 00 00 	lea    0x2b90(%rip),%rbp        # 3db0 <__init_array_end>
        1220:	53                   	push   %rbx
        1221:	4c 29 e5             	sub    %r12,%rbp
        1224:	48 83 ec 08          	sub    $0x8,%rsp
        1228:	e8 d3 fd ff ff       	callq  1000 <_init>
        122d:	48 c1 fd 03          	sar    $0x3,%rbp
        1231:	74 1b                	je     124e <__libc_csu_init+0x4e>
        1233:	31 db                	xor    %ebx,%ebx
        1235:	0f 1f 00             	nopl   (%rax)
        1238:	4c 89 fa             	mov    %r15,%rdx
        123b:	4c 89 f6             	mov    %r14,%rsi
        123e:	44 89 ef             	mov    %r13d,%edi
        1241:	41 ff 14 dc          	callq  *(%r12,%rbx,8)
        1245:	48 83 c3 01          	add    $0x1,%rbx
        1249:	48 39 dd             	cmp    %rbx,%rbp
        124c:	75 ea                	jne    1238 <__libc_csu_init+0x38>
        124e:	48 83 c4 08          	add    $0x8,%rsp
        1252:	5b                   	pop    %rbx
        1253:	5d                   	pop    %rbp
        1254:	41 5c                	pop    %r12
        1256:	41 5d                	pop    %r13
        1258:	41 5e                	pop    %r14
        125a:	41 5f                	pop    %r15
        125c:	c3                   	retq   
        125d:	0f 1f 00             	nopl   (%rax)

    0000000000001260 <__libc_csu_fini>:
        1260:	c3                   	retq   

    Disassembly of section .fini:

    0000000000001264 <_fini>:
        1264:	48 83 ec 08          	sub    $0x8,%rsp
        1268:	48 83 c4 08          	add    $0x8,%rsp
        126c:	c3                   	retq   
