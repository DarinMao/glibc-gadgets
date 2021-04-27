# libc6_2.28-0ubuntu1_amd64
Ubuntu GLIBC 2.28-0ubuntu1

```
MD5: 9dc614ec33ee0284064ec5535bda431c
SHA1: 35bc971d85479d1f7ad5f48752302d9dd185f577
```

```
0x103f50, 0x103f50, 0x103f57, 0x103f5c, 0x103f63, 0x103f66, 0x50186, 0x501e3, 0x501e3, 0x501ea, 0x501ef, 0x501f6, 0x50200, 0x5020a, 0x5020d, 0xdf1b4, 0xdf1b8, 0xdf1bb, 0xdf1c0, 0xdf1c4, 0xdf1cc, 0xdf1d4, 0xdf1dc, 0xdf1e0, 0xdf1e6, 0xdf1ee, 0xdf1f1, 0xdf365, 0xdf369, 0xdf36c, 0xdf371, 0xdf375, 0xdf37d, 0xdf381, 0xdf389, 0xdf391, 0xdf395, 0xdf397, 0xdf39f, 0xdf3a3, 0xdf3f2, 0xdf3f5, 0xdf3f9, 0xdf3fd, 0xdf401, 0xdf42c, 0xdf433, 0xdf437, 0xdf43b, 0xdf43f, 0xdf443, 0xdf447
```

