# libc6_2.23-0ubuntu3_amd64
Ubuntu GLIBC 2.23-0ubuntu3

```
MD5: d443f227870b9c29182cc7a7a007d881
SHA1: 375198810bb39e6593a968fcbcf6556789026743
```

```
0x45206, 0x4525a, 0x4525a, 0x45261, 0x45268, 0x4526d, 0x45277, 0x45281, 0x45284, 0x6f4fb, 0x6f4fe, 0x6f501, 0x6f503, 0xcc673, 0xcc67a, 0xcc748, 0xcc74f, 0xcc752, 0xef9f4, 0xef9f4, 0xef9fb, 0xefa00, 0xefa07, 0xefa0a, 0xf0897, 0xf0897, 0xf089e, 0xf08a3, 0xf08aa, 0xf08ad, 0xf59f9, 0xf5a01, 0xf5a09, 0xf5d9a, 0xf5d9f, 0xf5da2, 0xf5da6, 0xf5da9, 0xf5db1, 0xf5db9, 0xf5dc1, 0xf5e40, 0xf5e47
```

## one_gadget
```
0x45206 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x4525a execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xef9f4 execve("/bin/sh", rsp+0x50, environ)
constraints:
  [rsp+0x50] == NULL

0xf0897 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xf5db1 :
	<Bool reg_rbx_113384_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_113387_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113395_64{UNINITIALIZED} == 0xf7>
	<Bool True>
	<Bool reg_rcx_113397_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113397_64{UNINITIALIZED} == 0xffc0000000000000>
libc_base + 0xf5db9 :
	<Bool reg_rbx_113400_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_113402_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113410_64{UNINITIALIZED} == 0xc2>
	<Bool True>
	<Bool reg_rcx_113412_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113412_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xf59f9 :
	<Bool reg_r12_114020_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_114023_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_114026_64{UNINITIALIZED} == 0x7a>
	<Bool True>
	<Bool reg_r13_114028_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_114028_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xf5a01 :
	<Bool reg_r12_114037_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_114039_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_114042_64{UNINITIALIZED} == 0xf7>
	<Bool True>
	<Bool reg_r13_114044_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_114044_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0xf5dc1 :
	<Bool !(reg_cc_dep1_113415_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113423_64{UNINITIALIZED} == 0x7a>
	<Bool True>
	<Bool reg_rcx_113425_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113425_64{UNINITIALIZED} == 0xffff800000000000>
libc_base + 0xf5a09 :
	<Bool !(reg_cc_dep1_114054_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_114057_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_r13_114059_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_114059_64{UNINITIALIZED} == 0xfffffffffffffff8>
libc_base + 0xf5e40 :
	<Bool reg_rbp_113158_64{UNINITIALIZED} == 0xf6>
	<Bool True>
	<Bool reg_rcx_113160_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113160_64{UNINITIALIZED} == 0xffffffffffffffc0>
libc_base + 0xf5e47 :
	<Bool reg_rbp_113163_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_rcx_113165_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113165_64{UNINITIALIZED} == 0xffffffffffffff00>
libc_base + 0xf5d9a :
	<Bool reg_rsi_113332_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool True>
	<Bool reg_rbp_113338_64{UNINITIALIZED} + 0xffffffffffffff08 <= 0xffffffffffffffff>
	<Bool reg_rbp_113338_64{UNINITIALIZED} + 0xffffffffffffff08 == 0xffffffffffffff82>
libc_base + 0xf5d9f :
	<Bool reg_r8_113341_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rsi_113342_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool reg_rbp_113348_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r8_113341_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf5da2 :
	<Bool reg_rbx_113351_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rsi_113352_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool reg_rbp_113358_64{UNINITIALIZED} == 0xf6>
	<Bool (reg_rbx_113351_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf5da6 :
	<Bool reg_rbx_113362_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rsi_113361_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool reg_rbp_113368_64{UNINITIALIZED} == 0xe2>
	<Bool (reg_rbx_113362_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf5da9 :
	<Bool reg_rbx_113371_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_113374_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113381_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rbx_113371_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xefa00 :
	<Bool reg_rax_113440_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_rsi_113442_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113442_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xefa07 :
	<Bool reg_rax_113445_64{UNINITIALIZED} == 0xffffffff00000000>
	<Bool True>
	<Bool reg_rsi_113447_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113447_64{UNINITIALIZED} == 0xfffffffe00000000>
libc_base + 0x4526d :
	<Bool reg_rax_113825_64{UNINITIALIZED} == 0xffc0000000000000>
	<Bool True>
	<Bool reg_rsi_113827_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113827_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0x45277 :
	<Bool reg_rax_113831_64{UNINITIALIZED} == 0xffe0000000000000>
	<Bool True>
	<Bool reg_rsi_113833_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113833_64{UNINITIALIZED} == 0xfffffffff0000000>
libc_base + 0x45281 :
	<Bool reg_rax_113837_64{UNINITIALIZED} == 0xf000000000000000>
	<Bool True>
	<Bool reg_rsi_113839_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113839_64{UNINITIALIZED} == 0xfffffe0000000000>
libc_base + 0xf08a3 :
	<Bool reg_rax_114145_64{UNINITIALIZED} == 0xfffffffe00000000>
	<Bool True>
	<Bool reg_rsi_114147_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114147_64{UNINITIALIZED} == 0xfffffffffffffc00>
libc_base + 0xf08aa :
	<Bool reg_rax_114150_64{UNINITIALIZED} == 0xfffffffffffffe00>
	<Bool True>
	<Bool reg_rsi_114152_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114152_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0xcc673 :
	<Bool True>
	<Bool reg_rcx_112952_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_112952_64{UNINITIALIZED} == 0xfffffffffe000000>
libc_base + 0xcc67a :
	<Bool True>
	<Bool reg_rcx_112956_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_112956_64{UNINITIALIZED} == 0xfffffffffffe0000>
libc_base + 0xef9fb :
	<Bool True>
	<Bool reg_rax_113430_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113430_64{UNINITIALIZED} == 0xfffffffffff80000>
libc_base + 0xefa0a :
	<Bool True>
	<Bool reg_rsi_113451_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113451_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xcc748 :
	<Bool True>
	<Bool reg_rax_113500_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113500_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xcc74f :
	<Bool True>
	<Bool reg_rax_113504_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113504_64{UNINITIALIZED} == 0xffffffffff000000>
libc_base + 0xcc752 :
	<Bool True>
	<Bool reg_rsi_113510_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113510_64{UNINITIALIZED} == 0xfffffffe00000000>
libc_base + 0x45261 :
	<Bool True>
	<Bool reg_rax_113816_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113816_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0x45268 :
	<Bool True>
	<Bool reg_rax_113820_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113820_64{UNINITIALIZED} == 0xffffffffffffff80>
libc_base + 0x45284 :
	<Bool True>
	<Bool reg_rsi_113843_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113843_64{UNINITIALIZED} == 0xffe0000000000000>
libc_base + 0xf089e :
	<Bool True>
	<Bool reg_rax_114135_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_114135_64{UNINITIALIZED} == 0xfffffffffffff000>
libc_base + 0xf08ad :
	<Bool True>
	<Bool reg_rsi_114156_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114156_64{UNINITIALIZED} == 0xffffffffff000000>
libc_base + 0x6f4fb :
	<Bool reg_rsi_113586_64{UNINITIALIZED} == 0x0>
libc_base + 0x6f4fe :
	<Bool reg_rsi_113596_64{UNINITIALIZED} == 0x0>
libc_base + 0x6f501 :
	<Bool reg_rsi_113607_64{UNINITIALIZED} == 0x0>
libc_base + 0x6f503 :
	<Bool reg_rsi_113619_64{UNINITIALIZED} == 0x0>
libc_base + 0xef9f4 :
libc_base + 0x4525a :
libc_base + 0xf0897 :
```
