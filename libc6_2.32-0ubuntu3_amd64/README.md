# libc6_2.32-0ubuntu3_amd64
Ubuntu GLIBC 2.32-0ubuntu3

```
MD5: 466d3c76ab2fc51a488b38b928e8ffb9
SHA1: 274201bd6666cb31fd090632224af3da63b0f6a3
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
	<Bool reg_rdx_13629_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13632_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13628_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool reg_rbp_13633_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r10_13628_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xdf518 :
	<Bool reg_rdx_12701_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12703_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_12700_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_12700_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xdf70c :
	<Bool reg_r10_13616_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13619_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_13620_64{UNINITIALIZED} == 0x6e>
	<Bool (reg_r10_13616_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf713 :
	<Bool reg_rdx_13642_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13645_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13646_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13647_64{UNINITIALIZED} == 0x6f>
libc_base + 0xdf717 :
	<Bool reg_rdx_13656_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13659_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13660_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13661_64{UNINITIALIZED} == 0x2>
libc_base + 0xdf71f :
	<Bool reg_rdx_13671_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13673_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13674_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13675_64{UNINITIALIZED} == 0x1>
libc_base + 0xdf735 :
	<Bool reg_rbp_13891_64{UNINITIALIZED} == 0x1>
	<Bool True>
	<Bool reg_r10_13893_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_13893_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0xdf739 :
	<Bool reg_rbp_13898_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_13897_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_13897_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0xdf54c :
	<Bool True>
	<Bool reg_r15_12431_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_12431_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xdf54f :
	<Bool True>
	<Bool reg_r15_12434_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_12434_64{UNINITIALIZED} == 0xffffffc000000000>
libc_base + 0xdf51c :
	<Bool reg_rdx_12709_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12712_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_12710_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf520 :
	<Bool reg_rdx_12719_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12721_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_12718_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf523 :
	<Bool reg_rdx_12767_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12769_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12770_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf52a :
	<Bool reg_rdx_12777_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12780_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12781_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf532 :
	<Bool reg_rdx_12788_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_12790_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12791_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf727 :
	<Bool reg_rax_13685_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13686_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13687_64{UNINITIALIZED} == 0x6f>
libc_base + 0xdf72b :
	<Bool !(reg_cc_dep1_13696_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_13699_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13700_64{UNINITIALIZED} == 0x2>
libc_base + 0xdf53a :
	<Bool reg_rax_12798_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_12799_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf53e :
	<Bool !(reg_cc_dep1_12806_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_12809_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf7eb :
	<Bool reg_rbp_13827_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_13827_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf7ef :
	<Bool reg_rbp_13832_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13832_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7f2 :
	<Bool reg_rbp_13836_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13836_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7f6 :
	<Bool reg_rbp_13841_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_13843_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf7fa :
	<Bool reg_r10_13848_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13849_64{UNINITIALIZED} == 0x6a>
libc_base + 0xdf72d :
	<Bool reg_r10_13885_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13886_64{UNINITIALIZED} == 0x2>
libc_base + 0xdf7a6 :
	<Bool reg_rbp_13951_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_13951_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf7aa :
	<Bool reg_rbp_13956_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13956_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7ad :
	<Bool reg_rbp_13960_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13960_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf7b1 :
	<Bool reg_rbp_13964_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_13966_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf544 :
	<Bool reg_r15_12426_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf7b5 :
	<Bool reg_r15_13970_64{UNINITIALIZED} == 0xffffffffffffffef>
```
