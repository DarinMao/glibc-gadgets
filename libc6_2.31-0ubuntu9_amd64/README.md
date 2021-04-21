# libc6_2.31-0ubuntu9_amd64
Ubuntu GLIBC 2.31-0ubuntu9

```
MD5: 10fdeb77eea525914332769e9cd912ae
SHA1: ed475285eed517355f0e6976502d15df2237fc6f
```

## one-gadget
```
0xe6ce3 execve("/bin/sh", r10, r12)
constraints:
  [r10] == NULL || r10 == NULL
  [r12] == NULL || r12 == NULL

0xe6ce6 execve("/bin/sh", r10, rdx)
constraints:
  [r10] == NULL || r10 == NULL
  [rdx] == NULL || rdx == NULL

0xe6ce9 execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL
```

## angry_gadget
```
libc_base + 0xe6cb9 :
	<Bool reg_rdx_14524_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14526_64{UNINITIALIZED} == 0x2>
	<Bool reg_rax_14528_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14523_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_r10_14523_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6ce3 :
	<Bool reg_rbp_14164_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_14163_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_14163_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xe6ce6 :
	<Bool reg_rbp_14169_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_14168_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_14168_64{UNINITIALIZED} == 0xfffffffffffffff8>
libc_base + 0xe6aba :
	<Bool reg_rdx_14236_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14238_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14235_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_14235_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6cb6 :
	<Bool reg_r10_14512_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14514_64{UNINITIALIZED} == 0x67>
	<Bool reg_rax_14516_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r10_14512_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe6cbd :
	<Bool reg_rdx_14536_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14538_64{UNINITIALIZED} == 0x42>
	<Bool reg_rax_14540_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14541_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6cc1 :
	<Bool reg_rdx_14550_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_14552_64{UNINITIALIZED} == 0x67>
	<Bool reg_rax_14554_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14555_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6cc9 :
	<Bool reg_rbp_14563_64{UNINITIALIZED} == 0x66>
	<Bool reg_rdx_14565_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14566_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14567_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ccd :
	<Bool reg_rdx_14576_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14578_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14579_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14581_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6abe :
	<Bool reg_rdx_14244_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14247_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14245_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ac2 :
	<Bool reg_rdx_14254_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14256_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14253_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ac5 :
	<Bool reg_rdx_14302_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14304_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14305_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6acc :
	<Bool reg_rdx_14312_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14315_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14316_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ad4 :
	<Bool reg_rdx_14323_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14325_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14326_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6aee :
	<Bool True>
	<Bool reg_r15_14445_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14445_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0xe6af1 :
	<Bool True>
	<Bool reg_r15_14448_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14448_64{UNINITIALIZED} == 0xffff000000000000>
libc_base + 0xe6cd5 :
	<Bool reg_rax_14590_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14591_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14593_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6cd9 :
	<Bool !(reg_cc_dep1_14602_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_14605_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14607_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6d9e :
	<Bool reg_rbp_13077_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13077_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6da1 :
	<Bool reg_rbp_13082_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13082_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6da5 :
	<Bool reg_rbp_13088_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_13091_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6da9 :
	<Bool reg_rbp_13096_64{UNINITIALIZED} == 0x66>
	<Bool reg_r10_13098_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6dad :
	<Bool reg_rbp_13103_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_13105_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6db1 :
	<Bool reg_r10_13110_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13112_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6d59 :
	<Bool reg_rbp_14056_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_14056_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe6d5d :
	<Bool reg_rbp_14061_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14061_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6d60 :
	<Bool reg_rbp_14065_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14065_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6d64 :
	<Bool reg_rbp_14069_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_14071_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6cdb :
	<Bool reg_r10_14156_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14158_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6adc :
	<Bool reg_rax_14333_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14334_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ae0 :
	<Bool !(reg_cc_dep1_14341_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_14344_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6d68 :
	<Bool reg_r15_14075_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ae6 :
	<Bool reg_r15_14440_64{UNINITIALIZED} == 0xffffffffffffffef>
```
