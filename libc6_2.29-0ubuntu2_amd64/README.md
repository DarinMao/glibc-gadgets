# libc6_2.29-0ubuntu2_amd64
Ubuntu GLIBC 2.29-0ubuntu2

```
MD5: 2fb0d6800d4d79ffdc7a388d7fe6aea0
SHA1: 9bb401974abeef59efcdd0ae35c5fc0ce63d3e7b
```

```
0x106ef8, 0x106ef8, 0x106eff, 0x106f04, 0x106f0b, 0x106f0e, 0xe2194, 0xe2198, 0xe219b, 0xe21a0, 0xe21a4, 0xe21ac, 0xe21b4, 0xe21bc, 0xe21c0, 0xe21c6, 0xe21ce, 0xe21d1, 0xe2345, 0xe2349, 0xe234c, 0xe2351, 0xe2355, 0xe235d, 0xe2361, 0xe2369, 0xe2371, 0xe2375, 0xe2377, 0xe237f, 0xe237f, 0xe2383, 0xe2383, 0xe2386, 0xe23d2, 0xe23d5, 0xe23d9, 0xe23dd, 0xe23e1, 0xe240c, 0xe2413, 0xe2417, 0xe241b, 0xe241f, 0xe2423, 0xe2427
```

## one_gadget
```
0xe237f execve("/bin/sh", rcx, [rbp-0x70])
constraints:
  [rcx] == NULL || rcx == NULL
  [[rbp-0x70]] == NULL || [rbp-0x70] == NULL

0xe2383 execve("/bin/sh", rcx, rdx)
constraints:
  [rcx] == NULL || rcx == NULL
  [rdx] == NULL || rdx == NULL

0xe2386 execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL

0x106ef8 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xe2345 :
	<Bool reg_rcx_37287_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_37289_64{UNINITIALIZED} == 0x2>
	<Bool reg_rax_37291_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_37287_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe2349 :
	<Bool reg_rcx_37296_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_37298_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_37300_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_37296_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe2351 :
	<Bool reg_rsi_37313_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_37315_64{UNINITIALIZED} == 0x4>
	<Bool reg_rax_37317_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_37313_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe2355 :
	<Bool reg_rsi_37322_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_37324_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_37326_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_37322_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe235d :
	<Bool reg_rbp_37331_64{UNINITIALIZED} == 0x44>
	<Bool reg_rsi_37333_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_37334_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rsi_37333_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe2361 :
	<Bool reg_rsi_37340_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_37342_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_37343_64{UNINITIALIZED} == 0x2>
	<Bool (reg_rsi_37340_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe2369 :
	<Bool reg_rsi_37350_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_37352_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_37353_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_37354_64{UNINITIALIZED} == 0x6f>
libc_base + 0x106f04 :
	<Bool reg_rax_37912_64{UNINITIALIZED} == 0xfffffffe00000000>
	<Bool True>
	<Bool reg_rsi_37914_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_37914_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0x106f0b :
	<Bool reg_rax_37917_64{UNINITIALIZED} == 0xf000000000000000>
	<Bool True>
	<Bool reg_rsi_37919_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_37919_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xe237f :
	<Bool reg_rbp_38133_64{UNINITIALIZED} == 0x6e>
	<Bool True>
	<Bool reg_rcx_38135_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_38135_64{UNINITIALIZED} == 0xff00000000000000>
libc_base + 0xe21ce :
	<Bool True>
	<Bool reg_r15_37177_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_37177_64{UNINITIALIZED} == 0xffe0000000000000>
libc_base + 0xe21d1 :
	<Bool True>
	<Bool reg_r15_37180_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_37180_64{UNINITIALIZED} == 0xffe0000000000000>
libc_base + 0xe234c :
	<Bool reg_rbp_37306_64{UNINITIALIZED} == 0x54>
	<Bool reg_rax_37308_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_37306_64{UNINITIALIZED} + 0xffffffffffffff90 == 0xffffffffffffffe4>
libc_base + 0xe2371 :
	<Bool reg_rax_37361_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_37362_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_37363_64{UNINITIALIZED} == 0x2>
libc_base + 0xe2375 :
	<Bool !(reg_cc_dep1_37371_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rcx_37374_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_37375_64{UNINITIALIZED} == 0x42>
libc_base + 0x106eff :
	<Bool True>
	<Bool reg_rax_37902_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_37902_64{UNINITIALIZED} == 0xe000000000000000>
libc_base + 0x106f0e :
	<Bool True>
	<Bool reg_rsi_37923_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_37923_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xe2194 :
	<Bool reg_rcx_38050_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rax_38053_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_38050_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe2198 :
	<Bool reg_rcx_38058_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rax_38061_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_38058_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe21a0 :
	<Bool reg_rcx_38073_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_38076_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_38073_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe21a4 :
	<Bool reg_rcx_38081_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_38084_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_38081_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe21ac :
	<Bool reg_rcx_38089_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_38092_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_38093_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe21b4 :
	<Bool reg_rcx_38100_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_38102_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_38103_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe2383 :
	<Bool True>
	<Bool reg_rcx_38138_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rcx_38138_64{UNINITIALIZED} == 0xffffffffffffffc0>
libc_base + 0xe240c :
	<Bool reg_rbp_37085_64{UNINITIALIZED} == 0x7f>
	<Bool mem_7_37086_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe2413 :
	<Bool reg_rbp_37091_64{UNINITIALIZED} == 0x7f>
	<Bool mem_7_37092_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe2417 :
	<Bool reg_rbp_37098_64{UNINITIALIZED} == 0x72>
	<Bool mem_fffffffffffffffa_37099_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe241b :
	<Bool reg_rbp_37105_64{UNINITIALIZED} == 0x4f>
	<Bool reg_rcx_37108_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe241f :
	<Bool reg_rbp_37112_64{UNINITIALIZED} == 0x56>
	<Bool reg_rcx_37114_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe2423 :
	<Bool reg_rbp_37118_64{UNINITIALIZED} == 0x47>
	<Bool reg_rcx_37120_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe2427 :
	<Bool reg_rcx_37124_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_37125_64{UNINITIALIZED} == 0x42>
libc_base + 0xe21bc :
	<Bool reg_rax_38110_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_38111_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe21c0 :
	<Bool !(reg_cc_dep1_38118_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_38121_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe2377 :
	<Bool reg_rcx_38128_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_38129_64{UNINITIALIZED} == 0x1>
libc_base + 0xe23d2 :
	<Bool reg_rbp_38211_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_38211_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe23d5 :
	<Bool reg_rbp_38216_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_38216_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe23d9 :
	<Bool reg_rbp_38221_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_38221_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe23dd :
	<Bool reg_rbp_38225_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_38227_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe21c6 :
	<Bool reg_r15_37172_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe219b :
	<Bool reg_rax_38068_64{UNINITIALIZED} == 0x1>
libc_base + 0xe23e1 :
	<Bool reg_r15_38231_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x106ef8 :
```
