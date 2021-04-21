# libc6_2.32-0ubuntu3.1_amd64
2.32-0ubuntu3.1

```
MD5: 7469ffc73a653e9eaae96cabab1f9260
SHA1: c7e72ea920cdea2da1e1dd42829f435a5bd0c8b2
```

## one_gadget
```
0xdf735 execve("/bin/sh", r10, [rbp-0x70])
constraints:
  [r10] == NULL || r10 == NULL
  [[rbp-0x70]] == NULL || [rbp-0x70] == NULL

0xdf739 execve("/bin/sh", r10, rdx)
constraints:
  [r10] == NULL || r10 == NULL
  [rdx] == NULL || rdx == NULL

0xdf73c execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL
```

## angry_gadget
```
libc_base + 0xdf70f :
	<Bool reg_rdx_14725_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14728_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14724_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool reg_rbp_14729_64{UNINITIALIZED} == 0x62>
	<Bool (reg_r10_14724_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xdf735 :
	<Bool reg_rbp_12433_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_r10_12435_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_12435_64{UNINITIALIZED} == 0xfffffffff0000000>
libc_base + 0xdf739 :
	<Bool reg_rbp_12440_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_12439_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_12439_64{UNINITIALIZED} == 0xffffffffffffffe0>
libc_base + 0xdf518 :
	<Bool reg_rdx_13736_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13738_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13735_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_13735_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xdf70c :
	<Bool reg_r10_14712_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14715_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_14716_64{UNINITIALIZED} == 0x6a>
	<Bool (reg_r10_14712_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf713 :
	<Bool reg_rdx_14738_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14741_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14742_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14743_64{UNINITIALIZED} == 0x6f>
libc_base + 0xdf717 :
	<Bool reg_rdx_14752_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14755_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14756_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14757_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf71f :
	<Bool reg_rdx_14767_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14769_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14770_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14771_64{UNINITIALIZED} == 0x6a>
libc_base + 0xdf54c :
	<Bool True>
	<Bool reg_r15_13396_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_13396_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0xdf54f :
	<Bool True>
	<Bool reg_r15_13399_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_13399_64{UNINITIALIZED} == 0xffffffffff800000>
libc_base + 0xdf51c :
	<Bool reg_rdx_13744_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13747_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13745_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf520 :
	<Bool reg_rdx_13754_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13756_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13753_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf523 :
	<Bool reg_rdx_13802_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13804_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13805_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf52a :
	<Bool reg_rdx_13812_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13815_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13816_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf532 :
	<Bool reg_rdx_13823_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13825_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13826_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf727 :
	<Bool reg_rax_14780_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_14781_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14782_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf72b :
	<Bool !(reg_cc_dep1_14792_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_14795_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14796_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf72d :
	<Bool reg_r10_12427_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12428_64{UNINITIALIZED} == 0x42>
libc_base + 0xdf7a6 :
	<Bool reg_rbp_13341_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_13341_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf7aa :
	<Bool reg_rbp_13346_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13346_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7ad :
	<Bool reg_rbp_13350_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13350_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7b1 :
	<Bool reg_rbp_13354_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_13356_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf53a :
	<Bool reg_rax_13833_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13834_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf53e :
	<Bool !(reg_cc_dep1_13841_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_13844_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf7eb :
	<Bool reg_rbp_14361_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_14361_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf7ef :
	<Bool reg_rbp_14366_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14366_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7f2 :
	<Bool reg_rbp_14370_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_14370_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7f6 :
	<Bool reg_rbp_14375_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_14377_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf7fa :
	<Bool reg_r10_14382_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_14383_64{UNINITIALIZED} == 0x6f>
libc_base + 0xdf7b5 :
	<Bool reg_r15_13360_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf544 :
	<Bool reg_r15_13391_64{UNINITIALIZED} == 0xffffffffffffffef>
```
