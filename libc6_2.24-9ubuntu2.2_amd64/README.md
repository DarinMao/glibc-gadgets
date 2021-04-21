# libc6_2.24-9ubuntu2.2_amd64
Ubuntu GLIBC 2.24-9ubuntu2.2

```
MD5: 82ff57d04eb11340b072a4996e7bf89f
SHA1: 4e5dfd832191073e18a09728f68666b6465eeacd
```

## one_gadget
```
0x45526 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x4557a execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xf1651 execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0xf24cb execve("/bin/sh", rsp+0x60, environ)
constraints:
  [rsp+0x60] == NULL
```

## angry_gadget
```
libc_base + 0xce0c6 :
	<Bool reg_rax_109882_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_109884_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_109890_64{UNINITIALIZED} == 0x4e>
	<Bool True>
	<Bool reg_r9_109892_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109892_64{UNINITIALIZED} == 0xffffffffffffffe0>
libc_base + 0xce0ce :
	<Bool !(reg_cc_dep1_109904_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rax_109907_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool reg_rbp_109911_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_r9_109913_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109913_64{UNINITIALIZED} == 0xfffffffffff00000>
libc_base + 0xcde1d :
	<Bool reg_rax_108596_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_108599_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_108605_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108605_64{UNINITIALIZED} == 0xfffff00000000000>
libc_base + 0xcde25 :
	<Bool reg_rax_108616_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_108618_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_108624_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108624_64{UNINITIALIZED} == 0xffffffffffff0000>
libc_base + 0xcde2d :
	<Bool !(reg_cc_dep1_108635_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rax_108638_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool True>
	<Bool reg_r15_108642_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108642_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0xf165d :
	<Bool reg_rax_109080_64{UNINITIALIZED} == 0xfc00000000000000>
	<Bool True>
	<Bool reg_rsi_109082_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109082_64{UNINITIALIZED} == 0xfffffffc00000000>
libc_base + 0xf1664 :
	<Bool reg_rax_109085_64{UNINITIALIZED} == 0xffffffffffffffe0>
	<Bool True>
	<Bool reg_rsi_109087_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109087_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xce0e5 :
	<Bool reg_rbp_109206_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_r9_109208_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109208_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0x4558d :
	<Bool reg_rax_109364_64{UNINITIALIZED} == 0xffffffe000000000>
	<Bool True>
	<Bool reg_rsi_109366_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109366_64{UNINITIALIZED} == 0xfffffff000000000>
libc_base + 0x45597 :
	<Bool reg_rax_109370_64{UNINITIALIZED} == 0x8000000000000000>
	<Bool True>
	<Bool reg_rsi_109372_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109372_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0x455a1 :
	<Bool reg_rax_109376_64{UNINITIALIZED} == 0xff00000000000000>
	<Bool True>
	<Bool reg_rsi_109378_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109378_64{UNINITIALIZED} == 0xffffffffffffe000>
libc_base + 0xce09e :
	<Bool reg_rax_109764_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_109767_64{UNINITIALIZED} == 0x37>
	<Bool reg_rsi_109765_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_109764_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0a2 :
	<Bool reg_rax_109777_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_109780_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rsi_109778_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_109777_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0aa :
	<Bool reg_rax_109807_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_109810_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rsi_109808_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_109807_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0ae :
	<Bool reg_rax_109818_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_109820_64{UNINITIALIZED} == 0x2a>
	<Bool reg_rsi_109817_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_109818_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0b2 :
	<Bool reg_rax_109831_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_109833_64{UNINITIALIZED} == 0x1a>
	<Bool !(reg_cc_dep1_109835_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_109831_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xce0ba :
	<Bool reg_rbp_109849_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_109851_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_109852_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_109851_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xce0be :
	<Bool reg_rax_109866_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_109868_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_109873_64{UNINITIALIZED} == 0x42>
	<Bool (reg_rax_109866_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xf24d7 :
	<Bool reg_rax_110189_64{UNINITIALIZED} == 0xffe0000000000000>
	<Bool True>
	<Bool reg_rsi_110191_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110191_64{UNINITIALIZED} == 0xfffffffffffffc00>
libc_base + 0xf24de :
	<Bool reg_rax_110194_64{UNINITIALIZED} == 0xffff000000000000>
	<Bool True>
	<Bool reg_rsi_110196_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110196_64{UNINITIALIZED} == 0xfff8000000000000>
libc_base + 0xcde01 :
	<Bool reg_rax_108505_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rcx_108506_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_108505_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde05 :
	<Bool reg_rax_108521_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rcx_108522_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_108521_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde0d :
	<Bool reg_rax_108549_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rcx_108550_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_108549_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde11 :
	<Bool reg_rax_108565_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rcx_108564_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_108565_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde15 :
	<Bool reg_rax_108579_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_108582_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_108579_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcde41 :
	<Bool True>
	<Bool reg_r15_108654_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108654_64{UNINITIALIZED} == 0xfffffffffff80000>
libc_base + 0xcde48 :
	<Bool True>
	<Bool reg_r15_108658_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108658_64{UNINITIALIZED} == 0xffffffffffff0000>
libc_base + 0xcde4b :
	<Bool True>
	<Bool reg_r15_108662_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_108662_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xcde4e :
	<Bool True>
	<Bool reg_rsi_108667_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108667_64{UNINITIALIZED} == 0xfffffffffe000000>
libc_base + 0xf1658 :
	<Bool True>
	<Bool reg_rax_109070_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109070_64{UNINITIALIZED} == 0xffff000000000000>
libc_base + 0xf1667 :
	<Bool True>
	<Bool reg_rsi_109091_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109091_64{UNINITIALIZED} == 0xffffffff80000000>
libc_base + 0xce0e9 :
	<Bool True>
	<Bool reg_r9_109216_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109216_64{UNINITIALIZED} == 0xffffe00000000000>
libc_base + 0xce0f0 :
	<Bool True>
	<Bool reg_r9_109220_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109220_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xce0f3 :
	<Bool True>
	<Bool reg_rsi_109225_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109225_64{UNINITIALIZED} == 0xfffffffffff00000>
libc_base + 0x45581 :
	<Bool True>
	<Bool reg_rax_109355_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109355_64{UNINITIALIZED} == 0xfffffffffe000000>
libc_base + 0x45588 :
	<Bool True>
	<Bool reg_rax_109359_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109359_64{UNINITIALIZED} == 0xffffffffffffffc0>
libc_base + 0x455a4 :
	<Bool True>
	<Bool reg_rsi_109382_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109382_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0xce0a5 :
	<Bool reg_rbp_109793_64{UNINITIALIZED} == 0x37>
	<Bool reg_rsi_109791_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_109793_64{UNINITIALIZED} + 0xffffffffffffffb0 == 0xffffffffffffffe7>
libc_base + 0xf24d2 :
	<Bool True>
	<Bool reg_rax_110179_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_110179_64{UNINITIALIZED} == 0x2>
libc_base + 0xf24e1 :
	<Bool True>
	<Bool reg_rsi_110200_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110200_64{UNINITIALIZED} == 0xffffffc000000000>
libc_base + 0xcde08 :
	<Bool reg_rcx_108536_64{UNINITIALIZED} == 0x1>
libc_base + 0xf1651 :
libc_base + 0x4557a :
libc_base + 0xf24cb :
```
