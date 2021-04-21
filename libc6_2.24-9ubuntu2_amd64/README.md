# libc6_2.24-9ubuntu2_amd64
Ubuntu GLIBC 2.24-9ubuntu2

```
MD5: ace8ff055ecdbb88032cd5acbea0b6a8
SHA1: efc93447524dd116fe95e3c353c6146da963983a
```

## one_gadget
```
0x45526 execve("/bin/sh", rsp+0x30, environ)
constraints:
  rax == NULL

0x4557a execve("/bin/sh", rsp+0x30, environ)
constraints:
  [rsp+0x30] == NULL

0xf0a51 execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0xf18cb execve("/bin/sh", rsp+0x60, environ)
constraints:
  [rsp+0x60] == NULL
```

## angry_gadget
```
libc_base + 0xcd4c6 :
	<Bool reg_rax_110153_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_110155_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_110161_64{UNINITIALIZED} == 0x4f>
	<Bool True>
	<Bool reg_r9_110163_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_110163_64{UNINITIALIZED} == 0xffffc00000000000>
libc_base + 0xcd4ce :
	<Bool !(reg_cc_dep1_110176_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rax_110179_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool reg_rbp_110183_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_r9_110185_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_110185_64{UNINITIALIZED} == 0xfffffffc00000000>
libc_base + 0xcd21d :
	<Bool reg_rax_109602_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_109605_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_109611_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109611_64{UNINITIALIZED} == 0xffffffffffffc000>
libc_base + 0xcd225 :
	<Bool reg_rax_109623_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_109625_64{UNINITIALIZED}[6:6] == 0)>
	<Bool True>
	<Bool reg_r15_109631_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109631_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xcd22d :
	<Bool !(reg_cc_dep1_109644_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rax_109647_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffd>
	<Bool True>
	<Bool reg_r15_109651_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109651_64{UNINITIALIZED} == 0xfffff00000000000>
libc_base + 0x4558d :
	<Bool reg_rax_108283_64{UNINITIALIZED} == 0xffffffc000000000>
	<Bool True>
	<Bool reg_rsi_108285_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108285_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0x45597 :
	<Bool reg_rax_108289_64{UNINITIALIZED} == 0xffffffffffffffc0>
	<Bool True>
	<Bool reg_rsi_108291_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108291_64{UNINITIALIZED} == 0x2>
libc_base + 0x455a1 :
	<Bool reg_rax_108295_64{UNINITIALIZED} == 0xfffffffffff00000>
	<Bool True>
	<Bool reg_rsi_108297_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108297_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xf0a5d :
	<Bool reg_rax_109170_64{UNINITIALIZED} == 0xfe00000000000000>
	<Bool True>
	<Bool reg_rsi_109172_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109172_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0xf0a64 :
	<Bool reg_rax_109175_64{UNINITIALIZED} == 0xfffffff800000000>
	<Bool True>
	<Bool reg_rsi_109177_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109177_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0xcd4e5 :
	<Bool reg_rbp_109362_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_r9_109364_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109364_64{UNINITIALIZED} == 0xffffffffffffc000>
libc_base + 0xcd49e :
	<Bool reg_rax_110033_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_110036_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rsi_110034_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_110033_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4a2 :
	<Bool reg_rax_110046_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_110049_64{UNINITIALIZED} == 0x37>
	<Bool reg_rsi_110047_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_110046_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4aa :
	<Bool reg_rax_110074_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_110077_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rsi_110075_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_110074_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4ae :
	<Bool reg_rax_110090_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_110092_64{UNINITIALIZED} == 0x1a>
	<Bool reg_rsi_110089_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_110090_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4b2 :
	<Bool reg_rax_110105_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_110107_64{UNINITIALIZED} == 0x32>
	<Bool !(reg_cc_dep1_110109_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_110105_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd4ba :
	<Bool reg_rbp_110121_64{UNINITIALIZED} == 0x2a>
	<Bool reg_rax_110123_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_110124_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_110123_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xcd4be :
	<Bool reg_rax_110136_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_110138_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_110143_64{UNINITIALIZED} == 0x4e>
	<Bool (reg_rax_110136_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xf18d7 :
	<Bool reg_rax_110205_64{UNINITIALIZED} == 0xffffffffffffe000>
	<Bool True>
	<Bool reg_rsi_110207_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110207_64{UNINITIALIZED} == 0xfffffffffe000000>
libc_base + 0xf18de :
	<Bool reg_rax_110210_64{UNINITIALIZED} == 0xfffffffffc000000>
	<Bool True>
	<Bool reg_rsi_110212_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110212_64{UNINITIALIZED} == 0xffffff8000000000>
libc_base + 0x45581 :
	<Bool True>
	<Bool reg_rax_108274_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108274_64{UNINITIALIZED} == 0xffc0000000000000>
libc_base + 0x45588 :
	<Bool True>
	<Bool reg_rax_108278_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_108278_64{UNINITIALIZED} == 0xfffffe0000000000>
libc_base + 0x455a4 :
	<Bool True>
	<Bool reg_rsi_108301_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_108301_64{UNINITIALIZED} == 0xfff8000000000000>
libc_base + 0xf0a58 :
	<Bool True>
	<Bool reg_rax_109160_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_109160_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0xf0a67 :
	<Bool True>
	<Bool reg_rsi_109181_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109181_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xcd4e9 :
	<Bool True>
	<Bool reg_r9_109372_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109372_64{UNINITIALIZED} == 0xffffe00000000000>
libc_base + 0xcd4f0 :
	<Bool True>
	<Bool reg_r9_109376_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r9_109376_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xcd4f3 :
	<Bool True>
	<Bool reg_rsi_109381_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109381_64{UNINITIALIZED} == 0xfffc000000000000>
libc_base + 0xcd201 :
	<Bool reg_rax_109515_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rcx_109516_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_109515_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd205 :
	<Bool reg_rax_109526_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rcx_109527_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_109526_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd20d :
	<Bool reg_rax_109555_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rcx_109556_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_109555_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd211 :
	<Bool reg_rax_109571_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rcx_109570_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_109571_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd215 :
	<Bool reg_rax_109584_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_109587_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_109584_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xcd241 :
	<Bool True>
	<Bool reg_r15_109664_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109664_64{UNINITIALIZED} == 0xffff800000000000>
libc_base + 0xcd248 :
	<Bool True>
	<Bool reg_r15_109668_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109668_64{UNINITIALIZED} == 0xfffffffff0000000>
libc_base + 0xcd24b :
	<Bool True>
	<Bool reg_r15_109672_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_109672_64{UNINITIALIZED} == 0xfffffffffffffe00>
libc_base + 0xcd24e :
	<Bool True>
	<Bool reg_rsi_109677_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_109677_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0xcd4a5 :
	<Bool reg_rbp_110061_64{UNINITIALIZED} == 0x1>
	<Bool reg_rsi_110059_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_110061_64{UNINITIALIZED} + 0xffffffffffffffb0 == 0xffffffffffffffb1>
libc_base + 0xf18d2 :
	<Bool True>
	<Bool reg_rax_110195_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_110195_64{UNINITIALIZED} == 0xfffffe0000000000>
libc_base + 0xf18e1 :
	<Bool True>
	<Bool reg_rsi_110216_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_110216_64{UNINITIALIZED} == 0xffffe00000000000>
libc_base + 0xcd208 :
	<Bool reg_rcx_109540_64{UNINITIALIZED} == 0x1>
libc_base + 0x4557a :
libc_base + 0xf0a51 :
libc_base + 0xf18cb :
```
