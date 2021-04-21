# libc6_2.27-3ubuntu1.4_amd64
Ubuntu GLIBC 2.27-3ubuntu1.4

```
MD5: 8ee8363b834ad2c65a05bd40c8e4623e
SHA1: 46e93283ff53133360e02a73ae5b5ba375410855
```

## one_gadget
```
0x4f3d5 execve("/bin/sh", rsp+0x40, environ)
constraints:
  rsp & 0xf == 0
  rcx == NULL

0x4f432 execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0x10a41c execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xe561e :
	<Bool reg_rbp_32350_64{UNINITIALIZED} == 0x6f>
	<Bool True>
	<Bool reg_rcx_32352_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_32352_64{UNINITIALIZED} == 0xfffffffe00000000>
libc_base + 0x10a428 :
	<Bool reg_rax_33330_64{UNINITIALIZED} == 0xffc0000000000000>
	<Bool True>
	<Bool reg_rsi_33332_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33332_64{UNINITIALIZED} == 0x8000000000000000>
libc_base + 0x10a42f :
	<Bool reg_rax_33335_64{UNINITIALIZED} == 0xfff8000000000000>
	<Bool True>
	<Bool reg_rsi_33337_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33337_64{UNINITIALIZED} == 0xffffffffffe00000>
libc_base + 0x4f445 :
	<Bool reg_rax_33403_64{UNINITIALIZED} == 0xfffffe0000000000>
	<Bool True>
	<Bool reg_rsi_33405_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33405_64{UNINITIALIZED} == 0xfffffe0000000000>
libc_base + 0x4f44f :
	<Bool reg_rax_33408_64{UNINITIALIZED} == 0xfffffffe00000000>
	<Bool True>
	<Bool reg_rsi_33410_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33410_64{UNINITIALIZED} == 0xffe0000000000000>
libc_base + 0x4f459 :
	<Bool reg_rax_33414_64{UNINITIALIZED} == 0xfffffffe00000000>
	<Bool True>
	<Bool reg_rsi_33416_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33416_64{UNINITIALIZED} == 0xffffffffffe00000>
libc_base + 0xe55d1 :
	<Bool reg_rcx_33494_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_33497_64{UNINITIALIZED} == 0x44>
	<Bool reg_rax_33495_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_33494_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe55d5 :
	<Bool reg_rcx_33502_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_33505_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_33503_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_33502_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe55dd :
	<Bool reg_rsi_33517_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_33520_64{UNINITIALIZED} == 0x4>
	<Bool reg_rax_33518_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_33517_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe55e1 :
	<Bool reg_rsi_33526_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_33528_64{UNINITIALIZED} == 0x44>
	<Bool reg_rax_33525_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_33526_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe55e5 :
	<Bool reg_rsi_33533_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_33535_64{UNINITIALIZED} == 0x1>
	<Bool !(reg_cc_dep1_33537_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rsi_33533_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe55ed :
	<Bool reg_rbp_33543_64{UNINITIALIZED} == 0x4>
	<Bool reg_rsi_33545_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_33546_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rsi_33545_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe55f1 :
	<Bool reg_rsi_33553_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_33555_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_33560_64{UNINITIALIZED} == 0x2>
	<Bool (reg_rsi_33553_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe55f9 :
	<Bool reg_rsi_33564_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_33566_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rcx_33569_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_33573_64{UNINITIALIZED} == 0x6a>
libc_base + 0xe5622 :
	<Bool True>
	<Bool reg_rcx_32360_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_32360_64{UNINITIALIZED} == 0xffffff0000000000>
libc_base + 0xe5629 :
	<Bool True>
	<Bool reg_rcx_32364_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_32364_64{UNINITIALIZED} == 0xffffffffffffffc0>
libc_base + 0xe562c :
	<Bool True>
	<Bool reg_rsi_32369_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_32369_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xe5434 :
	<Bool reg_rcx_32711_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rax_32712_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_32711_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5438 :
	<Bool reg_rcx_32718_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rax_32719_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_32718_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5440 :
	<Bool reg_rcx_32731_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_32732_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_32731_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5444 :
	<Bool reg_rcx_32739_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_32738_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_32739_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5448 :
	<Bool reg_rcx_32745_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_32748_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rcx_32745_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5450 :
	<Bool reg_rcx_32754_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_32757_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r13_32760_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5458 :
	<Bool reg_rcx_32766_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_32768_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r13_32771_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x10a423 :
	<Bool True>
	<Bool reg_rax_33320_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_33320_64{UNINITIALIZED} == 0xfffffffffffffc00>
libc_base + 0x10a432 :
	<Bool True>
	<Bool reg_rsi_33341_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33341_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0x4f439 :
	<Bool True>
	<Bool reg_rax_33394_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_33394_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0x4f440 :
	<Bool True>
	<Bool reg_rax_33398_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_33398_64{UNINITIALIZED} == 0xffffffffc0000000>
libc_base + 0x4f45c :
	<Bool True>
	<Bool reg_rsi_33420_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33420_64{UNINITIALIZED} == 0xffffffe000000000>
libc_base + 0xe55d8 :
	<Bool reg_rbp_33512_64{UNINITIALIZED} == 0x54>
	<Bool reg_rax_33510_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_33512_64{UNINITIALIZED} + 0xffffffffffffff90 == 0xffffffffffffffe4>
libc_base + 0xe5601 :
	<Bool !(reg_cc_dep1_33576_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rcx_33579_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_33583_64{UNINITIALIZED} == 0x6e>
libc_base + 0xe546f :
	<Bool True>
	<Bool reg_r13_34499_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_34499_64{UNINITIALIZED} == 0xffffffff00000000>
libc_base + 0xe5476 :
	<Bool True>
	<Bool reg_r13_34503_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_34503_64{UNINITIALIZED} == 0xff80000000000000>
libc_base + 0xe5479 :
	<Bool True>
	<Bool reg_r13_34507_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_34507_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0xe547c :
	<Bool True>
	<Bool reg_rsi_34512_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_34512_64{UNINITIALIZED} == 0xffff800000000000>
libc_base + 0xe565d :
	<Bool reg_rbp_31995_64{UNINITIALIZED} == 0x1>
	<Bool mem_ffffffffffffff89_31996_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5661 :
	<Bool reg_rbp_32002_64{UNINITIALIZED} == 0x7f>
	<Bool reg_rcx_32005_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5665 :
	<Bool reg_rbp_32009_64{UNINITIALIZED} == 0x4f>
	<Bool reg_rcx_32012_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5669 :
	<Bool reg_rbp_32016_64{UNINITIALIZED} == 0x56>
	<Bool reg_rcx_32018_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe566d :
	<Bool reg_rbp_32022_64{UNINITIALIZED} == 0x47>
	<Bool reg_rcx_32024_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5656 :
	<Bool reg_rbp_32028_64{UNINITIALIZED} == 0x77>
	<Bool mem_ffffffffffffffff_32029_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5460 :
	<Bool !(reg_cc_dep1_32777_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r13_32780_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5490 :
	<Bool reg_rbp_34843_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_34843_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe5494 :
	<Bool reg_rbp_34848_64{UNINITIALIZED} == 0x47>
	<Bool reg_r13_34851_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5497 :
	<Bool reg_rbp_34855_64{UNINITIALIZED} == 0x47>
	<Bool reg_r13_34858_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe549b :
	<Bool reg_rbp_34862_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r13_34864_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe543b :
	<Bool reg_rax_32725_64{UNINITIALIZED} == 0x1>
libc_base + 0xe549f :
	<Bool reg_r13_34868_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x10a41c :
libc_base + 0x4f432 :
```
