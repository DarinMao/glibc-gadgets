# libc6_2.23-0ubuntu11.2_amd64
Ubuntu GLIBC 2.23-0ubuntu11.2

```
MD5: fb1692c79359ae96029e590c23872ed5
SHA1: ae799c0d270a8152908e5882bde6424c6693f7a3
```

## one_gadget
```
0x45226 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x4527a execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xf0364 execve("/bin/sh", rsp+0x50, environ)
constraints:
  [rsp+0x50] == NULL

0xf1207 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xf6721 :
	<Bool reg_rbx_113434_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_113437_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113445_64{UNINITIALIZED} == 0xc2>
	<Bool True>
	<Bool reg_rcx_113447_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113447_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xf6729 :
	<Bool reg_rbx_113450_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_113452_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113460_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_rcx_113462_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113462_64{UNINITIALIZED} == 0xffffffff80000000>
libc_base + 0xf6371 :
	<Bool reg_r12_113771_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_113773_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113776_64{UNINITIALIZED} == 0xda>
	<Bool True>
	<Bool reg_r13_113778_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_113778_64{UNINITIALIZED} == 0xfffffffffffe0000>
libc_base + 0xf6731 :
	<Bool !(reg_cc_dep1_113465_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113473_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_rcx_113475_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113475_64{UNINITIALIZED} == 0xfffffffffffffe00>
libc_base + 0xf6379 :
	<Bool !(reg_cc_dep1_113788_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113791_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_r13_113793_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_113793_64{UNINITIALIZED} == 0xffffe00000000000>
libc_base + 0xf67b0 :
	<Bool reg_rbp_112763_64{UNINITIALIZED} == 0xf2>
	<Bool True>
	<Bool reg_rcx_112765_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_112765_64{UNINITIALIZED} == 0xfff0000000000000>
libc_base + 0xf67b7 :
	<Bool reg_rbp_112768_64{UNINITIALIZED} == 0xf6>
	<Bool True>
	<Bool reg_rcx_112770_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_112770_64{UNINITIALIZED} == 0xffffffffffc00000>
libc_base + 0xf0370 :
	<Bool reg_rax_113031_64{UNINITIALIZED} == 0xfffffffffffc0000>
	<Bool True>
	<Bool reg_rsi_113033_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113033_64{UNINITIALIZED} == 0xfffffe0000000000>
libc_base + 0xf0377 :
	<Bool reg_rax_113036_64{UNINITIALIZED} == 0xfffe000000000000>
	<Bool True>
	<Bool reg_rsi_113038_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113038_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xf1213 :
	<Bool reg_rax_113148_64{UNINITIALIZED} == 0xffffffff80000000>
	<Bool True>
	<Bool reg_rsi_113150_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113150_64{UNINITIALIZED} == 0xfe00000000000000>
libc_base + 0xf121a :
	<Bool reg_rax_113153_64{UNINITIALIZED} == 0xff00000000000000>
	<Bool True>
	<Bool reg_rsi_113155_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113155_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xf670a :
	<Bool reg_rsi_113382_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool True>
	<Bool reg_rbp_113388_64{UNINITIALIZED} + 0xffffffffffffff08 <= 0xffffffffffffffff>
	<Bool reg_rbp_113388_64{UNINITIALIZED} + 0xffffffffffffff08 == 0xffffffffffffffca>
libc_base + 0xf670f :
	<Bool reg_r8_113391_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rsi_113392_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool reg_rbp_113398_64{UNINITIALIZED} == 0x7a>
	<Bool (reg_r8_113391_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf6712 :
	<Bool reg_rbx_113401_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rsi_113402_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool reg_rbp_113408_64{UNINITIALIZED} == 0xf6>
	<Bool (reg_rbx_113401_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf6716 :
	<Bool reg_rbx_113412_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rsi_113411_64{UNINITIALIZED}[31:0] == 0x1>
	<Bool reg_rbp_113418_64{UNINITIALIZED} == 0x7a>
	<Bool (reg_rbx_113412_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xf6719 :
	<Bool reg_rbx_113421_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_113424_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_113431_64{UNINITIALIZED} == 0xf2>
	<Bool (reg_rbx_113421_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0x4528d :
	<Bool reg_rax_114242_64{UNINITIALIZED} == 0xffffffffffffff00>
	<Bool True>
	<Bool reg_rsi_114244_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114244_64{UNINITIALIZED} == 0xfe00000000000000>
libc_base + 0x45297 :
	<Bool reg_rax_114248_64{UNINITIALIZED} == 0xfffffffffffffc00>
	<Bool True>
	<Bool reg_rsi_114250_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114250_64{UNINITIALIZED} == 0xfffffffffffffff8>
libc_base + 0x452a1 :
	<Bool reg_rax_114254_64{UNINITIALIZED} == 0xfffffffff8000000>
	<Bool True>
	<Bool reg_rsi_114256_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114256_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xf036b :
	<Bool True>
	<Bool reg_rax_113021_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113021_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xf037a :
	<Bool True>
	<Bool reg_rsi_113042_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113042_64{UNINITIALIZED} == 0x8000000000000000>
libc_base + 0xcd173 :
	<Bool True>
	<Bool reg_rcx_113092_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113092_64{UNINITIALIZED} == 0xfe00000000000000>
libc_base + 0xcd17a :
	<Bool True>
	<Bool reg_rcx_113096_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_113096_64{UNINITIALIZED} == 0xf000000000000000>
libc_base + 0xf120e :
	<Bool True>
	<Bool reg_rax_113138_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113138_64{UNINITIALIZED} == 0xfffffffffffffff0>
libc_base + 0xf121d :
	<Bool True>
	<Bool reg_rsi_113159_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113159_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xcd248 :
	<Bool True>
	<Bool reg_rax_113867_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113867_64{UNINITIALIZED} == 0xffffffffffff0000>
libc_base + 0xcd24f :
	<Bool True>
	<Bool reg_rax_113871_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_113871_64{UNINITIALIZED} == 0xffffc00000000000>
libc_base + 0xcd252 :
	<Bool True>
	<Bool reg_rsi_113877_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_113877_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0x45281 :
	<Bool True>
	<Bool reg_rax_114233_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_114233_64{UNINITIALIZED} == 0xffffffffffffffc0>
libc_base + 0x45288 :
	<Bool True>
	<Bool reg_rax_114237_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_114237_64{UNINITIALIZED} == 0xffffffffffffc000>
libc_base + 0x452a4 :
	<Bool True>
	<Bool reg_rsi_114260_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_114260_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0x6f5cb :
	<Bool reg_rsi_113508_64{UNINITIALIZED} == 0x0>
libc_base + 0x6f5ce :
	<Bool reg_rsi_113518_64{UNINITIALIZED} == 0x0>
libc_base + 0x6f5d1 :
	<Bool reg_rsi_113529_64{UNINITIALIZED} == 0x0>
libc_base + 0x6f5d3 :
	<Bool reg_rsi_113541_64{UNINITIALIZED} == 0x0>
libc_base + 0xf0364 :
libc_base + 0xf1207 :
libc_base + 0x4527a :
```
