# libc6_2.24-3ubuntu2.2_amd64
Ubuntu GLIBC 2.24-3ubuntu2.2

```
MD5: cfcef452ef69ea2dd73d6f55d7607c2b
SHA1: 013fb4a88610a3d00572b93162dd9724be869210
```

```
0x45556, 0x455aa, 0x455aa, 0x455b1, 0x455b8, 0x455bd, 0x455c7, 0x455d1, 0x455d4, 0xcde26, 0xcde2a, 0xcde2d, 0xcde32, 0xcde36, 0xcde3a, 0xcde42, 0xcde4a, 0xcde52, 0xcde6a, 0xcde71, 0xcde74, 0xcde77, 0xce0ca, 0xce0ce, 0xce0d1, 0xce0d6, 0xce0da, 0xce0de, 0xce0e6, 0xce0ea, 0xce0f2, 0xce0fa, 0xce119, 0xce11d, 0xce124, 0xce127, 0xf1691, 0xf1691, 0xf1698, 0xf169d, 0xf16a4, 0xf16a7, 0xf2519, 0xf2519, 0xf2520, 0xf2525, 0xf252c, 0xf252f
```

## one_gadget
```
0x45556 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x455aa execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xf1691 execve("/bin/sh", rsp+0x50, environ)
constraints:
  [rsp+0x50] == NULL

0xf2519 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xce0f2 :
	<Bool reg_rdx_108389_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108391_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_108398_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_r9_108400_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108400_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0xce0fa :
	<Bool !(reg_cc_dep1_108405_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rdx_108408_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool reg_rbp_108413_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_r9_108415_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108415_64{UNINITIALIZED} == 0x2>
libc_base + 0xcde42 :
	<Bool reg_rax_110067_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_110070_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_110077_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_110077_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0xcde4a :
	<Bool reg_rax_110083_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_110085_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_110092_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_110092_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xcde52 :
	<Bool !(reg_cc_dep1_110098_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rax_110101_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool True>
	<Bool reg_r15_110106_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_110106_64{UNINITIALIZED} == 0xffffffffffffffe0>
libc_base + 0xce0ca :
	<Bool reg_rdx_108299_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_108302_64{UNINITIALIZED} == 0x2>
	<Bool reg_rax_108300_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rdx_108299_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0ce :
	<Bool reg_rdx_108309_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_108312_64{UNINITIALIZED} == 0x36>
	<Bool reg_rax_108310_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rdx_108309_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0d6 :
	<Bool reg_rdx_108328_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_108331_64{UNINITIALIZED} == 0x36>
	<Bool reg_rax_108329_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rdx_108328_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0da :
	<Bool reg_rdx_108340_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_108342_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rax_108339_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rdx_108340_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0de :
	<Bool reg_rdx_108349_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_108351_64{UNINITIALIZED} == 0x1>
	<Bool !(reg_cc_dep1_108353_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rdx_108349_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0e6 :
	<Bool reg_rbp_108362_64{UNINITIALIZED} == 0x37>
	<Bool reg_rdx_108364_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108365_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rdx_108364_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xce0ea :
	<Bool reg_rdx_108375_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108377_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_108383_64{UNINITIALIZED} == 0x42>
	<Bool (reg_rdx_108375_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xf169d :
	<Bool reg_rax_108686_64{UNINITIALIZED} == 0xffffffffffffe000>
	<Bool True>
	<Bool reg_rsi_108688_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108688_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xf16a4 :
	<Bool reg_rax_108691_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_rsi_108693_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108693_64{UNINITIALIZED} == 0xfffffffff0000000>
libc_base + 0x455bd :
	<Bool reg_rax_109207_64{UNINITIALIZED} == 0xffffffffffffffe0>
	<Bool True>
	<Bool reg_rsi_109209_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109209_64{UNINITIALIZED} == 0xffffffffffe00000>
libc_base + 0x455c7 :
	<Bool reg_rax_109213_64{UNINITIALIZED} == 0xffffffffe0000000>
	<Bool True>
	<Bool reg_rsi_109215_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109215_64{UNINITIALIZED} == 0x2>
libc_base + 0x455d1 :
	<Bool reg_rax_109219_64{UNINITIALIZED} == 0xffffffffffffff00>
	<Bool True>
	<Bool reg_rsi_109221_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109221_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xf2525 :
	<Bool reg_rax_109276_64{UNINITIALIZED} == 0xfffffffffffffe00>
	<Bool True>
	<Bool reg_rsi_109278_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109278_64{UNINITIALIZED} == 0xffc0000000000000>
libc_base + 0xf252c :
	<Bool reg_rax_109281_64{UNINITIALIZED} == 0xfffffffffffc0000>
	<Bool True>
	<Bool reg_rsi_109283_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109283_64{UNINITIALIZED} == 0xffffffffc0000000>
libc_base + 0xce119 :
	<Bool reg_rbp_109504_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_r9_109506_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109506_64{UNINITIALIZED} == 0xffffffff80000000>
libc_base + 0xce0d1 :
	<Bool reg_rbp_108321_64{UNINITIALIZED} == 0x2a>
	<Bool reg_rax_108319_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_108321_64{UNINITIALIZED} + 0xffffffffffffffb0 == 0xffffffffffffffda>
libc_base + 0xf1698 :
	<Bool True>
	<Bool reg_rax_108676_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108676_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0xf16a7 :
	<Bool True>
	<Bool reg_rsi_108697_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108697_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0x455b1 :
	<Bool True>
	<Bool reg_rax_109198_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109198_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0x455b8 :
	<Bool True>
	<Bool reg_rax_109202_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109202_64{UNINITIALIZED} == 0xffff800000000000>
libc_base + 0x455d4 :
	<Bool True>
	<Bool reg_rsi_109225_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109225_64{UNINITIALIZED} == 0xfffff00000000000>
libc_base + 0xf2520 :
	<Bool True>
	<Bool reg_rax_109266_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109266_64{UNINITIALIZED} == 0xfffffffff8000000>
libc_base + 0xf252f :
	<Bool True>
	<Bool reg_rsi_109287_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109287_64{UNINITIALIZED} == 0xfffffffffffffe00>
libc_base + 0xce11d :
	<Bool True>
	<Bool reg_r9_109514_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109514_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xce124 :
	<Bool True>
	<Bool reg_r9_109518_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109518_64{UNINITIALIZED} == 0xffffffe000000000>
libc_base + 0xce127 :
	<Bool True>
	<Bool reg_rsi_109523_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109523_64{UNINITIALIZED} == 0xffffffffffc00000>
libc_base + 0xcde6a :
	<Bool True>
	<Bool reg_r15_109652_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109652_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0xcde71 :
	<Bool True>
	<Bool reg_r15_109656_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109656_64{UNINITIALIZED} == 0xfffffffffffffff0>
libc_base + 0xcde74 :
	<Bool True>
	<Bool reg_r15_109660_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109660_64{UNINITIALIZED} == 0xffffffffffff0000>
libc_base + 0xcde77 :
	<Bool True>
	<Bool reg_rsi_109665_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109665_64{UNINITIALIZED} == 0xfffffffff8000000>
libc_base + 0xcde26 :
	<Bool reg_rax_110008_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rdx_110009_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_110008_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde2a :
	<Bool reg_rax_110018_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rdx_110019_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_110018_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde32 :
	<Bool reg_rax_110037_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rdx_110038_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_110037_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde36 :
	<Bool reg_rax_110047_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rdx_110046_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_110047_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde3a :
	<Bool reg_rax_110056_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_110059_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_110056_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde2d :
	<Bool reg_rdx_110028_64{UNINITIALIZED} == 0x1>
libc_base + 0xf1691 :
libc_base + 0x455aa :
libc_base + 0xf2519 :
```
