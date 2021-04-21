# libc6_2.26-0ubuntu2.1_amd64
Ubuntu GLIBC 2.26-0ubuntu2.1

```
MD5: 522a2681d9ccad1ed953f8f61f2f42d1
SHA1: cc8df6278e095fcc4ca8a98e1f1c69c04db30a4c
```

## one_gadget
```
0x47c46 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x47c9a execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xfccde execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0xfdb8e execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xd9a5c :
	<Bool reg_rbp_108439_64{UNINITIALIZED} == 0x97>
	<Bool True>
	<Bool mem_7_108440_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_7_108440_64{UNINITIALIZED} == 0xfffffffffff00000>
libc_base + 0xd9a63 :
	<Bool reg_rbp_108445_64{UNINITIALIZED} == 0x97>
	<Bool True>
	<Bool mem_7_108446_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_7_108446_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0xd9a6a :
	<Bool reg_rbp_108452_64{UNINITIALIZED} == 0x3f>
	<Bool True>
	<Bool mem_ffffffffffffffaf_108453_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_ffffffffffffffaf_108453_64{UNINITIALIZED} == 0xfffff00000000000>
libc_base + 0xd9a72 :
	<Bool reg_rbp_108459_64{UNINITIALIZED} == 0x8a>
	<Bool True>
	<Bool mem_fffffffffffffffa_108460_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_fffffffffffffffa_108460_64{UNINITIALIZED} == 0xffffffffffe00000>
libc_base + 0xd9a79 :
	<Bool reg_rbp_108466_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_rcx_108470_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108470_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0xd9a7d :
	<Bool reg_rbp_108473_64{UNINITIALIZED} == 0x54>
	<Bool True>
	<Bool reg_rcx_108476_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108476_64{UNINITIALIZED} == 0xffffff0000000000>
libc_base + 0xd9a81 :
	<Bool reg_rbp_108479_64{UNINITIALIZED} == 0x47>
	<Bool True>
	<Bool reg_rcx_108482_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108482_64{UNINITIALIZED} == 0xffffffffffff8000>
libc_base + 0xd9a85 :
	<Bool reg_rbp_108485_64{UNINITIALIZED} == 0x42>
	<Bool True>
	<Bool reg_rcx_108487_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108487_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xfccea :
	<Bool reg_rax_108679_64{UNINITIALIZED} == 0xffffffffffff8000>
	<Bool True>
	<Bool reg_rsi_108681_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108681_64{UNINITIALIZED} == 0xfffffffffffffc00>
libc_base + 0xfccf1 :
	<Bool reg_rax_108684_64{UNINITIALIZED} == 0xfffffffffffffe00>
	<Bool True>
	<Bool reg_rsi_108686_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108686_64{UNINITIALIZED} == 0xfffffffffffffff0>
libc_base + 0xd9a38 :
	<Bool reg_rbp_108739_64{UNINITIALIZED} == 0x6e>
	<Bool True>
	<Bool reg_rcx_108741_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108741_64{UNINITIALIZED} == 0xfffffffff8000000>
libc_base + 0x47cad :
	<Bool reg_rax_109728_64{UNINITIALIZED} == 0xffffffffffe00000>
	<Bool True>
	<Bool reg_rsi_109730_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109730_64{UNINITIALIZED} == 0xffffff0000000000>
libc_base + 0x47cb7 :
	<Bool reg_rax_109734_64{UNINITIALIZED} == 0xfffffffffff80000>
	<Bool True>
	<Bool reg_rsi_109736_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109736_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0x47cc1 :
	<Bool reg_rax_109740_64{UNINITIALIZED} == 0xffffffffffffffff>
	<Bool True>
	<Bool reg_rsi_109742_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109742_64{UNINITIALIZED} == 0xfffffffe00000000>
libc_base + 0xfdb9a :
	<Bool reg_rax_109845_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_rsi_109847_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109847_64{UNINITIALIZED} == 0xff80000000000000>
libc_base + 0xfdba1 :
	<Bool reg_rax_109850_64{UNINITIALIZED} == 0xffffffff00000000>
	<Bool True>
	<Bool reg_rsi_109852_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109852_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0xd989a :
	<Bool reg_rbp_109927_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_r13_109930_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109930_64{UNINITIALIZED} == 0xfe00000000000000>
libc_base + 0xfcce5 :
	<Bool True>
	<Bool reg_rax_108669_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108669_64{UNINITIALIZED} == 0xfffffffffff80000>
libc_base + 0xfccf4 :
	<Bool True>
	<Bool reg_rsi_108690_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108690_64{UNINITIALIZED} == 0xfffffffe00000000>
libc_base + 0xd9a3c :
	<Bool True>
	<Bool reg_rcx_108749_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108749_64{UNINITIALIZED} == 0xfffffffffff80000>
libc_base + 0xd9a43 :
	<Bool True>
	<Bool reg_rcx_108753_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_108753_64{UNINITIALIZED} == 0xf000000000000000>
libc_base + 0xd9a46 :
	<Bool True>
	<Bool reg_rsi_108758_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108758_64{UNINITIALIZED} == 0xffffff0000000000>
libc_base + 0xd9763 :
	<Bool True>
	<Bool reg_r13_109189_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109189_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xd976a :
	<Bool True>
	<Bool reg_r13_109193_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109193_64{UNINITIALIZED} == 0xfff8000000000000>
libc_base + 0xd976d :
	<Bool True>
	<Bool reg_r13_109197_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109197_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0xd9770 :
	<Bool True>
	<Bool reg_rsi_109202_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109202_64{UNINITIALIZED} == 0xffffffffffffffe0>
libc_base + 0x47ca1 :
	<Bool True>
	<Bool reg_rax_109719_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109719_64{UNINITIALIZED} == 0xfffffffffffffe00>
libc_base + 0x47ca8 :
	<Bool True>
	<Bool reg_rax_109723_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109723_64{UNINITIALIZED} == 0x8000000000000000>
libc_base + 0x47cc4 :
	<Bool True>
	<Bool reg_rsi_109746_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109746_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0xfdb95 :
	<Bool True>
	<Bool reg_rax_109835_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109835_64{UNINITIALIZED} == 0xff80000000000000>
libc_base + 0xfdba4 :
	<Bool True>
	<Bool reg_rsi_109856_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109856_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xd989e :
	<Bool True>
	<Bool reg_r13_109934_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109934_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xd9887 :
	<Bool reg_rbp_109909_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_109909_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xd988a :
	<Bool reg_rbp_109914_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_109914_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xd988e :
	<Bool reg_rbp_109919_64{UNINITIALIZED} == 0x3f>
	<Bool 0xffffffffffffffb0 + reg_rbp_109919_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xd9896 :
	<Bool reg_rbp_109923_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_109923_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xfccde :
libc_base + 0x47c9a :
libc_base + 0xfdb8e :
```
