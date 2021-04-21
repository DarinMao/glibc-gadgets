# libc6_2.27-3ubuntu1.2_amd64
Ubuntu GLIBC 2.27-3ubuntu1.2

```
MD5: 35ef4ffc9c6ad7ffd1fd8c16f14dc766
SHA1: a22321cd65f28f70cf321614fdfd22f36ecd0afe
```

## one_gadget
```
0x4f365 execve("/bin/sh", rsp+0x40, environ)
constraints:
  rsp & 0xf == 0
  rcx == NULL

0x4f3c2 execve("/bin/sh", rsp+0x40, environ)
constraints:
  [rsp+0x40] == NULL

0x10a45c execve("/bin/sh", rsp+0x70, environ)
constraints:
  [rsp+0x70] == NULL
```

## angry_gadget
```
libc_base + 0x10a468 :
	<Bool reg_rax_31924_64{UNINITIALIZED} == 0xffff000000000000>
	<Bool True>
	<Bool reg_rsi_31926_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_31926_64{UNINITIALIZED} == 0xfffffffffffffc00>
libc_base + 0x10a46f :
	<Bool reg_rax_31929_64{UNINITIALIZED} == 0xffc0000000000000>
	<Bool True>
	<Bool reg_rsi_31931_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_31931_64{UNINITIALIZED} == 0xfc00000000000000>
libc_base + 0x4f3d5 :
	<Bool reg_rax_31997_64{UNINITIALIZED} == 0xffffff0000000000>
	<Bool True>
	<Bool reg_rsi_31999_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_31999_64{UNINITIALIZED} == 0x1>
libc_base + 0x4f3df :
	<Bool reg_rax_32003_64{UNINITIALIZED} == 0xffff800000000000>
	<Bool True>
	<Bool reg_rsi_32005_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_32005_64{UNINITIALIZED} == 0xfffffc0000000000>
libc_base + 0x4f3e9 :
	<Bool reg_rax_32009_64{UNINITIALIZED} == 0xf800000000000000>
	<Bool True>
	<Bool reg_rsi_32011_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_32011_64{UNINITIALIZED} == 0xfffffffffffffe00>
libc_base + 0xe58bf :
	<Bool reg_rbp_32778_64{UNINITIALIZED} == 0x2>
	<Bool True>
	<Bool reg_r10_32780_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_32780_64{UNINITIALIZED} == 0xffffffc000000000>
libc_base + 0xe5872 :
	<Bool reg_rax_32988_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rbp_32991_64{UNINITIALIZED} == 0x44>
	<Bool reg_rcx_32989_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rax_32988_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5876 :
	<Bool reg_rax_32996_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rbp_32999_64{UNINITIALIZED} == 0x2>
	<Bool reg_rcx_32997_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rax_32996_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe587e :
	<Bool reg_rax_33011_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rbp_33014_64{UNINITIALIZED} == 0x54>
	<Bool reg_rcx_33012_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_33011_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5882 :
	<Bool reg_rax_33020_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_33022_64{UNINITIALIZED} == 0x1>
	<Bool reg_rcx_33019_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_33020_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe5886 :
	<Bool reg_rax_33027_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rbp_33029_64{UNINITIALIZED} == 0x57>
	<Bool !(reg_cc_dep1_33031_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_33027_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe588e :
	<Bool reg_rbp_33037_64{UNINITIALIZED} == 0x4>
	<Bool reg_rax_33039_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_33040_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rax_33039_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe5892 :
	<Bool reg_rax_33047_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_33049_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_rbp_33054_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rax_33047_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff0>
libc_base + 0xe589a :
	<Bool reg_rax_33058_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_33060_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_33063_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_33067_64{UNINITIALIZED} == 0x1>
libc_base + 0x10a463 :
	<Bool True>
	<Bool reg_rax_31914_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_31914_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0x10a472 :
	<Bool True>
	<Bool reg_rsi_31935_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_31935_64{UNINITIALIZED} == 0xfffffffffe000000>
libc_base + 0x4f3c9 :
	<Bool True>
	<Bool reg_rax_31988_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_31988_64{UNINITIALIZED} == 0xffffe00000000000>
libc_base + 0x4f3d0 :
	<Bool True>
	<Bool reg_rax_31992_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rax_31992_64{UNINITIALIZED} == 0xffffffffc0000000>
libc_base + 0x4f3ec :
	<Bool True>
	<Bool reg_rsi_32015_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_32015_64{UNINITIALIZED} == 0xfff8000000000000>
libc_base + 0xe56c4 :
	<Bool reg_rcx_32628_64{UNINITIALIZED}[63:4] == 0x7ffffffffff000>
	<Bool reg_rax_32629_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * (reg_rcx_32628_64{UNINITIALIZED}[63:4] .. 0)[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe56c8 :
	<Bool reg_rcx_32635_64{UNINITIALIZED} == 0x7ffffffffff0000>
	<Bool reg_rax_32636_64{UNINITIALIZED} == 0x1>
	<Bool (0x7fffffffffeffff + 0xffffffffffffffff * reg_rcx_32635_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe56d0 :
	<Bool reg_rcx_32648_64{UNINITIALIZED}[63:3] == 0x1fffffffffffffff>
	<Bool reg_rax_32649_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_32648_64{UNINITIALIZED}[63:3] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe56d4 :
	<Bool reg_rcx_32656_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool reg_rax_32655_64{UNINITIALIZED} == 0x1>
	<Bool (reg_rcx_32656_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe56d8 :
	<Bool reg_rcx_32662_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_32665_64{UNINITIALIZED}[6:6] == 0)>
	<Bool (reg_rcx_32662_64{UNINITIALIZED}[60:0] .. 0) == 0xfffffffffffffff8>
libc_base + 0xe56e0 :
	<Bool reg_rcx_32671_64{UNINITIALIZED}[60:0] == 0x1fffffffffffffff>
	<Bool !(reg_cc_dep1_32674_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r14_32677_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe56e8 :
	<Bool reg_rcx_32683_64{UNINITIALIZED}[60:0] == 0x1ffffffffffffffe>
	<Bool !(reg_cc_dep1_32685_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r14_32688_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58c3 :
	<Bool True>
	<Bool reg_r10_32788_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_32788_64{UNINITIALIZED} == 0xfffffffff8000000>
libc_base + 0xe58ca :
	<Bool True>
	<Bool reg_r10_32792_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r10_32792_64{UNINITIALIZED} == 0xfffffffffff00000>
libc_base + 0xe58cd :
	<Bool True>
	<Bool reg_rsi_32797_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_32797_64{UNINITIALIZED} == 0xffc0000000000000>
libc_base + 0xe5879 :
	<Bool reg_rbp_33006_64{UNINITIALIZED} == 0x56>
	<Bool reg_rcx_33004_64{UNINITIALIZED} == 0x1>
	<Bool reg_rbp_33006_64{UNINITIALIZED} + 0xffffffffffffff90 == 0xffffffffffffffe6>
libc_base + 0xe58a2 :
	<Bool !(reg_cc_dep1_33071_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r10_33074_64{UNINITIALIZED} == 0xffffffffffffffef>
	<Bool reg_rbp_33078_64{UNINITIALIZED} == 0x1>
libc_base + 0xe56ff :
	<Bool True>
	<Bool reg_r14_33140_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r14_33140_64{UNINITIALIZED} == 0xc000000000000000>
libc_base + 0xe5706 :
	<Bool True>
	<Bool reg_r14_33144_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r14_33144_64{UNINITIALIZED} == 0xfffff80000000000>
libc_base + 0xe5709 :
	<Bool True>
	<Bool reg_r14_33148_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_r14_33148_64{UNINITIALIZED} == 0xf800000000000000>
libc_base + 0xe570c :
	<Bool True>
	<Bool reg_rsi_33153_64{UNINITIALIZED} <= 0xffffffffffffffff>
	<Bool reg_rsi_33153_64{UNINITIALIZED} == 0x1>
libc_base + 0xe56f0 :
	<Bool !(reg_cc_dep1_32694_64{UNINITIALIZED}[6:6] == 0)>
	<Bool reg_r14_32697_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58e0 :
	<Bool reg_rbp_32703_64{UNINITIALIZED} == 0x2>
	<Bool mem_ffffffffffffff8a_32704_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58e7 :
	<Bool reg_rbp_32709_64{UNINITIALIZED} == 0x3a>
	<Bool mem_ffffffffffffffc2_32710_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58eb :
	<Bool reg_rbp_32715_64{UNINITIALIZED} == 0x7f>
	<Bool reg_r10_32718_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58ef :
	<Bool reg_rbp_32722_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r10_32725_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58f3 :
	<Bool reg_rbp_32729_64{UNINITIALIZED} == 0x56>
	<Bool reg_r10_32731_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe58f7 :
	<Bool reg_rbp_32735_64{UNINITIALIZED} == 0x47>
	<Bool reg_r10_32737_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5720 :
	<Bool reg_rbp_34301_64{UNINITIALIZED} == 0x47>
	<Bool 0xffffffffffffffb0 + reg_rbp_34301_64{UNINITIALIZED} == 0xfffffffffffffff7>
libc_base + 0xe5724 :
	<Bool reg_rbp_34306_64{UNINITIALIZED} == 0x47>
	<Bool reg_r14_34309_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe5727 :
	<Bool reg_rbp_34313_64{UNINITIALIZED} == 0x47>
	<Bool reg_r14_34316_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe572b :
	<Bool reg_rbp_34320_64{UNINITIALIZED} == 0x4f>
	<Bool reg_r14_34322_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0xe56cb :
	<Bool reg_rax_32642_64{UNINITIALIZED} == 0x1>
libc_base + 0xe572f :
	<Bool reg_r14_34326_64{UNINITIALIZED} == 0xffffffffffffffef>
libc_base + 0x10a45c :
libc_base + 0x4f3c2 :
```
