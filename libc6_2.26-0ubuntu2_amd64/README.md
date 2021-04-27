# libc6_2.26-0ubuntu2_amd64
Ubuntu GLIBC 2.26-0ubuntu2

```
MD5: 0afff217261aae2d6421b84ef13a220f
SHA1: 08d7e3b1a7a983fdb893b11943c9e3884e59e887
```

```
0x47c46, 0x47c9a, 0x47c9a, 0x47ca1, 0x47ca8, 0x47cad, 0x47cb7, 0x47cc1, 0x47cc4, 0xd9703, 0xd970a, 0xd970d, 0xd9710, 0xd9827, 0xd982a, 0xd982e, 0xd9836, 0xd983a, 0xd983e, 0xd99d8, 0xd99dc, 0xd99e3, 0xd99e6, 0xd99fc, 0xd9a03, 0xd9a0a, 0xd9a12, 0xd9a19, 0xd9a1d, 0xd9a21, 0xd9a25, 0xfcc6e, 0xfcc6e, 0xfcc75, 0xfcc7a, 0xfcc81, 0xfcc84, 0xfdb1e, 0xfdb1e, 0xfdb25, 0xfdb2a, 0xfdb31, 0xfdb34
```

## one_gadget
```
0x47c46 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x47c9a execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xfcc6e execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0xfdb1e execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xd983a :
	<Bool reg_rbp_109120_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_r13_109123_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109123_64{UNINITIALIZED} == 0xffffffffffffe000>
libc_base + 0xfcc7a :
	<Bool reg_rax_109754_64{UNINITIALIZED} == 0xffffffffc0000000>
	<Bool True>
	<Bool reg_rsi_109756_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109756_64{UNINITIALIZED} == 0xfff0000000000000>
libc_base + 0xfcc81 :
	<Bool reg_rax_109759_64{UNINITIALIZED} == 0x8000000000000000>
	<Bool True>
	<Bool reg_rsi_109761_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109761_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xd99fc :
	<Bool reg_rbp_109987_64{UNINITIALIZED} == 0x97>
	<Bool True>
	<Bool mem_7_109988_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_7_109988_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0xd9a03 :
	<Bool reg_rbp_109993_64{UNINITIALIZED} == 0x97>
	<Bool True>
	<Bool mem_7_109994_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_7_109994_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xd9a0a :
	<Bool reg_rbp_110000_64{UNINITIALIZED} == 0x3f>
	<Bool True>
	<Bool mem_ffffffffffffffaf_110001_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_ffffffffffffffaf_110001_64{UNINITIALIZED} == 0xffffffffff000000>
libc_base + 0xd9a12 :
	<Bool reg_rbp_110007_64{UNINITIALIZED} == 0x8a>
	<Bool True>
	<Bool mem_fffffffffffffffa_110008_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool mem_fffffffffffffffa_110008_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xd9a19 :
	<Bool reg_rbp_110014_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_rcx_110018_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110018_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xd9a1d :
	<Bool reg_rbp_110021_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_rcx_110024_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110024_64{UNINITIALIZED} == 0xffffffc000000000>
libc_base + 0xd9a21 :
	<Bool reg_rbp_110027_64{UNINITIALIZED} == 0x47>
	<Bool True>
	<Bool reg_rcx_110030_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110030_64{UNINITIALIZED} == 0xffffffffc0000000>
libc_base + 0xd9a25 :
	<Bool reg_rbp_110033_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_rcx_110035_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110035_64{UNINITIALIZED} == 0xfffffffc00000000>
libc_base + 0x47cad :
	<Bool reg_rax_110154_64{UNINITIALIZED} == 0xffffffffe0000000>
	<Bool True>
	<Bool reg_rsi_110156_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110156_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0x47cb7 :
	<Bool reg_rax_110160_64{UNINITIALIZED} == 0xfffff00000000000>
	<Bool True>
	<Bool reg_rsi_110162_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110162_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0x47cc1 :
	<Bool reg_rax_110166_64{UNINITIALIZED} == 0xff80000000000000>
	<Bool True>
	<Bool reg_rsi_110168_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110168_64{UNINITIALIZED} == 0x8000000000000000>
libc_base + 0xfdb2a :
	<Bool reg_rax_110223_64{UNINITIALIZED} == 0xffffffffff000000>
	<Bool True>
	<Bool reg_rsi_110225_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110225_64{UNINITIALIZED} == 0xffffffffffff0000>
libc_base + 0xfdb31 :
	<Bool reg_rax_110228_64{UNINITIALIZED} == 0xffffffffffff8000>
	<Bool True>
	<Bool reg_rsi_110230_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110230_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xd99d8 :
	<Bool reg_rbp_110465_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_rcx_110467_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110467_64{UNINITIALIZED} == 0xfffff00000000000>
libc_base + 0xd9703 :
	<Bool True>
	<Bool reg_r13_108852_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_108852_64{UNINITIALIZED} == 0xffffffffffff8000>
libc_base + 0xd970a :
	<Bool True>
	<Bool reg_r13_108856_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_108856_64{UNINITIALIZED} == 0xffffffffffffe000>
libc_base + 0xd970d :
	<Bool True>
	<Bool reg_r13_108860_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_108860_64{UNINITIALIZED} == 0xfffffffff0000000>
libc_base + 0xd9710 :
	<Bool True>
	<Bool reg_rsi_108865_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108865_64{UNINITIALIZED} == 0xffff000000000000>
libc_base + 0xd983e :
	<Bool True>
	<Bool reg_r13_109127_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r13_109127_64{UNINITIALIZED} == 0xffffffffffffff80>
libc_base + 0xfcc75 :
	<Bool True>
	<Bool reg_rax_109744_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109744_64{UNINITIALIZED} == 0xfffffffffffffff8>
libc_base + 0xfcc84 :
	<Bool True>
	<Bool reg_rsi_109765_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109765_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0x47ca1 :
	<Bool True>
	<Bool reg_rax_110145_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_110145_64{UNINITIALIZED} == 0xffffffffff000000>
libc_base + 0x47ca8 :
	<Bool True>
	<Bool reg_rax_110149_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_110149_64{UNINITIALIZED} == 0xfffffffffff00000>
libc_base + 0x47cc4 :
	<Bool True>
	<Bool reg_rsi_110172_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110172_64{UNINITIALIZED} == 0xfff0000000000000>
libc_base + 0xfdb25 :
	<Bool True>
	<Bool reg_rax_110213_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_110213_64{UNINITIALIZED} == 0xffffffffffffe000>
libc_base + 0xfdb34 :
	<Bool True>
	<Bool reg_rsi_110234_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110234_64{UNINITIALIZED} == 0x1>
libc_base + 0xd99dc :
	<Bool True>
	<Bool reg_rcx_110475_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110475_64{UNINITIALIZED} == 0xfffffffffc000000>
libc_base + 0xd99e3 :
	<Bool True>
	<Bool reg_rcx_110479_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_110479_64{UNINITIALIZED} == 0xffffff8000000000>
libc_base + 0xd99e6 :
	<Bool True>
	<Bool reg_rsi_110484_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110484_64{UNINITIALIZED} == 0xffffffffffffff80>
libc_base + 0xd9827 :
	<Bool reg_rbp_109102_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_109102_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xd982a :
	<Bool reg_rbp_109107_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_109107_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xd982e :
	<Bool reg_rbp_109112_64{UNINITIALIZED} == 0x3f>
	<Bool 0xffffffffffffffb0 + reg_rbp_109112_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xd9836 :
	<Bool reg_rbp_109116_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_109116_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xfcc6e :
libc_base + 0x47c9a :
libc_base + 0xfdb1e :
```
