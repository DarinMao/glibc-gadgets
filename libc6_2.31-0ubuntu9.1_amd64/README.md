# libc6_2.31-0ubuntu9.1_amd64
Ubuntu GLIBC 2.31-0ubuntu9.1

```
MD5: 1ec728d58f7fc0d302119e9bb53050f8
SHA1: 4fcd76645607f38d91f65654ddd6b9770b5ea54a
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
	<Bool reg_rdx_14017_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14019_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_14021_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14016_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_r10_14016_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6e46 :
	<Bool reg_r10_14005_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14007_64{UNINITIALIZED} == 0x67>
	<Bool reg_rax_14009_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r10_14005_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe6e4d :
	<Bool reg_rdx_14029_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_14031_64{UNINITIALIZED} == 0x66>
	<Bool reg_rax_14033_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14034_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e51 :
	<Bool reg_rdx_14043_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_14045_64{UNINITIALIZED} == 0x2>
	<Bool reg_rax_14047_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14048_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e59 :
	<Bool reg_rbp_14057_64{UNINITIALIZED} == 0x66>
	<Bool reg_rdx_14059_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14060_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14061_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6e5d :
	<Bool reg_rdx_14070_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14072_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14073_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14075_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6e73 :
	<Bool reg_rbp_14654_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_14653_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_14653_64{UNINITIALIZED} == 0xffffffffffffe000>
libc_base + 0xe6e76 :
	<Bool reg_rbp_14659_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_14658_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_14658_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xe6c4a :
	<Bool reg_rdx_14726_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14728_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14725_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_14725_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6e65 :
	<Bool reg_rax_14084_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14085_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14087_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6e69 :
	<Bool !(reg_cc_dep1_14096_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_14099_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14101_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c7e :
	<Bool True>
	<Bool reg_r15_14607_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14607_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xe6c81 :
	<Bool True>
	<Bool reg_r15_14610_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14610_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xe6c4e :
	<Bool reg_rdx_14734_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14737_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14735_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c52 :
	<Bool reg_rdx_14744_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14746_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14743_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c55 :
	<Bool reg_rdx_14792_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14794_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14795_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c5c :
	<Bool reg_rdx_14802_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14805_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14806_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c64 :
	<Bool reg_rdx_14813_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14815_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14816_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ee9 :
	<Bool reg_rbp_13927_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_13927_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe6eed :
	<Bool reg_rbp_13932_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13932_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6ef0 :
	<Bool reg_rbp_13936_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13936_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6ef4 :
	<Bool reg_rbp_13940_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_13942_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f2e :
	<Bool reg_rbp_14238_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14238_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6f31 :
	<Bool reg_rbp_14243_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14243_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6f35 :
	<Bool reg_rbp_14249_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_14252_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f39 :
	<Bool reg_rbp_14257_64{UNINITIALIZED} == 0x66>
	<Bool reg_r10_14259_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f3d :
	<Bool reg_rbp_14264_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_14266_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6f41 :
	<Bool reg_r10_14271_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14273_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6e6b :
	<Bool reg_r10_14646_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14648_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c6c :
	<Bool reg_rax_14823_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14824_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c70 :
	<Bool !(reg_cc_dep1_14831_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_14834_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6ef8 :
	<Bool reg_r15_13946_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c76 :
	<Bool reg_r15_14602_64{UNINITIALIZED} == 0xffffffffffffffef>
```
