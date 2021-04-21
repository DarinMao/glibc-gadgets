# libc6_2.32-0ubuntu6_amd64
Ubuntu GLIBC 2.32-0ubuntu6

```
MD5: c1412b7848916b43f3595c0865ad3f1c
SHA1: c5932550cddc354b739a62cedd27a1e021897b85
```

## one_gadget
```
0xdf555 execve("/bin/sh", r10, [rbp-0x70])
constraints:
  [r10] == NULL || r10 == NULL
  [[rbp-0x70]] == NULL || [rbp-0x70] == NULL

0xdf559 execve("/bin/sh", r10, rdx)
constraints:
  [r10] == NULL || r10 == NULL
  [rdx] == NULL || rdx == NULL

0xdf55c execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL
```

## angry_gadget
```
libc_base + 0xdf52f :
	<Bool reg_rdx_12530_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12533_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_12529_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool reg_rbp_12534_64{UNINITIALIZED} == 0x42>
	<Bool (reg_r10_12529_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xdf52c :
	<Bool reg_r10_12517_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12520_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_12521_64{UNINITIALIZED} == 0x62>
	<Bool (reg_r10_12517_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf533 :
	<Bool reg_rdx_12543_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12546_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_12547_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12548_64{UNINITIALIZED} == 0x62>
libc_base + 0xdf537 :
	<Bool reg_rdx_12557_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_12560_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_12561_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12562_64{UNINITIALIZED} == 0x6f>
libc_base + 0xdf53f :
	<Bool reg_rdx_12571_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_12573_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_12574_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12575_64{UNINITIALIZED} == 0x2>
libc_base + 0xdf525 :
	<Bool reg_r10_12621_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_12623_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_12624_64{UNINITIALIZED} == 0x6f>
	<Bool (reg_r10_12621_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xdf555 :
	<Bool reg_rbp_12733_64{UNINITIALIZED} == 0x6f>
	<Bool True>
	<Bool reg_r10_12735_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_12735_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xdf559 :
	<Bool reg_rbp_12740_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_12739_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_12739_64{UNINITIALIZED} == 0xfffffff800000000>
libc_base + 0xdf338 :
	<Bool reg_rdx_13108_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13110_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13107_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_13107_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xdf547 :
	<Bool reg_rax_12585_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_12586_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12587_64{UNINITIALIZED} == 0x42>
libc_base + 0xdf54b :
	<Bool !(reg_cc_dep1_12597_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_12600_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12601_64{UNINITIALIZED} == 0x42>
libc_base + 0xdf36c :
	<Bool True>
	<Bool reg_r15_12797_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_12797_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0xdf36f :
	<Bool True>
	<Bool reg_r15_12800_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_12800_64{UNINITIALIZED} == 0xffffffffffffff00>
libc_base + 0xdf33c :
	<Bool reg_rdx_13116_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_13119_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13117_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf340 :
	<Bool reg_rdx_13126_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13128_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_13125_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf343 :
	<Bool reg_rdx_13174_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13176_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13177_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf34a :
	<Bool reg_rdx_13184_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_13187_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13188_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf352 :
	<Bool reg_rdx_13195_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13197_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13198_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf5c6 :
	<Bool reg_rbp_12436_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_12436_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf5ca :
	<Bool reg_rbp_12441_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_12441_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf5cd :
	<Bool reg_rbp_12445_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_12445_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf5d1 :
	<Bool reg_rbp_12449_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_12451_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf54d :
	<Bool reg_r10_12727_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12728_64{UNINITIALIZED} == 0x6a>
libc_base + 0xdf60b :
	<Bool reg_rbp_12968_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_12968_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xdf60f :
	<Bool reg_rbp_12973_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_12973_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf612 :
	<Bool reg_rbp_12977_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_12977_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xdf616 :
	<Bool reg_rbp_12982_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_12984_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf61a :
	<Bool reg_r10_12989_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_12990_64{UNINITIALIZED} == 0x62>
libc_base + 0xdf35a :
	<Bool reg_rax_13205_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_13206_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf35e :
	<Bool !(reg_cc_dep1_13213_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_13216_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf5d5 :
	<Bool reg_r15_12455_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xdf364 :
	<Bool reg_r15_12792_64{UNINITIALIZED} == 0xffffffffffffffef>
```