## one_gadget
```
0x50186 execve("/bin/sh", rsp+0x40, environ)
constraints:
  rsp & 0xf == 0
  rcx == NULL

0x501e3 execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0x103f50 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xdf365 :
	<Bool reg_rcx_34155_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_34157_64{UNINITIALIZED} == 0x54>
	<Bool reg_rax_34159_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_34155_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf369 :
	<Bool reg_rcx_34164_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_34166_64{UNINITIALIZED} == 0x54>
	<Bool reg_rax_34168_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_34164_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf371 :
	<Bool reg_rsi_34181_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_34183_64{UNINITIALIZED} == 0x56>
	<Bool reg_rax_34185_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_34181_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf375 :
	<Bool reg_rsi_34190_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_34192_64{UNINITIALIZED} == 0x44>
	<Bool reg_rax_34194_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_34190_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf37d :
	<Bool reg_rbp_34199_64{UNINITIALIZED} == 0x4>
	<Bool reg_rsi_34201_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_34202_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_34201_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xdf381 :
	<Bool reg_rsi_34208_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_34210_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_34211_64{UNINITIALIZED} == 0x6e>
	<Bool (reg_rsi_34208_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xdf389 :
	<Bool reg_rsi_34218_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_34220_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_34221_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_34222_64{UNINITIALIZED} == 0x1>
libc_base + 0x103f5c :
	<Bool reg_rax_35853_64{UNINITIALIZED} == 0xffc0000000000000>
	<Bool True>
	<Bool reg_rsi_35855_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_35855_64{UNINITIALIZED} == 0xffffffffffc00000>
libc_base + 0x103f63 :
	<Bool reg_rax_35858_64{UNINITIALIZED} == 0xffffc00000000000>
	<Bool True>
	<Bool reg_rsi_35860_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_35860_64{UNINITIALIZED} == 0xffffffffffff8000>
libc_base + 0xdf39f :
	<Bool reg_rbp_36021_64{UNINITIALIZED} == 0x62>
	<Bool True>
	<Bool reg_rcx_36023_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_36023_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0x501ef :
	<Bool reg_rax_36082_64{UNINITIALIZED} == 0xfffffffe00000000>
	<Bool True>
	<Bool reg_rsi_36084_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_36084_64{UNINITIALIZED} == 0xff80000000000000>
libc_base + 0x501f6 :
	<Bool reg_rax_36087_64{UNINITIALIZED} == 0xc000000000000000>
	<Bool True>
	<Bool reg_rsi_36089_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_36089_64{UNINITIALIZED} == 0xfffff00000000000>
libc_base + 0x50200 :
	<Bool reg_rax_36093_64{UNINITIALIZED} == 0xffffffffc0000000>
	<Bool True>
	<Bool reg_rsi_36095_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_36095_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0x5020a :
	<Bool reg_rax_36099_64{UNINITIALIZED} == 0xffffffc000000000>
	<Bool True>
	<Bool reg_rsi_36101_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_36101_64{UNINITIALIZED} == 0xfffe000000000000>
libc_base + 0xdf1ee :
	<Bool True>
	<Bool reg_r15_34076_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_34076_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf1f1 :
	<Bool True>
	<Bool reg_r15_34079_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_34079_64{UNINITIALIZED} == 0xff80000000000000>
libc_base + 0xdf36c :
	<Bool reg_rbp_34174_64{UNINITIALIZED} == 0x54>
	<Bool reg_rax_34176_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_34174_64{UNINITIALIZED} + 0xffffffffffffff90 == 0xffffffffffffffe4>
libc_base + 0xdf391 :
	<Bool reg_rax_34230_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_34231_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_34232_64{UNINITIALIZED} == 0x42>
libc_base + 0xdf395 :
	<Bool !(reg_cc_dep1_34240_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rcx_34243_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_34244_64{UNINITIALIZED} == 0x6a>
libc_base + 0xdf1b4 :
	<Bool reg_rcx_35763_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rax_35766_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_35763_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf1b8 :
	<Bool reg_rcx_35771_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rax_35774_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_35771_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf1c0 :
	<Bool reg_rcx_35786_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_35789_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_35786_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf1c4 :
	<Bool reg_rcx_35794_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_35797_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_35794_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf1cc :
	<Bool reg_rcx_35802_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_35805_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_35806_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf1d4 :
	<Bool reg_rcx_35813_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_35815_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_35816_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x103f57 :
	<Bool True>
	<Bool reg_rax_35843_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_35843_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0x103f66 :
	<Bool True>
	<Bool reg_rsi_35864_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_35864_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xdf3a3 :
	<Bool True>
	<Bool reg_rcx_36026_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_36026_64{UNINITIALIZED} == 0xfffffe0000000000>
libc_base + 0x501ea :
	<Bool True>
	<Bool reg_rax_36072_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_36072_64{UNINITIALIZED} == 0xfffffffc00000000>
libc_base + 0x5020d :
	<Bool True>
	<Bool reg_rsi_36105_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_36105_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0xdf1dc :
	<Bool reg_rax_35823_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_35824_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf1e0 :
	<Bool !(reg_cc_dep1_35831_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_35834_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf397 :
	<Bool reg_rcx_36016_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_36017_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf42c :
	<Bool reg_rbp_36144_64{UNINITIALIZED} == 0x7f>
	<Bool mem_7_36145_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf433 :
	<Bool reg_rbp_36150_64{UNINITIALIZED} == 0x7f>
	<Bool mem_7_36151_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf437 :
	<Bool reg_rbp_36157_64{UNINITIALIZED} == 0x2>
	<Bool mem_ffffffffffffff8a_36158_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf43b :
	<Bool reg_rbp_36164_64{UNINITIALIZED} == 0x4f>
	<Bool reg_rcx_36167_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf43f :
	<Bool reg_rbp_36171_64{UNINITIALIZED} == 0x56>
	<Bool reg_rcx_36173_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf443 :
	<Bool reg_rbp_36177_64{UNINITIALIZED} == 0x47>
	<Bool reg_rcx_36179_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf447 :
	<Bool reg_rcx_36183_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_36184_64{UNINITIALIZED} == 0x42>
libc_base + 0xdf3f2 :
	<Bool reg_rbp_36236_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_36236_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf3f5 :
	<Bool reg_rbp_36241_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_36241_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf3f9 :
	<Bool reg_rbp_36246_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_36246_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf3fd :
	<Bool reg_rbp_36250_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_36252_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf1e6 :
	<Bool reg_r15_34071_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf1bb :
	<Bool reg_rax_35781_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf401 :
	<Bool reg_r15_36256_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x103f50 :
libc_base + 0x501e3 :
```
