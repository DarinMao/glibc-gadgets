# libc6_2.27-3ubuntu1_amd64
Ubuntu GLIBC 2.27-3ubuntu1

```
MD5: 50390b2ae8aaa73c47745040f54e602f
SHA1: 18292bd12d37bfaf58e8dded9db7f1f5da1192cb
```

## one_gadget
```
0x4f2c5 execve("/bin/sh", rsp+0x40, environ)
constraints:
  rsp & 0xf == 0
  rcx == NULL

0x4f322 execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0x10a38c execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0x4f335 :
	<Bool reg_rax_33249_64{UNINITIALIZED} == 0xfffffffffffe0000>
	<Bool True>
	<Bool reg_rsi_33251_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33251_64{UNINITIALIZED} == 0xffffffe000000000>
libc_base + 0x4f33f :
	<Bool reg_rax_33255_64{UNINITIALIZED} == 0xfffff00000000000>
	<Bool True>
	<Bool reg_rsi_33257_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33257_64{UNINITIALIZED} == 0xf000000000000000>
libc_base + 0x4f349 :
	<Bool reg_rax_33261_64{UNINITIALIZED} == 0xfffffffffc000000>
	<Bool True>
	<Bool reg_rsi_33263_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33263_64{UNINITIALIZED} == 0x8000000000000000>
libc_base + 0xe585f :
	<Bool reg_rbp_33624_64{UNINITIALIZED} == 0x6f>
	<Bool True>
	<Bool reg_r10_33626_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_33626_64{UNINITIALIZED} == 0xffffffffffe00000>
libc_base + 0xe5812 :
	<Bool reg_rax_34023_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_34026_64{UNINITIALIZED} == 0x4c>
	<Bool reg_rcx_34024_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_34023_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5816 :
	<Bool reg_rax_34031_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_34034_64{UNINITIALIZED} == 0x56>
	<Bool reg_rcx_34032_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_34031_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe581e :
	<Bool reg_rax_34046_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_34049_64{UNINITIALIZED} == 0x57>
	<Bool reg_rcx_34047_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_34046_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5822 :
	<Bool reg_rax_34055_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_34057_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_34054_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_34055_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5826 :
	<Bool reg_rax_34062_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_34064_64{UNINITIALIZED} == 0x2>
	<Bool !(reg_cc_dep1_34066_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_34062_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe582e :
	<Bool reg_rbp_34072_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_34074_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_34075_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_34074_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe5832 :
	<Bool reg_rax_34082_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_34084_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_34089_64{UNINITIALIZED} == 0x62>
	<Bool (reg_rax_34082_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe583a :
	<Bool reg_rax_34093_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_34095_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_34098_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_34102_64{UNINITIALIZED} == 0x6e>
libc_base + 0x10a398 :
	<Bool reg_rax_34760_64{UNINITIALIZED} == 0xfffffc0000000000>
	<Bool True>
	<Bool reg_rsi_34762_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_34762_64{UNINITIALIZED} == 0xffffffffffff0000>
libc_base + 0x10a39f :
	<Bool reg_rax_34765_64{UNINITIALIZED} == 0xe000000000000000>
	<Bool True>
	<Bool reg_rsi_34767_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_34767_64{UNINITIALIZED} == 0xffffffc000000000>
libc_base + 0xe5664 :
	<Bool reg_rcx_31939_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rax_31940_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_31939_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5668 :
	<Bool reg_rcx_31946_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rax_31947_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_31946_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5670 :
	<Bool reg_rcx_31959_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_31960_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_31959_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5674 :
	<Bool reg_rcx_31967_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_31966_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_31967_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5678 :
	<Bool reg_rcx_31973_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_31976_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rcx_31973_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5680 :
	<Bool reg_rcx_31982_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_31985_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r14_31988_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5688 :
	<Bool reg_rcx_31994_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_31996_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r14_31999_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x4f329 :
	<Bool True>
	<Bool reg_rax_33240_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_33240_64{UNINITIALIZED} == 0xffffffffffffff00>
libc_base + 0x4f330 :
	<Bool True>
	<Bool reg_rax_33244_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_33244_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0x4f34c :
	<Bool True>
	<Bool reg_rsi_33267_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33267_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0xe569f :
	<Bool True>
	<Bool reg_r14_33307_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r14_33307_64{UNINITIALIZED} == 0xffffffff00000000>
libc_base + 0xe56a6 :
	<Bool True>
	<Bool reg_r14_33311_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r14_33311_64{UNINITIALIZED} == 0xfffffffe00000000>
libc_base + 0xe56a9 :
	<Bool True>
	<Bool reg_r14_33315_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r14_33315_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xe56ac :
	<Bool True>
	<Bool reg_rsi_33320_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33320_64{UNINITIALIZED} == 0xfffffffff8000000>
libc_base + 0xe5863 :
	<Bool True>
	<Bool reg_r10_33634_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_33634_64{UNINITIALIZED} == 0xffffffffff800000>
libc_base + 0xe586a :
	<Bool True>
	<Bool reg_r10_33638_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_33638_64{UNINITIALIZED} == 0xffff800000000000>
libc_base + 0xe586d :
	<Bool True>
	<Bool reg_rsi_33643_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33643_64{UNINITIALIZED} == 0xffffffe000000000>
libc_base + 0xe5819 :
	<Bool reg_rbp_34041_64{UNINITIALIZED} == 0x4c>
	<Bool reg_rcx_34039_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_34041_64{UNINITIALIZED} + 0xffffffffffffff90 == 0xffffffffffffffdc>
libc_base + 0xe5842 :
	<Bool !(reg_cc_dep1_34105_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_34108_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_34112_64{UNINITIALIZED} == 0x2>
libc_base + 0x10a393 :
	<Bool True>
	<Bool reg_rax_34750_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_34750_64{UNINITIALIZED} == 0x2>
libc_base + 0x10a3a2 :
	<Bool True>
	<Bool reg_rsi_34771_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_34771_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0xe5690 :
	<Bool !(reg_cc_dep1_32005_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r14_32008_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe56c0 :
	<Bool reg_rbp_34120_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_34120_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe56c4 :
	<Bool reg_rbp_34125_64{UNINITIALIZED} == 0x47>
	<Bool reg_r14_34128_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe56c7 :
	<Bool reg_rbp_34132_64{UNINITIALIZED} == 0x47>
	<Bool reg_r14_34135_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe56cb :
	<Bool reg_rbp_34139_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r14_34141_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe588b :
	<Bool reg_rbp_34833_64{UNINITIALIZED} == 0x7f>
	<Bool reg_r10_34836_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe588f :
	<Bool reg_rbp_34840_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_34843_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5893 :
	<Bool reg_rbp_34847_64{UNINITIALIZED} == 0x56>
	<Bool reg_r10_34849_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5897 :
	<Bool reg_rbp_34853_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_34855_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe566b :
	<Bool reg_rax_31953_64{UNINITIALIZED} == 0x1>
libc_base + 0xe56cf :
	<Bool reg_r14_34145_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x4f322 :
libc_base + 0x10a38c :
```
