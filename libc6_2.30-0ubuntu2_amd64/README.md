# libc6_2.30-0ubuntu2_amd64
Ubuntu GLIBC 2.30-0ubuntu2

```
MD5: a94f33f0d81f9c62022a288a4ee49a83
SHA1: b1817619deaef57c422d292390ab82759226b5f7
```

```
0x10afa9, 0x10afa9, 0x10afb0, 0x10afb5, 0x10afbc, 0x10afbf, 0xe696a, 0xe696e, 0xe6972, 0xe6975, 0xe697c, 0xe6984, 0xe698c, 0xe6990, 0xe6996, 0xe699e, 0xe69a1, 0xe6b66, 0xe6b69, 0xe6b6d, 0xe6b71, 0xe6b79, 0xe6b7d, 0xe6b85, 0xe6b89, 0xe6b8b, 0xe6b93, 0xe6b93, 0xe6b96, 0xe6b96, 0xe6b99, 0xe6c09, 0xe6c0d, 0xe6c10, 0xe6c14, 0xe6c18, 0xe6c4e, 0xe6c51, 0xe6c55, 0xe6c59, 0xe6c5d, 0xe6c61
```

## one_gadget
```
0xe6b93 execve("/bin/sh", r10, r12)
constraints:
  [r10] == NULL || r10 == NULL
  [r12] == NULL || r12 == NULL

0xe6b96 execve("/bin/sh", r10, rdx)
constraints:
  [r10] == NULL || r10 == NULL
  [rdx] == NULL || rdx == NULL

0xe6b99 execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL

0x10afa9 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xe6b69 :
	<Bool reg_rdx_13423_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_13425_64{UNINITIALIZED} == 0x2>
	<Bool reg_rax_13427_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13422_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_r10_13422_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6b93 :
	<Bool reg_rbp_12618_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_12617_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_12617_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0xe6b96 :
	<Bool reg_rbp_12623_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_12622_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_12622_64{UNINITIALIZED} == 0xffffffc000000000>
libc_base + 0xe696a :
	<Bool reg_rdx_12690_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12692_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_12689_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_12689_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0x10afb5 :
	<Bool reg_rax_12906_64{UNINITIALIZED} == 0xffffffff00000000>
	<Bool True>
	<Bool reg_rsi_12908_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_12908_64{UNINITIALIZED} == 0x1>
libc_base + 0x10afbc :
	<Bool reg_rax_12911_64{UNINITIALIZED} == 0xfffffffff0000000>
	<Bool True>
	<Bool reg_rsi_12913_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_12913_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0xe6b66 :
	<Bool reg_r10_13411_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_13413_64{UNINITIALIZED} == 0x67>
	<Bool reg_rax_13415_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r10_13411_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe6b6d :
	<Bool reg_rdx_13435_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_13437_64{UNINITIALIZED} == 0x67>
	<Bool reg_rax_13439_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13440_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b71 :
	<Bool reg_rdx_13448_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_13450_64{UNINITIALIZED} == 0x66>
	<Bool reg_rax_13452_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13453_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b79 :
	<Bool reg_rbp_13462_64{UNINITIALIZED} == 0x1>
	<Bool reg_rdx_13464_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13465_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13466_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b7d :
	<Bool reg_rdx_13475_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13477_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13478_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13480_64{UNINITIALIZED} == 0x77>
libc_base + 0xe696e :
	<Bool reg_rdx_12698_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12701_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_12699_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6972 :
	<Bool reg_rdx_12708_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12710_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_12707_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6975 :
	<Bool reg_rdx_12756_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12758_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12759_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe697c :
	<Bool reg_rdx_12766_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12769_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12770_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6984 :
	<Bool reg_rdx_12777_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_12779_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12780_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x10afb0 :
	<Bool True>
	<Bool reg_rax_12896_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_12896_64{UNINITIALIZED} == 0xfffffffc00000000>
libc_base + 0x10afbf :
	<Bool True>
	<Bool reg_rsi_12917_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_12917_64{UNINITIALIZED} == 0xfe00000000000000>
libc_base + 0xe699e :
	<Bool True>
	<Bool reg_r15_13294_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_13294_64{UNINITIALIZED} == 0xffffffffffffffc0>
libc_base + 0xe69a1 :
	<Bool True>
	<Bool reg_r15_13297_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_13297_64{UNINITIALIZED} == 0x1>
libc_base + 0xe6b85 :
	<Bool reg_rax_13489_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13490_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13492_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6b89 :
	<Bool !(reg_cc_dep1_13501_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_13504_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13506_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c09 :
	<Bool reg_rbp_12431_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_12431_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe6c0d :
	<Bool reg_rbp_12436_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_12436_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c10 :
	<Bool reg_rbp_12440_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_12440_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c14 :
	<Bool reg_rbp_12444_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_12446_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b8b :
	<Bool reg_r10_12610_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12612_64{UNINITIALIZED} == 0x77>
libc_base + 0xe698c :
	<Bool reg_rax_12787_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12788_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6990 :
	<Bool !(reg_cc_dep1_12795_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_12798_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c4e :
	<Bool reg_rbp_14488_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14488_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c51 :
	<Bool reg_rbp_14493_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14493_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c55 :
	<Bool reg_rbp_14499_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_14502_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c59 :
	<Bool reg_rbp_14507_64{UNINITIALIZED} == 0x42>
	<Bool reg_r10_14509_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c5d :
	<Bool reg_rbp_14514_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_14516_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c61 :
	<Bool reg_r10_14521_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14523_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c18 :
	<Bool reg_r15_12450_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6996 :
	<Bool reg_r15_13289_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x10afa9 :
```
