# libc6_2.31-0ubuntu9.2_amd64
Ubuntu GLIBC 2.31-0ubuntu9.2

```
MD5: d371da546786965fe0ee40147ffef716
SHA1: a1ca4cd2d1df2fcd2c0f582665051c261d84c1d6
```

```
0xe6c4a, 0xe6c4e, 0xe6c52, 0xe6c55, 0xe6c5c, 0xe6c64, 0xe6c6c, 0xe6c70, 0xe6c76, 0xe6c7e, 0xe6c81, 0xe6e46, 0xe6e49, 0xe6e4d, 0xe6e51, 0xe6e59, 0xe6e5d, 0xe6e65, 0xe6e69, 0xe6e6b, 0xe6e73, 0xe6e73, 0xe6e76, 0xe6e76, 0xe6e79, 0xe6ee9, 0xe6eed, 0xe6ef0, 0xe6ef4, 0xe6ef8, 0xe6f2e, 0xe6f31, 0xe6f35, 0xe6f39, 0xe6f3d, 0xe6f41
```

## one_gadget
```
0xe6e73 execve("/bin/sh", r10, r12)
constraints:
  [r10] == NULL || r10 == NULL
  [r12] == NULL || r12 == NULL

0xe6e76 execve("/bin/sh", r10, rdx)
constraints:
  [r10] == NULL || r10 == NULL
  [rdx] == NULL || rdx == NULL

0xe6e79 execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL
```

## angry_gadget
```
libc_base + 0xe6e49 :
	<Bool reg_rdx_14137_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14139_64{UNINITIALIZED} == 0x66>
	<Bool reg_rax_14141_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14136_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_r10_14136_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6e73 :
	<Bool reg_rbp_13711_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_13710_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_13710_64{UNINITIALIZED} == 0xfffffffffffe0000>
libc_base + 0xe6e76 :
	<Bool reg_rbp_13716_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_13715_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_13715_64{UNINITIALIZED} == 0xfffffffc00000000>
libc_base + 0xe6c4a :
	<Bool reg_rdx_13783_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13785_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13782_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_13782_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6e46 :
	<Bool reg_r10_14125_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14127_64{UNINITIALIZED} == 0x62>
	<Bool reg_rax_14129_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r10_14125_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe6e4d :
	<Bool reg_rdx_14149_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14151_64{UNINITIALIZED} == 0x67>
	<Bool reg_rax_14153_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14154_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e51 :
	<Bool reg_rdx_14162_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_14164_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_14166_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14167_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e59 :
	<Bool reg_rbp_14176_64{UNINITIALIZED} == 0x62>
	<Bool reg_rdx_14178_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14179_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14180_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e5d :
	<Bool reg_rdx_14189_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14191_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14192_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14194_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c4e :
	<Bool reg_rdx_13791_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13794_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13792_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c52 :
	<Bool reg_rdx_13801_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13803_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13800_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c55 :
	<Bool reg_rdx_13849_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13851_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13852_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c5c :
	<Bool reg_rdx_13859_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13862_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13863_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c64 :
	<Bool reg_rdx_13870_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13872_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13873_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e65 :
	<Bool reg_rax_14203_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14204_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14206_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6e69 :
	<Bool !(reg_cc_dep1_14215_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_14218_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14220_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c7e :
	<Bool True>
	<Bool reg_r15_14677_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14677_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xe6c81 :
	<Bool True>
	<Bool reg_r15_14680_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14680_64{UNINITIALIZED} == 0xffe0000000000000>
libc_base + 0xe6e6b :
	<Bool reg_r10_13703_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13705_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c6c :
	<Bool reg_rax_13880_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13881_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c70 :
	<Bool !(reg_cc_dep1_13888_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_13891_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ee9 :
	<Bool reg_rbp_14047_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_14047_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe6eed :
	<Bool reg_rbp_14052_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14052_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6ef0 :
	<Bool reg_rbp_14056_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14056_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6ef4 :
	<Bool reg_rbp_14060_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_14062_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f2e :
	<Bool reg_rbp_14590_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14590_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6f31 :
	<Bool reg_rbp_14595_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14595_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6f35 :
	<Bool reg_rbp_14601_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_14604_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f39 :
	<Bool reg_rbp_14609_64{UNINITIALIZED} == 0x2>
	<Bool reg_r10_14611_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f3d :
	<Bool reg_rbp_14616_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_14618_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f41 :
	<Bool reg_r10_14623_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14625_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6ef8 :
	<Bool reg_r15_14066_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c76 :
	<Bool reg_r15_14672_64{UNINITIALIZED} == 0xffffffffffffffef>
```
