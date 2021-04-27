# libc6_2.24-3ubuntu1_amd64
Ubuntu GLIBC 2.24-3ubuntu1

```
MD5: 6ffb6029c0b4c6988fd97c324cb354a7
SHA1: 9bdc7f85eae570c04a463c8165c8f255bee7cb75
```

```
0x45556, 0x455aa, 0x455aa, 0x455b1, 0x455b8, 0x455bd, 0x455c7, 0x455d1, 0x455d4, 0xcd226, 0xcd22a, 0xcd22d, 0xcd232, 0xcd236, 0xcd23a, 0xcd242, 0xcd24a, 0xcd252, 0xcd26a, 0xcd271, 0xcd274, 0xcd277, 0xcd4ca, 0xcd4ce, 0xcd4d1, 0xcd4d6, 0xcd4da, 0xcd4de, 0xcd4e6, 0xcd4ea, 0xcd4f2, 0xcd4fa, 0xcd519, 0xcd51d, 0xcd524, 0xcd527, 0xf0a91, 0xf0a91, 0xf0a98, 0xf0a9d, 0xf0aa4, 0xf0aa7, 0xf1919, 0xf1919, 0xf1920, 0xf1925, 0xf192c, 0xf192f
```

## one_gadget
```
0x45556 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x455aa execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xf0a91 execve("/bin/sh", rsp+0x50, environ)
constraints:
  [rsp+0x50] == NULL

0xf1919 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xcd4f2 :
	<Bool reg_rdx_108639_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108641_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_108648_64{UNINITIALIZED} == 0x4e>
	<Bool True>
	<Bool reg_r9_108650_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108650_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0xcd4fa :
	<Bool !(reg_cc_dep1_108655_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rdx_108658_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool reg_rbp_108663_64{UNINITIALIZED} == 0x42>
	<Bool True>
	<Bool reg_r9_108665_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108665_64{UNINITIALIZED} == 0xffffffffffffff80>
libc_base + 0xcd242 :
	<Bool reg_rax_109552_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_109555_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_109562_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109562_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0xcd24a :
	<Bool reg_rax_109568_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_109570_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_109577_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109577_64{UNINITIALIZED} == 0xffff000000000000>
libc_base + 0xcd252 :
	<Bool !(reg_cc_dep1_109583_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rax_109586_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool True>
	<Bool reg_r15_109591_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109591_64{UNINITIALIZED} == 0xfffffffffffffc00>
libc_base + 0x455bd :
	<Bool reg_rax_108323_64{UNINITIALIZED} == 0xff00000000000000>
	<Bool True>
	<Bool reg_rsi_108325_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108325_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0x455c7 :
	<Bool reg_rax_108329_64{UNINITIALIZED} == 0xc000000000000000>
	<Bool True>
	<Bool reg_rsi_108331_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108331_64{UNINITIALIZED} == 0xf000000000000000>
libc_base + 0x455d1 :
	<Bool reg_rax_108335_64{UNINITIALIZED} == 0xfffe000000000000>
	<Bool True>
	<Bool reg_rsi_108337_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108337_64{UNINITIALIZED} == 0x2>
libc_base + 0xcd4ca :
	<Bool reg_rdx_108550_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_108553_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_108551_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rdx_108550_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4ce :
	<Bool reg_rdx_108560_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_108563_64{UNINITIALIZED} == 0x36>
	<Bool reg_rax_108561_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rdx_108560_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4d6 :
	<Bool reg_rdx_108580_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_108583_64{UNINITIALIZED} == 0x36>
	<Bool reg_rax_108581_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rdx_108580_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4da :
	<Bool reg_rdx_108591_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_108593_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rax_108590_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rdx_108591_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4de :
	<Bool reg_rdx_108600_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_108602_64{UNINITIALIZED} == 0x2>
	<Bool !(reg_cc_dep1_108604_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rdx_108600_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4e6 :
	<Bool reg_rbp_108613_64{UNINITIALIZED} == 0x37>
	<Bool reg_rdx_108615_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108616_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rdx_108615_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xcd4ea :
	<Bool reg_rdx_108625_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108627_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_108633_64{UNINITIALIZED} == 0x4a>
	<Bool (reg_rdx_108625_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xf0a9d :
	<Bool reg_rax_108682_64{UNINITIALIZED} == 0xffffffffc0000000>
	<Bool True>
	<Bool reg_rsi_108684_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108684_64{UNINITIALIZED} == 0xfffffffffffffe00>
libc_base + 0xf0aa4 :
	<Bool reg_rax_108687_64{UNINITIALIZED} == 0xe000000000000000>
	<Bool True>
	<Bool reg_rsi_108689_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108689_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xcd519 :
	<Bool reg_rbp_108836_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_r9_108838_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108838_64{UNINITIALIZED} == 0xfffffffffffff000>
libc_base + 0xf1925 :
	<Bool reg_rax_109672_64{UNINITIALIZED} == 0xfffffffffffe0000>
	<Bool True>
	<Bool reg_rsi_109674_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109674_64{UNINITIALIZED} == 0xffffffe000000000>
libc_base + 0xf192c :
	<Bool reg_rax_109677_64{UNINITIALIZED} == 0xf800000000000000>
	<Bool True>
	<Bool reg_rsi_109679_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109679_64{UNINITIALIZED} == 0xfffffffffe000000>
libc_base + 0x455b1 :
	<Bool True>
	<Bool reg_rax_108314_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108314_64{UNINITIALIZED} == 0xf000000000000000>
libc_base + 0x455b8 :
	<Bool True>
	<Bool reg_rax_108318_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108318_64{UNINITIALIZED} == 0xffffffff00000000>
libc_base + 0x455d4 :
	<Bool True>
	<Bool reg_rsi_108341_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108341_64{UNINITIALIZED} == 0xffe0000000000000>
libc_base + 0xcd4d1 :
	<Bool reg_rbp_108573_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_108571_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_108573_64{UNINITIALIZED} + 0xffffffffffffffb0 == 0xffffffffffffffb1>
libc_base + 0xf0a98 :
	<Bool True>
	<Bool reg_rax_108672_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108672_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xf0aa7 :
	<Bool True>
	<Bool reg_rsi_108693_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108693_64{UNINITIALIZED} == 0xf000000000000000>
libc_base + 0xcd51d :
	<Bool True>
	<Bool reg_r9_108846_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108846_64{UNINITIALIZED} == 0xffffffffffffc000>
libc_base + 0xcd524 :
	<Bool True>
	<Bool reg_r9_108850_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_108850_64{UNINITIALIZED} == 0xffffffffc0000000>
libc_base + 0xcd527 :
	<Bool True>
	<Bool reg_rsi_108855_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108855_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0xcd26a :
	<Bool True>
	<Bool reg_r15_108918_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108918_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xcd271 :
	<Bool True>
	<Bool reg_r15_108922_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108922_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xcd274 :
	<Bool True>
	<Bool reg_r15_108926_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108926_64{UNINITIALIZED} == 0xff80000000000000>
libc_base + 0xcd277 :
	<Bool True>
	<Bool reg_rsi_108931_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108931_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xcd226 :
	<Bool reg_rax_109493_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rdx_109494_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_109493_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd22a :
	<Bool reg_rax_109503_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rdx_109504_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_109503_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd232 :
	<Bool reg_rax_109521_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rdx_109522_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_109521_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd236 :
	<Bool reg_rax_109531_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rdx_109530_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_109531_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd23a :
	<Bool reg_rax_109540_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_109543_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_109540_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf1920 :
	<Bool True>
	<Bool reg_rax_109662_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109662_64{UNINITIALIZED} == 0xffffff8000000000>
libc_base + 0xf192f :
	<Bool True>
	<Bool reg_rsi_109683_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109683_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xcd22d :
	<Bool reg_rdx_109513_64{UNINITIALIZED} == 0x1>
libc_base + 0x455aa :
libc_base + 0xf0a91 :
libc_base + 0xf1919 :
```
