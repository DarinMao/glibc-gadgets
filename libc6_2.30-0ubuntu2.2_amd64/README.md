# libc6_2.30-0ubuntu2.2_amd64
Ubuntu GLIBC 2.30-0ubuntu2.2

```
MD5: 0f4ea249dca27daae534cf24ee67deb7
SHA1: 4ccc5527621a51871b05451c5b43525ea7bb87fa
```

## one_gadget
```
0xe6b93 execve("/bin/sh", r10, r12)
constraints:
  [r10] == NULL || r10 == NULL
  [r12] == NULL || r12 == NULL

0xe6b96 execve("/bin/sh", r10, rdx)
constraints:
  [r10] == NULL || r10 == NULL
  [rdx] == NULL || rdx == NULL

0xe6b99 execve("/bin/sh", rsi, rdx)
constraints:
  [rsi] == NULL || rsi == NULL
  [rdx] == NULL || rdx == NULL

0x10af39 execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0xe6b69 :
	<Bool reg_rdx_13723_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_13725_64{UNINITIALIZED} == 0x66>
	<Bool reg_rax_13727_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13722_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_r10_13722_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6b93 :
	<Bool reg_rbp_13392_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_13391_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_13391_64{UNINITIALIZED} == 0xfffffffffffff800>
libc_base + 0xe6b96 :
	<Bool reg_rbp_13397_64{UNINITIALIZED} == 0x77>
	<Bool True>
	<Bool reg_r10_13396_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_13396_64{UNINITIALIZED} == 0xfffffffffffe0000>
libc_base + 0xe6b66 :
	<Bool reg_r10_13711_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_13713_64{UNINITIALIZED} == 0x1>
	<Bool reg_rax_13715_64{UNINITIALIZED} == 0x1>
	<Bool (reg_r10_13711_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe6b6d :
	<Bool reg_rdx_13735_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_13737_64{UNINITIALIZED} == 0x42>
	<Bool reg_rax_13739_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13740_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b71 :
	<Bool reg_rdx_13749_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_13751_64{UNINITIALIZED} == 0x66>
	<Bool reg_rax_13753_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13754_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b79 :
	<Bool reg_rbp_13763_64{UNINITIALIZED} == 0x2>
	<Bool reg_rdx_13765_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13766_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13767_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b7d :
	<Bool reg_rdx_13776_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_13778_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13779_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13781_64{UNINITIALIZED} == 0x77>
libc_base + 0x10af45 :
	<Bool reg_rax_14400_64{UNINITIALIZED} == 0xfffff80000000000>
	<Bool True>
	<Bool reg_rsi_14402_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_14402_64{UNINITIALIZED} == 0xfffffffff0000000>
libc_base + 0x10af4c :
	<Bool reg_rax_14405_64{UNINITIALIZED} == 0xc000000000000000>
	<Bool True>
	<Bool reg_rsi_14407_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_14407_64{UNINITIALIZED} == 0xffffffffe0000000>
libc_base + 0xe696a :
	<Bool reg_rdx_14474_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14476_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14473_64{UNINITIALIZED}[63:3] == 0x1ffffffffffffffd>
	<Bool (reg_rcx_14473_64{UNINITIALIZED}[63:3] .. 0) == 0xffffffffffffffe8>
libc_base + 0xe6b85 :
	<Bool reg_rax_13790_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13791_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13793_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6b89 :
	<Bool !(reg_cc_dep1_13802_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_13805_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13807_64{UNINITIALIZED} == 0x77>
libc_base + 0xe699e :
	<Bool True>
	<Bool reg_r15_14349_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14349_64{UNINITIALIZED} == 0xffffffffffe00000>
libc_base + 0xe69a1 :
	<Bool True>
	<Bool reg_r15_14352_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r15_14352_64{UNINITIALIZED} == 0xffffffe000000000>
libc_base + 0x10af40 :
	<Bool True>
	<Bool reg_rax_14390_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_14390_64{UNINITIALIZED} == 0xfffffffffffff000>
libc_base + 0x10af4f :
	<Bool True>
	<Bool reg_rsi_14411_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_14411_64{UNINITIALIZED} == 0xfffffffffffc0000>
libc_base + 0xe696e :
	<Bool reg_rdx_14482_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_14485_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14483_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6972 :
	<Bool reg_rdx_14492_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14494_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_14491_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6975 :
	<Bool reg_rdx_14540_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14542_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14543_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe697c :
	<Bool reg_rdx_14550_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_14553_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14554_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6984 :
	<Bool reg_rdx_14561_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool reg_rax_14563_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14564_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6b8b :
	<Bool reg_r10_13384_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13386_64{UNINITIALIZED} == 0x77>
libc_base + 0xe6c09 :
	<Bool reg_rbp_13504_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_13504_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe6c0d :
	<Bool reg_rbp_13509_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13509_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c10 :
	<Bool reg_rbp_13513_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13513_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c14 :
	<Bool reg_rbp_13517_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r15_13519_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c4e :
	<Bool reg_rbp_13943_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13943_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c51 :
	<Bool reg_rbp_13948_64{UNINITIALIZED} == 0x4f>
	<Bool 0xffffffffffffffb0 + reg_rbp_13948_64{UNINITIALIZED} == 0xffffffffffffffff>
libc_base + 0xe6c55 :
	<Bool reg_rbp_13954_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_13957_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c59 :
	<Bool reg_rbp_13962_64{UNINITIALIZED} == 0x1>
	<Bool reg_r10_13964_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c5d :
	<Bool reg_rbp_13969_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_13971_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c61 :
	<Bool reg_r10_13976_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_13978_64{UNINITIALIZED} == 0x77>
libc_base + 0xe698c :
	<Bool reg_rax_14571_64{UNINITIALIZED} == 0x1>
	<Bool reg_r15_14572_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6990 :
	<Bool !(reg_cc_dep1_14579_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r15_14582_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6c18 :
	<Bool reg_r15_13523_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe6996 :
	<Bool reg_r15_14344_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x10af39 :
```
