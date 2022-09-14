
# Data Propagation Report

- **STAT1** : Number of instructions that hit unique coverpoints and update the signature.
- **STAT2** : Number of instructions that hit covepoints which are not unique but still update the signature
- **STAT3** : Number of instructions that hit a unique coverpoint but do not update signature
- **STAT4** : Number of multiple signature updates for the same coverpoint
- **STAT5** : Number of times the signature was overwritten

| Param                     | Value    |
|---------------------------|----------|
| XLEN                      | 64      |
| TEST_REGION               | [('0x80000390', '0x80001eb0')]      |
| SIG_REGION                | [('0x80003010', '0x800037b0', '244 dwords')]      |
| COV_LABELS                | sm3p0      |
| TEST_NAME                 | /scratch/git-repo/incoresemi/temp/riscof_work/sm3p0-rwp1.S/ref.S    |
| Total Number of coverpoints| 220     |
| Total Coverpoints Hit     | 56      |
| Total Signature Updates   | 243      |
| STAT1                     | 27      |
| STAT2                     | 54      |
| STAT3                     | 0     |
| STAT4                     | 162     |
| STAT5                     | 0     |

## Details for STAT2:

```
Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000434]:sm3p0
      [0x80000438]:xori
      [0x8000043c]:sd
 -- Signature Address: 0x80003028 Data: 0x6c0235478476d693
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x3
      - rd : x1
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000048c]:sm3p0
      [0x80000490]:add
      [0x80000494]:sd
 -- Signature Address: 0x80003040 Data: 0x9c55496a0dd09a3f
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x3
      - rd : x1
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000052c]:sm3p0
      [0x80000530]:xori
      [0x80000534]:sd
 -- Signature Address: 0x80003070 Data: 0xa38b1ba100e1a410
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x4
      - rd : x2
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000057c]:sm3p0
      [0x80000580]:add
      [0x80000584]:sd
 -- Signature Address: 0x80003088 Data: 0x6fef7bd653074732
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x4
      - rd : x2
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000062c]:sm3p0
      [0x80000630]:xori
      [0x80000634]:sd
 -- Signature Address: 0x800030b8 Data: 0xa32d78a156913d4c
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x5
      - rd : x3
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000684]:sm3p0
      [0x80000688]:add
      [0x8000068c]:sd
 -- Signature Address: 0x800030d0 Data: 0x0c6725bcd625f8df
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x5
      - rd : x3
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000734]:sm3p0
      [0x80000738]:xori
      [0x8000073c]:sd
 -- Signature Address: 0x80003100 Data: 0xc2836a061a0fcf81
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x6
      - rd : x4
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000078c]:sm3p0
      [0x80000790]:add
      [0x80000794]:sd
 -- Signature Address: 0x80003118 Data: 0x26575c5dd6d5b6ce
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x6
      - rd : x4
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000083c]:sm3p0
      [0x80000840]:xori
      [0x80000844]:sd
 -- Signature Address: 0x80003148 Data: 0xc2f9ebc8964e2340
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x7
      - rd : x5
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000894]:sm3p0
      [0x80000898]:add
      [0x8000089c]:sd
 -- Signature Address: 0x80003160 Data: 0xbd83b67d41c6b234
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x7
      - rd : x5
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000944]:sm3p0
      [0x80000948]:xori
      [0x8000094c]:sd
 -- Signature Address: 0x80003190 Data: 0xb9ad09d251b7c65e
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x8
      - rd : x6
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000099c]:sm3p0
      [0x800009a0]:add
      [0x800009a4]:sd
 -- Signature Address: 0x800031a8 Data: 0xb866479b18496d21
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x8
      - rd : x6
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000a4c]:sm3p0
      [0x80000a50]:xori
      [0x80000a54]:sd
 -- Signature Address: 0x800031d8 Data: 0xf4d1d9964994cd7b
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x9
      - rd : x7
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000aa4]:sm3p0
      [0x80000aa8]:add
      [0x80000aac]:sd
 -- Signature Address: 0x800031f0 Data: 0x5f2a25d60f65a0a0
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x9
      - rd : x7
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000b34]:sm3p0
      [0x80000b38]:xori
      [0x80000b3c]:sd
 -- Signature Address: 0x80003220 Data: 0xefee114b8007dd12
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x10
      - rd : x8
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000b7c]:sm3p0
      [0x80000b80]:add
      [0x80000b84]:sd
 -- Signature Address: 0x80003238 Data: 0xf92aad547dfda0b2
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x10
      - rd : x8
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000c2c]:sm3p0
      [0x80000c30]:xori
      [0x80000c34]:sd
 -- Signature Address: 0x80003268 Data: 0x8f03e50370f7b95d
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x11
      - rd : x9
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000c84]:sm3p0
      [0x80000c88]:add
      [0x80000c8c]:sd
 -- Signature Address: 0x80003280 Data: 0x24a25aa00c721591
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x11
      - rd : x9
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000d34]:sm3p0
      [0x80000d38]:xori
      [0x80000d3c]:sd
 -- Signature Address: 0x800032b0 Data: 0x8d8bacf813cda113
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x12
      - rd : x10
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000d8c]:sm3p0
      [0x80000d90]:add
      [0x80000d94]:sd
 -- Signature Address: 0x800032c8 Data: 0x3f220927ea532d08
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x12
      - rd : x10
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000e2c]:sm3p0
      [0x80000e30]:xori
      [0x80000e34]:sd
 -- Signature Address: 0x800032f8 Data: 0x3141db26f99ff86d
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x13
      - rd : x11
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000e7c]:sm3p0
      [0x80000e80]:add
      [0x80000e84]:sd
 -- Signature Address: 0x80003310 Data: 0x6f9ee25fdab51b9a
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x13
      - rd : x11
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000f2c]:sm3p0
      [0x80000f30]:xori
      [0x80000f34]:sd
 -- Signature Address: 0x80003340 Data: 0x547acb3ed65da8a0
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x14
      - rd : x12
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80000f84]:sm3p0
      [0x80000f88]:add
      [0x80000f8c]:sd
 -- Signature Address: 0x80003358 Data: 0x7c995be624da1627
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x14
      - rd : x12
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001024]:sm3p0
      [0x80001028]:xori
      [0x8000102c]:sd
 -- Signature Address: 0x80003388 Data: 0xfe04416c5f747b0c
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x15
      - rd : x13
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001074]:sm3p0
      [0x80001078]:add
      [0x8000107c]:sd
 -- Signature Address: 0x800033a0 Data: 0x9af382afe49cdff7
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x15
      - rd : x13
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001124]:sm3p0
      [0x80001128]:xori
      [0x8000112c]:sd
 -- Signature Address: 0x800033d0 Data: 0x8b0a522aa3c87b65
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x16
      - rd : x14
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000117c]:sm3p0
      [0x80001180]:add
      [0x80001184]:sd
 -- Signature Address: 0x800033e8 Data: 0xce0c80566a5c5e66
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x16
      - rd : x14
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000122c]:sm3p0
      [0x80001230]:xori
      [0x80001234]:sd
 -- Signature Address: 0x80003418 Data: 0x69ae119a85e2cc35
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x17
      - rd : x15
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001284]:sm3p0
      [0x80001288]:add
      [0x8000128c]:sd
 -- Signature Address: 0x80003430 Data: 0xdd3f62c5341c25a0
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x17
      - rd : x15
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001334]:sm3p0
      [0x80001338]:xori
      [0x8000133c]:sd
 -- Signature Address: 0x80003460 Data: 0x64ee2c7cb7b9be0a
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x18
      - rd : x16
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000138c]:sm3p0
      [0x80001390]:add
      [0x80001394]:sd
 -- Signature Address: 0x80003478 Data: 0x374edbffadc99dd4
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x18
      - rd : x16
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000143c]:sm3p0
      [0x80001440]:xori
      [0x80001444]:sd
 -- Signature Address: 0x800034a8 Data: 0x6cfe896f1ca9ad63
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x19
      - rd : x17
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001494]:sm3p0
      [0x80001498]:add
      [0x8000149c]:sd
 -- Signature Address: 0x800034c0 Data: 0x971d313c7b41ceab
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x19
      - rd : x17
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001544]:sm3p0
      [0x80001548]:xori
      [0x8000154c]:sd
 -- Signature Address: 0x800034f0 Data: 0x3a2f646bd41d2736
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x20
      - rd : x18
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000159c]:sm3p0
      [0x800015a0]:add
      [0x800015a4]:sd
 -- Signature Address: 0x80003508 Data: 0xb5380c9b07fa8737
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x20
      - rd : x18
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000163c]:sm3p0
      [0x80001640]:xori
      [0x80001644]:sd
 -- Signature Address: 0x80003538 Data: 0xe728e41bce3ffa8f
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x21
      - rd : x19
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000168c]:sm3p0
      [0x80001690]:add
      [0x80001694]:sd
 -- Signature Address: 0x80003550 Data: 0x8e307d8db507e365
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x21
      - rd : x19
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000173c]:sm3p0
      [0x80001740]:xori
      [0x80001744]:sd
 -- Signature Address: 0x80003580 Data: 0xd5a23f5ff2bac320
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x22
      - rd : x20
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001794]:sm3p0
      [0x80001798]:add
      [0x8000179c]:sd
 -- Signature Address: 0x80003598 Data: 0xb9800962697ab4d4
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x22
      - rd : x20
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001834]:sm3p0
      [0x80001838]:xori
      [0x8000183c]:sd
 -- Signature Address: 0x800035c8 Data: 0x3d8ec31da797efa4
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x23
      - rd : x21
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001884]:sm3p0
      [0x80001888]:add
      [0x8000188c]:sd
 -- Signature Address: 0x800035e0 Data: 0x303509d11bd80da6
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x23
      - rd : x21
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001934]:sm3p0
      [0x80001938]:xori
      [0x8000193c]:sd
 -- Signature Address: 0x80003610 Data: 0x615890f77a6a777e
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x24
      - rd : x22
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x8000198c]:sm3p0
      [0x80001990]:add
      [0x80001994]:sd
 -- Signature Address: 0x80003628 Data: 0x82ddebd35f06f7ad
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x24
      - rd : x22
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001a3c]:sm3p0
      [0x80001a40]:xori
      [0x80001a44]:sd
 -- Signature Address: 0x80003658 Data: 0xecd58e89f9513eaf
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x25
      - rd : x23
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001a94]:sm3p0
      [0x80001a98]:add
      [0x80001a9c]:sd
 -- Signature Address: 0x80003670 Data: 0x4aef382f9bdf9ce3
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x25
      - rd : x23
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001b44]:sm3p0
      [0x80001b48]:xori
      [0x80001b4c]:sd
 -- Signature Address: 0x800036a0 Data: 0xcc679c3b2de91157
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x26
      - rd : x24
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001b9c]:sm3p0
      [0x80001ba0]:add
      [0x80001ba4]:sd
 -- Signature Address: 0x800036b8 Data: 0x386c49b8fde3c55e
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x26
      - rd : x24
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001c4c]:sm3p0
      [0x80001c50]:xori
      [0x80001c54]:sd
 -- Signature Address: 0x800036e8 Data: 0xd277af9d0556869a
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x27
      - rd : x25
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001ca4]:sm3p0
      [0x80001ca8]:add
      [0x80001cac]:sd
 -- Signature Address: 0x80003700 Data: 0x0434d58201bed3ee
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x27
      - rd : x25
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001d54]:sm3p0
      [0x80001d58]:xori
      [0x80001d5c]:sd
 -- Signature Address: 0x80003730 Data: 0x4c18c344f27da73b
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x28
      - rd : x26
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001dac]:sm3p0
      [0x80001db0]:add
      [0x80001db4]:sd
 -- Signature Address: 0x80003748 Data: 0x4122e41019be8a6c
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x28
      - rd : x26
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001e4c]:sm3p0
      [0x80001e50]:xori
      [0x80001e54]:sd
 -- Signature Address: 0x80003778 Data: 0xd2eccdf1bf2f1a18
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x29
      - rd : x27
      - rs1 != rd




Op without unique coverpoint updates Signature
 -- Code Sequence:
      [0x80001e9c]:sm3p0
      [0x80001ea0]:add
      [0x80001ea4]:sd
 -- Signature Address: 0x80003790 Data: 0x50ab860752e0df3e
 -- Redundant Coverpoints hit by the op
      - opcode : sm3p0
      - rs1 : x29
      - rd : x27
      - rs1 != rd






```

## Details of STAT3

```


```

## Details of STAT4:

```
Last Coverpoint : ['opcode : sm3p0', 'rs1 : x3', 'rd : x1', 'rs1 != rd']
Last Code Sequence : 
	-[0x800003dc]:sm3p0
	-[0x800003e0]:xor
	-[0x800003e4]:sd
Current Store : [0x800003e8] : None -- Store: [0x80003018]:0x00000000c602f5f0




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x3', 'rd : x1', 'rs1 != rd']
Last Code Sequence : 
	-[0x800003dc]:sm3p0
	-[0x800003e0]:xor
	-[0x800003e4]:sd
Current Store : [0x800003ec] : None -- Store: [0x80003020]:0x93fdcab8bd8bdc9c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x3', 'rd : x1', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000434]:sm3p0
	-[0x80000438]:xori
	-[0x8000043c]:sd
Current Store : [0x80000440] : None -- Store: [0x80003030]:0x00000000c4fcf976




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x3', 'rd : x1', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000434]:sm3p0
	-[0x80000438]:xori
	-[0x8000043c]:sd
Current Store : [0x80000444] : None -- Store: [0x80003038]:0xffffffff3b030689




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x3', 'rd : x1', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000048c]:sm3p0
	-[0x80000490]:add
	-[0x80000494]:sd
Current Store : [0x80000498] : None -- Store: [0x80003048]:0x00000000989aff85




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x3', 'rd : x1', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000048c]:sm3p0
	-[0x80000490]:add
	-[0x80000494]:sd
Current Store : [0x8000049c] : None -- Store: [0x80003050]:0x93fdcab9142428f1




Last Coverpoint : ['rs1 : x4', 'rd : x2']
Last Code Sequence : 
	-[0x800004dc]:sm3p0
	-[0x800004e0]:xor
	-[0x800004e4]:sd
Current Store : [0x800004e8] : None -- Store: [0x80003060]:0x0000000020ceb018




Last Coverpoint : ['rs1 : x4', 'rd : x2']
Last Code Sequence : 
	-[0x800004dc]:sm3p0
	-[0x800004e0]:xor
	-[0x800004e4]:sd
Current Store : [0x800004ec] : None -- Store: [0x80003068]:0x5c74e45edfd0ebf7




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x4', 'rd : x2', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000052c]:sm3p0
	-[0x80000530]:xori
	-[0x80000534]:sd
Current Store : [0x80000538] : None -- Store: [0x80003078]:0x000000008b8985d2




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x4', 'rd : x2', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000052c]:sm3p0
	-[0x80000530]:xori
	-[0x80000534]:sd
Current Store : [0x8000053c] : None -- Store: [0x80003080]:0xffffffff74767a2d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x4', 'rd : x2', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000057c]:sm3p0
	-[0x80000580]:add
	-[0x80000584]:sd
Current Store : [0x80000588] : None -- Store: [0x80003090]:0x00000000d3ed859a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x4', 'rd : x2', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000057c]:sm3p0
	-[0x80000580]:add
	-[0x80000584]:sd
Current Store : [0x8000058c] : None -- Store: [0x80003098]:0x5c74e45fd30be189




Last Coverpoint : ['rs1 : x5', 'rd : x3']
Last Code Sequence : 
	-[0x800005d4]:sm3p0
	-[0x800005d8]:xor
	-[0x800005dc]:sd
Current Store : [0x800005e0] : None -- Store: [0x800030a8]:0x00000000df0fc027




Last Coverpoint : ['rs1 : x5', 'rd : x3']
Last Code Sequence : 
	-[0x800005d4]:sm3p0
	-[0x800005d8]:xor
	-[0x800005dc]:sd
Current Store : [0x800005e4] : None -- Store: [0x800030b0]:0x5cd2875e76610294




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x5', 'rd : x3', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000062c]:sm3p0
	-[0x80000630]:xori
	-[0x80000634]:sd
Current Store : [0x80000638] : None -- Store: [0x800030c0]:0x000000000e7308c3




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x5', 'rd : x3', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000062c]:sm3p0
	-[0x80000630]:xori
	-[0x80000634]:sd
Current Store : [0x8000063c] : None -- Store: [0x800030c8]:0xfffffffff18cf73c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x5', 'rd : x3', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000684]:sm3p0
	-[0x80000688]:add
	-[0x8000068c]:sd
Current Store : [0x80000690] : None -- Store: [0x800030d8]:0x000000006c6beb38




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x5', 'rd : x3', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000684]:sm3p0
	-[0x80000688]:add
	-[0x8000068c]:sd
Current Store : [0x80000694] : None -- Store: [0x800030e0]:0x5cd2875f15daadeb




Last Coverpoint : ['rs1 : x6', 'rd : x4']
Last Code Sequence : 
	-[0x800006dc]:sm3p0
	-[0x800006e0]:xor
	-[0x800006e4]:sd
Current Store : [0x800006e8] : None -- Store: [0x800030f0]:0x000000005225c02f




Last Coverpoint : ['rs1 : x6', 'rd : x4']
Last Code Sequence : 
	-[0x800006dc]:sm3p0
	-[0x800006e0]:xor
	-[0x800006e4]:sd
Current Store : [0x800006ec] : None -- Store: [0x800030f8]:0x3d7c95f9b7d5f051




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x6', 'rd : x4', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000734]:sm3p0
	-[0x80000738]:xori
	-[0x8000073c]:sd
Current Store : [0x80000740] : None -- Store: [0x80003108]:0x000000009a92f9aa




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x6', 'rd : x4', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000734]:sm3p0
	-[0x80000738]:xori
	-[0x8000073c]:sd
Current Store : [0x80000744] : None -- Store: [0x80003110]:0xffffffff656d0655




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x6', 'rd : x4', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000078c]:sm3p0
	-[0x80000790]:add
	-[0x80000794]:sd
Current Store : [0x80000798] : None -- Store: [0x80003120]:0x00000000102586c8




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x6', 'rd : x4', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000078c]:sm3p0
	-[0x80000790]:add
	-[0x80000794]:sd
Current Store : [0x8000079c] : None -- Store: [0x80003128]:0x3d7c95f9f615b746




Last Coverpoint : ['rs1 : x7', 'rd : x5']
Last Code Sequence : 
	-[0x800007e4]:sm3p0
	-[0x800007e8]:xor
	-[0x800007ec]:sd
Current Store : [0x800007f0] : None -- Store: [0x80003138]:0x00000000e823ffe3




Last Coverpoint : ['rs1 : x7', 'rd : x5']
Last Code Sequence : 
	-[0x800007e4]:sm3p0
	-[0x800007e8]:xor
	-[0x800007ec]:sd
Current Store : [0x800007f4] : None -- Store: [0x80003140]:0x3d0614378192235c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x7', 'rd : x5', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000083c]:sm3p0
	-[0x80000840]:xori
	-[0x80000844]:sd
Current Store : [0x80000848] : None -- Store: [0x80003150]:0x000000004c898ef0




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x7', 'rd : x5', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000083c]:sm3p0
	-[0x80000840]:xori
	-[0x80000844]:sd
Current Store : [0x8000084c] : None -- Store: [0x80003158]:0xffffffffb376710f




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x7', 'rd : x5', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000894]:sm3p0
	-[0x80000898]:add
	-[0x8000089c]:sd
Current Store : [0x800008a0] : None -- Store: [0x80003168]:0x00000000a8ca593a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x7', 'rd : x5', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000894]:sm3p0
	-[0x80000898]:add
	-[0x8000089c]:sd
Current Store : [0x800008a4] : None -- Store: [0x80003170]:0x3d061438127c35f9




Last Coverpoint : ['rs1 : x8', 'rd : x6']
Last Code Sequence : 
	-[0x800008ec]:sm3p0
	-[0x800008f0]:xor
	-[0x800008f4]:sd
Current Store : [0x800008f8] : None -- Store: [0x80003180]:0x00000000421ec13b




Last Coverpoint : ['rs1 : x8', 'rd : x6']
Last Code Sequence : 
	-[0x800008ec]:sm3p0
	-[0x800008f0]:xor
	-[0x800008f4]:sd
Current Store : [0x800008fc] : None -- Store: [0x80003188]:0x4652f62dec56f89a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x8', 'rd : x6', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000944]:sm3p0
	-[0x80000948]:xori
	-[0x8000094c]:sd
Current Store : [0x80000950] : None -- Store: [0x80003198]:0x00000000b287d992




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x8', 'rd : x6', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000944]:sm3p0
	-[0x80000948]:xori
	-[0x8000094c]:sd
Current Store : [0x80000954] : None -- Store: [0x800031a0]:0xffffffff4d78266d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x8', 'rd : x6', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000099c]:sm3p0
	-[0x800009a0]:add
	-[0x800009a4]:sd
Current Store : [0x800009a8] : None -- Store: [0x800031b0]:0x0000000050d11f83




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x8', 'rd : x6', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000099c]:sm3p0
	-[0x800009a0]:add
	-[0x800009a4]:sd
Current Store : [0x800009ac] : None -- Store: [0x800031b8]:0x4652f62dff195924




Last Coverpoint : ['rs1 : x9', 'rd : x7']
Last Code Sequence : 
	-[0x800009f4]:sm3p0
	-[0x800009f8]:xor
	-[0x800009fc]:sd
Current Store : [0x80000a00] : None -- Store: [0x800031c8]:0x000000007519b067




Last Coverpoint : ['rs1 : x9', 'rd : x7']
Last Code Sequence : 
	-[0x800009f4]:sm3p0
	-[0x800009f8]:xor
	-[0x800009fc]:sd
Current Store : [0x80000a04] : None -- Store: [0x800031d0]:0x0b2e2669c37282e3




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x9', 'rd : x7', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000a4c]:sm3p0
	-[0x80000a50]:xori
	-[0x80000a54]:sd
Current Store : [0x80000a58] : None -- Store: [0x800031e0]:0x00000000faf8a8c1




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x9', 'rd : x7', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000a4c]:sm3p0
	-[0x80000a50]:xori
	-[0x80000a54]:sd
Current Store : [0x80000a5c] : None -- Store: [0x800031e8]:0xffffffff0507573e




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x9', 'rd : x7', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000aa4]:sm3p0
	-[0x80000aa8]:add
	-[0x80000aac]:sd
Current Store : [0x80000ab0] : None -- Store: [0x800031f8]:0x000000008564fe75




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x9', 'rd : x7', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000aa4]:sm3p0
	-[0x80000aa8]:add
	-[0x80000aac]:sd
Current Store : [0x80000ab4] : None -- Store: [0x80003200]:0x0b2e266a3bd030f9




Last Coverpoint : ['rs1 : x10', 'rd : x8']
Last Code Sequence : 
	-[0x80000aec]:sm3p0
	-[0x80000af0]:xor
	-[0x80000af4]:sd
Current Store : [0x80000af8] : None -- Store: [0x80003210]:0x00000000c5120dd1




Last Coverpoint : ['rs1 : x10', 'rd : x8']
Last Code Sequence : 
	-[0x80000aec]:sm3p0
	-[0x80000af0]:xor
	-[0x80000af4]:sd
Current Store : [0x80000afc] : None -- Store: [0x80003218]:0x1011eeb4baea2f3c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x10', 'rd : x8', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000b34]:sm3p0
	-[0x80000b38]:xori
	-[0x80000b3c]:sd
Current Store : [0x80000b40] : None -- Store: [0x80003228]:0x000000003598f81d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x10', 'rd : x8', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000b34]:sm3p0
	-[0x80000b38]:xori
	-[0x80000b3c]:sd
Current Store : [0x80000b44] : None -- Store: [0x80003230]:0xffffffffca6707e2




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x10', 'rd : x8', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000b7c]:sm3p0
	-[0x80000b80]:add
	-[0x80000b84]:sd
Current Store : [0x80000b88] : None -- Store: [0x80003240]:0x00000000c7d83fb2




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x10', 'rd : x8', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000b7c]:sm3p0
	-[0x80000b80]:add
	-[0x80000b84]:sd
Current Store : [0x80000b8c] : None -- Store: [0x80003248]:0x1011eeb547d0629f




Last Coverpoint : ['rs1 : x11', 'rd : x9']
Last Code Sequence : 
	-[0x80000bd4]:sm3p0
	-[0x80000bd8]:xor
	-[0x80000bdc]:sd
Current Store : [0x80000be0] : None -- Store: [0x80003258]:0x0000000021eaf76a




Last Coverpoint : ['rs1 : x11', 'rd : x9']
Last Code Sequence : 
	-[0x80000bd4]:sm3p0
	-[0x80000bd8]:xor
	-[0x80000bdc]:sd
Current Store : [0x80000be4] : None -- Store: [0x80003260]:0x70fc1afcaee2b1c8




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x11', 'rd : x9', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000c2c]:sm3p0
	-[0x80000c30]:xori
	-[0x80000c34]:sd
Current Store : [0x80000c38] : None -- Store: [0x80003270]:0x00000000ed3fe253




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x11', 'rd : x9', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000c2c]:sm3p0
	-[0x80000c30]:xori
	-[0x80000c34]:sd
Current Store : [0x80000c3c] : None -- Store: [0x80003278]:0xffffffff12c01dac




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x11', 'rd : x9', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000c84]:sm3p0
	-[0x80000c88]:add
	-[0x80000c8c]:sd
Current Store : [0x80000c90] : None -- Store: [0x80003288]:0x00000000c37b2f6d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x11', 'rd : x9', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000c84]:sm3p0
	-[0x80000c88]:add
	-[0x80000c8c]:sd
Current Store : [0x80000c94] : None -- Store: [0x80003290]:0x70fc1afd5283760f




Last Coverpoint : ['rs1 : x12', 'rd : x10']
Last Code Sequence : 
	-[0x80000cdc]:sm3p0
	-[0x80000ce0]:xor
	-[0x80000ce4]:sd
Current Store : [0x80000ce8] : None -- Store: [0x800032a0]:0x0000000016d354f1




Last Coverpoint : ['rs1 : x12', 'rd : x10']
Last Code Sequence : 
	-[0x80000cdc]:sm3p0
	-[0x80000ce0]:xor
	-[0x80000ce4]:sd
Current Store : [0x80000cec] : None -- Store: [0x800032a8]:0x72745307fae10a1d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x12', 'rd : x10', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000d34]:sm3p0
	-[0x80000d38]:xori
	-[0x80000d3c]:sd
Current Store : [0x80000d40] : None -- Store: [0x800032b8]:0x00000000caa9a0af




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x12', 'rd : x10', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000d34]:sm3p0
	-[0x80000d38]:xori
	-[0x80000d3c]:sd
Current Store : [0x80000d44] : None -- Store: [0x800032c0]:0xffffffff35565f50




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x12', 'rd : x10', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000d8c]:sm3p0
	-[0x80000d90]:add
	-[0x80000d94]:sd
Current Store : [0x80000d98] : None -- Store: [0x800032d0]:0x000000001618e87a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x12', 'rd : x10', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000d8c]:sm3p0
	-[0x80000d90]:add
	-[0x80000d94]:sd
Current Store : [0x80000d9c] : None -- Store: [0x800032d8]:0x72745308024b4766




Last Coverpoint : ['rs1 : x13', 'rd : x11']
Last Code Sequence : 
	-[0x80000ddc]:sm3p0
	-[0x80000de0]:xor
	-[0x80000de4]:sd
Current Store : [0x80000de8] : None -- Store: [0x800032e8]:0x000000009f278254




Last Coverpoint : ['rs1 : x13', 'rd : x11']
Last Code Sequence : 
	-[0x80000ddc]:sm3p0
	-[0x80000de0]:xor
	-[0x80000de4]:sd
Current Store : [0x80000dec] : None -- Store: [0x800032f0]:0xcebe24d9994785c6




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x13', 'rd : x11', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000e2c]:sm3p0
	-[0x80000e30]:xori
	-[0x80000e34]:sd
Current Store : [0x80000e38] : None -- Store: [0x80003300]:0x0000000036b4d0a1




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x13', 'rd : x11', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000e2c]:sm3p0
	-[0x80000e30]:xori
	-[0x80000e34]:sd
Current Store : [0x80000e3c] : None -- Store: [0x80003308]:0xffffffffc94b2f5e




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x13', 'rd : x11', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000e7c]:sm3p0
	-[0x80000e80]:add
	-[0x80000e84]:sd
Current Store : [0x80000e88] : None -- Store: [0x80003318]:0x0000000087b79b45




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x13', 'rd : x11', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000e7c]:sm3p0
	-[0x80000e80]:add
	-[0x80000e84]:sd
Current Store : [0x80000e8c] : None -- Store: [0x80003320]:0xcebe24d98e17a2d7




Last Coverpoint : ['rs1 : x14', 'rd : x12']
Last Code Sequence : 
	-[0x80000ed4]:sm3p0
	-[0x80000ed8]:xor
	-[0x80000edc]:sd
Current Store : [0x80000ee0] : None -- Store: [0x80003330]:0x000000002a696319




Last Coverpoint : ['rs1 : x14', 'rd : x12']
Last Code Sequence : 
	-[0x80000ed4]:sm3p0
	-[0x80000ed8]:xor
	-[0x80000edc]:sd
Current Store : [0x80000ee4] : None -- Store: [0x80003338]:0xab8534c103cb3446




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x14', 'rd : x12', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000f2c]:sm3p0
	-[0x80000f30]:xori
	-[0x80000f34]:sd
Current Store : [0x80000f38] : None -- Store: [0x80003348]:0x000000003c4d45b7




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x14', 'rd : x12', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000f2c]:sm3p0
	-[0x80000f30]:xori
	-[0x80000f34]:sd
Current Store : [0x80000f3c] : None -- Store: [0x80003350]:0xffffffffc3b2ba48




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x14', 'rd : x12', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000f84]:sm3p0
	-[0x80000f88]:add
	-[0x80000f8c]:sd
Current Store : [0x80000f90] : None -- Store: [0x80003360]:0x00000000bcb811da




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x14', 'rd : x12', 'rs1 != rd']
Last Code Sequence : 
	-[0x80000f84]:sm3p0
	-[0x80000f88]:add
	-[0x80000f8c]:sd
Current Store : [0x80000f94] : None -- Store: [0x80003368]:0xab8534c1e65a6939




Last Coverpoint : ['rs1 : x15', 'rd : x13']
Last Code Sequence : 
	-[0x80000fd4]:sm3p0
	-[0x80000fd8]:xor
	-[0x80000fdc]:sd
Current Store : [0x80000fe0] : None -- Store: [0x80003378]:0x000000006ecaf90b




Last Coverpoint : ['rs1 : x15', 'rd : x13']
Last Code Sequence : 
	-[0x80000fd4]:sm3p0
	-[0x80000fd8]:xor
	-[0x80000fdc]:sd
Current Store : [0x80000fe4] : None -- Store: [0x80003380]:0x01fbbe93ce417df8




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x15', 'rd : x13', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001024]:sm3p0
	-[0x80001028]:xori
	-[0x8000102c]:sd
Current Store : [0x80001030] : None -- Store: [0x80003390]:0x00000000419add5a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x15', 'rd : x13', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001024]:sm3p0
	-[0x80001028]:xori
	-[0x8000102c]:sd
Current Store : [0x80001034] : None -- Store: [0x80003398]:0xffffffffbe6522a5




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x15', 'rd : x13', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001074]:sm3p0
	-[0x80001078]:add
	-[0x8000107c]:sd
Current Store : [0x80001080] : None -- Store: [0x800033a8]:0x0000000062ccf907




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x15', 'rd : x13', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001074]:sm3p0
	-[0x80001078]:add
	-[0x8000107c]:sd
Current Store : [0x80001084] : None -- Store: [0x800033b0]:0x01fbbe9403587dfa




Last Coverpoint : ['rs1 : x16', 'rd : x14']
Last Code Sequence : 
	-[0x800010cc]:sm3p0
	-[0x800010d0]:xor
	-[0x800010d4]:sd
Current Store : [0x800010d8] : None -- Store: [0x800033c0]:0x00000000ce0555d4




Last Coverpoint : ['rs1 : x16', 'rd : x14']
Last Code Sequence : 
	-[0x800010cc]:sm3p0
	-[0x800010d0]:xor
	-[0x800010d4]:sd
Current Store : [0x800010dc] : None -- Store: [0x800033c8]:0x74f5add59232d14e




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x16', 'rd : x14', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001124]:sm3p0
	-[0x80001128]:xori
	-[0x8000112c]:sd
Current Store : [0x80001130] : None -- Store: [0x800033d8]:0x00000000c5f5f7b2




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x16', 'rd : x14', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001124]:sm3p0
	-[0x80001128]:xori
	-[0x8000112c]:sd
Current Store : [0x80001134] : None -- Store: [0x800033e0]:0xffffffff3a0a084d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x16', 'rd : x14', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000117c]:sm3p0
	-[0x80001180]:add
	-[0x80001184]:sd
Current Store : [0x80001188] : None -- Store: [0x800033f0]:0x000000006e2c460a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x16', 'rd : x14', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000117c]:sm3p0
	-[0x80001180]:add
	-[0x80001184]:sd
Current Store : [0x8000118c] : None -- Store: [0x800033f8]:0x74f5add5ca63caa4




Last Coverpoint : ['rs1 : x17', 'rd : x15']
Last Code Sequence : 
	-[0x800011d4]:sm3p0
	-[0x800011d8]:xor
	-[0x800011dc]:sd
Current Store : [0x800011e0] : None -- Store: [0x80003408]:0x00000000805e7c5c




Last Coverpoint : ['rs1 : x17', 'rd : x15']
Last Code Sequence : 
	-[0x800011d4]:sm3p0
	-[0x800011d8]:xor
	-[0x800011dc]:sd
Current Store : [0x800011e4] : None -- Store: [0x80003410]:0x9651ee65fa434f96




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x17', 'rd : x15', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000122c]:sm3p0
	-[0x80001230]:xori
	-[0x80001234]:sd
Current Store : [0x80001238] : None -- Store: [0x80003420]:0x00000000d811acfb




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x17', 'rd : x15', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000122c]:sm3p0
	-[0x80001230]:xori
	-[0x80001234]:sd
Current Store : [0x8000123c] : None -- Store: [0x80003428]:0xffffffff27ee5304




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x17', 'rd : x15', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001284]:sm3p0
	-[0x80001288]:add
	-[0x8000128c]:sd
Current Store : [0x80001290] : None -- Store: [0x80003438]:0x0000000047170df0




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x17', 'rd : x15', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001284]:sm3p0
	-[0x80001288]:add
	-[0x8000128c]:sd
Current Store : [0x80001294] : None -- Store: [0x80003440]:0x9651ee65c13441ba




Last Coverpoint : ['rs1 : x18', 'rd : x16']
Last Code Sequence : 
	-[0x800012dc]:sm3p0
	-[0x800012e0]:xor
	-[0x800012e4]:sd
Current Store : [0x800012e8] : None -- Store: [0x80003450]:0x0000000093a515fb




Last Coverpoint : ['rs1 : x18', 'rd : x16']
Last Code Sequence : 
	-[0x800012dc]:sm3p0
	-[0x800012e0]:xor
	-[0x800012e4]:sd
Current Store : [0x800012ec] : None -- Store: [0x80003458]:0x9b11d383dbe3540e




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x18', 'rd : x16', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001334]:sm3p0
	-[0x80001338]:xori
	-[0x8000133c]:sd
Current Store : [0x80001340] : None -- Store: [0x80003468]:0x00000000b8d0c416




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x18', 'rd : x16', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001334]:sm3p0
	-[0x80001338]:xori
	-[0x8000133c]:sd
Current Store : [0x80001344] : None -- Store: [0x80003470]:0xffffffff472f3be9




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x18', 'rd : x16', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000138c]:sm3p0
	-[0x80001390]:add
	-[0x80001394]:sd
Current Store : [0x80001398] : None -- Store: [0x80003480]:0x00000000055b6f1c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x18', 'rd : x16', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000138c]:sm3p0
	-[0x80001390]:add
	-[0x80001394]:sd
Current Store : [0x8000139c] : None -- Store: [0x80003488]:0x9b11d3834da1b111




Last Coverpoint : ['rs1 : x19', 'rd : x17']
Last Code Sequence : 
	-[0x800013e4]:sm3p0
	-[0x800013e8]:xor
	-[0x800013ec]:sd
Current Store : [0x800013f0] : None -- Store: [0x80003498]:0x0000000053c6e100




Last Coverpoint : ['rs1 : x19', 'rd : x17']
Last Code Sequence : 
	-[0x800013e4]:sm3p0
	-[0x800013e8]:xor
	-[0x800013ec]:sd
Current Store : [0x800013f4] : None -- Store: [0x800034a0]:0x93017690b090b39c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x19', 'rd : x17', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000143c]:sm3p0
	-[0x80001440]:xori
	-[0x80001444]:sd
Current Store : [0x80001448] : None -- Store: [0x800034b0]:0x0000000015355209




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x19', 'rd : x17', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000143c]:sm3p0
	-[0x80001440]:xori
	-[0x80001444]:sd
Current Store : [0x8000144c] : None -- Store: [0x800034b8]:0xffffffffeacaadf6




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x19', 'rd : x17', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001494]:sm3p0
	-[0x80001498]:add
	-[0x8000149c]:sd
Current Store : [0x800014a0] : None -- Store: [0x800034c8]:0x00000000658a6ede




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x19', 'rd : x17', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001494]:sm3p0
	-[0x80001498]:add
	-[0x8000149c]:sd
Current Store : [0x800014a4] : None -- Store: [0x800034d0]:0x9301769148e0c17a




Last Coverpoint : ['rs1 : x20', 'rd : x18']
Last Code Sequence : 
	-[0x800014ec]:sm3p0
	-[0x800014f0]:xor
	-[0x800014f4]:sd
Current Store : [0x800014f8] : None -- Store: [0x800034e0]:0x00000000f057d6a2




Last Coverpoint : ['rs1 : x20', 'rd : x18']
Last Code Sequence : 
	-[0x800014ec]:sm3p0
	-[0x800014f0]:xor
	-[0x800014f4]:sd
Current Store : [0x800014fc] : None -- Store: [0x800034e8]:0xc5d09b94dbb50e6b




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x20', 'rd : x18', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001544]:sm3p0
	-[0x80001548]:xori
	-[0x8000154c]:sd
Current Store : [0x80001550] : None -- Store: [0x800034f8]:0x00000000a03ee2a4




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x20', 'rd : x18', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001544]:sm3p0
	-[0x80001548]:xori
	-[0x8000154c]:sd
Current Store : [0x80001554] : None -- Store: [0x80003500]:0xffffffff5fc11d5b




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x20', 'rd : x18', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000159c]:sm3p0
	-[0x800015a0]:add
	-[0x800015a4]:sd
Current Store : [0x800015a8] : None -- Store: [0x80003510]:0x00000000fc9ae6cd




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x20', 'rd : x18', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000159c]:sm3p0
	-[0x800015a0]:add
	-[0x800015a4]:sd
Current Store : [0x800015ac] : None -- Store: [0x80003518]:0xc5d09b95287dbf96




Last Coverpoint : ['rs1 : x21', 'rd : x19']
Last Code Sequence : 
	-[0x800015ec]:sm3p0
	-[0x800015f0]:xor
	-[0x800015f4]:sd
Current Store : [0x800015f8] : None -- Store: [0x80003528]:0x000000000c3db6ef




Last Coverpoint : ['rs1 : x21', 'rd : x19']
Last Code Sequence : 
	-[0x800015ec]:sm3p0
	-[0x800015f0]:xor
	-[0x800015f4]:sd
Current Store : [0x800015fc] : None -- Store: [0x80003530]:0x18d71be43dfdb39f




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x21', 'rd : x19', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000163c]:sm3p0
	-[0x80001640]:xori
	-[0x80001644]:sd
Current Store : [0x80001648] : None -- Store: [0x80003540]:0x0000000044d5796c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x21', 'rd : x19', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000163c]:sm3p0
	-[0x80001640]:xori
	-[0x80001644]:sd
Current Store : [0x8000164c] : None -- Store: [0x80003548]:0xffffffffbb2a8693




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x21', 'rd : x19', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000168c]:sm3p0
	-[0x80001690]:add
	-[0x80001694]:sd
Current Store : [0x80001698] : None -- Store: [0x80003558]:0x000000007c0a4200




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x21', 'rd : x19', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000168c]:sm3p0
	-[0x80001690]:add
	-[0x80001694]:sd
Current Store : [0x8000169c] : None -- Store: [0x80003560]:0x18d71be4adca4770




Last Coverpoint : ['rs1 : x22', 'rd : x20']
Last Code Sequence : 
	-[0x800016e4]:sm3p0
	-[0x800016e8]:xor
	-[0x800016ec]:sd
Current Store : [0x800016f0] : None -- Store: [0x80003570]:0x0000000027b2bd68




Last Coverpoint : ['rs1 : x22', 'rd : x20']
Last Code Sequence : 
	-[0x800016e4]:sm3p0
	-[0x800016e8]:xor
	-[0x800016ec]:sd
Current Store : [0x800016f4] : None -- Store: [0x80003578]:0x2a5dc0a02af781b7




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x22', 'rd : x20', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000173c]:sm3p0
	-[0x80001740]:xori
	-[0x80001744]:sd
Current Store : [0x80001748] : None -- Store: [0x80003588]:0x00000000017d67b0




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x22', 'rd : x20', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000173c]:sm3p0
	-[0x80001740]:xori
	-[0x80001744]:sd
Current Store : [0x8000174c] : None -- Store: [0x80003590]:0xfffffffffe82984f




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x22', 'rd : x20', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001794]:sm3p0
	-[0x80001798]:add
	-[0x8000179c]:sd
Current Store : [0x800017a0] : None -- Store: [0x800035a0]:0x00000000f5bbcef3




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x22', 'rd : x20', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001794]:sm3p0
	-[0x80001798]:add
	-[0x8000179c]:sd
Current Store : [0x800017a4] : None -- Store: [0x800035a8]:0x2a5dc0a103010bd2




Last Coverpoint : ['rs1 : x23', 'rd : x21']
Last Code Sequence : 
	-[0x800017e4]:sm3p0
	-[0x800017e8]:xor
	-[0x800017ec]:sd
Current Store : [0x800017f0] : None -- Store: [0x800035b8]:0x000000004efcfa29




Last Coverpoint : ['rs1 : x23', 'rd : x21']
Last Code Sequence : 
	-[0x800017e4]:sm3p0
	-[0x800017e8]:xor
	-[0x800017ec]:sd
Current Store : [0x800017f4] : None -- Store: [0x800035c0]:0xc2713ce21694ea72




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x23', 'rd : x21', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001834]:sm3p0
	-[0x80001838]:xori
	-[0x8000183c]:sd
Current Store : [0x80001840] : None -- Store: [0x800035d0]:0x000000005701e9c4




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x23', 'rd : x21', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001834]:sm3p0
	-[0x80001838]:xori
	-[0x8000183c]:sd
Current Store : [0x80001844] : None -- Store: [0x800035d8]:0xffffffffa8fe163b




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x23', 'rd : x21', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001884]:sm3p0
	-[0x80001888]:add
	-[0x8000188c]:sd
Current Store : [0x80001890] : None -- Store: [0x800035e8]:0x00000000b08f7621




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x23', 'rd : x21', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001884]:sm3p0
	-[0x80001888]:add
	-[0x8000188c]:sd
Current Store : [0x80001894] : None -- Store: [0x800035f0]:0xc2713ce308f7867c




Last Coverpoint : ['rs1 : x24', 'rd : x22']
Last Code Sequence : 
	-[0x800018dc]:sm3p0
	-[0x800018e0]:xor
	-[0x800018e4]:sd
Current Store : [0x800018e8] : None -- Store: [0x80003600]:0x000000005a7104dd




Last Coverpoint : ['rs1 : x24', 'rd : x22']
Last Code Sequence : 
	-[0x800018dc]:sm3p0
	-[0x800018e0]:xor
	-[0x800018e4]:sd
Current Store : [0x800018ec] : None -- Store: [0x80003608]:0x9ea76f08dfe48c5c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x24', 'rd : x22', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001934]:sm3p0
	-[0x80001938]:xori
	-[0x8000193c]:sd
Current Store : [0x80001940] : None -- Store: [0x80003618]:0x0000000040787f5e




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x24', 'rd : x22', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001934]:sm3p0
	-[0x80001938]:xori
	-[0x8000193c]:sd
Current Store : [0x80001944] : None -- Store: [0x80003620]:0xffffffffbf8780a1




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x24', 'rd : x22', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000198c]:sm3p0
	-[0x80001990]:add
	-[0x80001994]:sd
Current Store : [0x80001998] : None -- Store: [0x80003630]:0x00000000bdb3131e




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x24', 'rd : x22', 'rs1 != rd']
Last Code Sequence : 
	-[0x8000198c]:sm3p0
	-[0x80001990]:add
	-[0x80001994]:sd
Current Store : [0x8000199c] : None -- Store: [0x80003638]:0x9ea76f0943489b9f




Last Coverpoint : ['rs1 : x25', 'rd : x23']
Last Code Sequence : 
	-[0x800019e4]:sm3p0
	-[0x800019e8]:xor
	-[0x800019ec]:sd
Current Store : [0x800019f0] : None -- Store: [0x80003648]:0x000000009a2cbad8




Last Coverpoint : ['rs1 : x25', 'rd : x23']
Last Code Sequence : 
	-[0x800019e4]:sm3p0
	-[0x800019e8]:xor
	-[0x800019ec]:sd
Current Store : [0x800019f4] : None -- Store: [0x80003650]:0x132a71769c827b88




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x25', 'rd : x23', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001a3c]:sm3p0
	-[0x80001a40]:xori
	-[0x80001a44]:sd
Current Store : [0x80001a48] : None -- Store: [0x80003660]:0x00000000267393ff




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x25', 'rd : x23', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001a3c]:sm3p0
	-[0x80001a40]:xori
	-[0x80001a44]:sd
Current Store : [0x80001a4c] : None -- Store: [0x80003668]:0xffffffffd98c6c00




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x25', 'rd : x23', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001a94]:sm3p0
	-[0x80001a98]:add
	-[0x80001a9c]:sd
Current Store : [0x80001aa0] : None -- Store: [0x80003678]:0x000000001d216c6b




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x25', 'rd : x23', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001a94]:sm3p0
	-[0x80001a98]:add
	-[0x80001a9c]:sd
Current Store : [0x80001aa4] : None -- Store: [0x80003680]:0x132a717623d02dbb




Last Coverpoint : ['rs1 : x26', 'rd : x24']
Last Code Sequence : 
	-[0x80001aec]:sm3p0
	-[0x80001af0]:xor
	-[0x80001af4]:sd
Current Store : [0x80001af8] : None -- Store: [0x80003690]:0x000000003d97f659




Last Coverpoint : ['rs1 : x26', 'rd : x24']
Last Code Sequence : 
	-[0x80001aec]:sm3p0
	-[0x80001af0]:xor
	-[0x80001af4]:sd
Current Store : [0x80001afc] : None -- Store: [0x80003698]:0x339863c4ef8118f1




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x26', 'rd : x24', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001b44]:sm3p0
	-[0x80001b48]:xori
	-[0x80001b4c]:sd
Current Store : [0x80001b50] : None -- Store: [0x800036a8]:0x00000000dd65e4de




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x26', 'rd : x24', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001b44]:sm3p0
	-[0x80001b48]:xori
	-[0x80001b4c]:sd
Current Store : [0x80001b54] : None -- Store: [0x800036b0]:0xffffffff229a1b21




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x26', 'rd : x24', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001b9c]:sm3p0
	-[0x80001ba0]:add
	-[0x80001ba4]:sd
Current Store : [0x80001ba8] : None -- Store: [0x800036c0]:0x00000000b0d48362




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x26', 'rd : x24', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001b9c]:sm3p0
	-[0x80001ba0]:add
	-[0x80001ba4]:sd
Current Store : [0x80001bac] : None -- Store: [0x800036c8]:0x339863c582eb720a




Last Coverpoint : ['rs1 : x27', 'rd : x25']
Last Code Sequence : 
	-[0x80001bf4]:sm3p0
	-[0x80001bf8]:xor
	-[0x80001bfc]:sd
Current Store : [0x80001c00] : None -- Store: [0x800036d8]:0x00000000c222016f




Last Coverpoint : ['rs1 : x27', 'rd : x25']
Last Code Sequence : 
	-[0x80001bf4]:sm3p0
	-[0x80001bf8]:xor
	-[0x80001bfc]:sd
Current Store : [0x80001c04] : None -- Store: [0x800036e0]:0x2d885062388b780a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x27', 'rd : x25', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001c4c]:sm3p0
	-[0x80001c50]:xori
	-[0x80001c54]:sd
Current Store : [0x80001c58] : None -- Store: [0x800036f0]:0x00000000a56fb83d




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x27', 'rd : x25', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001c4c]:sm3p0
	-[0x80001c50]:xori
	-[0x80001c54]:sd
Current Store : [0x80001c5c] : None -- Store: [0x800036f8]:0xffffffff5a9047c2




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x27', 'rd : x25', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001ca4]:sm3p0
	-[0x80001ca8]:add
	-[0x80001cac]:sd
Current Store : [0x80001cb0] : None -- Store: [0x80003708]:0x00000000dbc50c90




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x27', 'rd : x25', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001ca4]:sm3p0
	-[0x80001ca8]:add
	-[0x80001cac]:sd
Current Store : [0x80001cb4] : None -- Store: [0x80003710]:0x2d885063d66e85f5




Last Coverpoint : ['rs1 : x28', 'rd : x26']
Last Code Sequence : 
	-[0x80001cfc]:sm3p0
	-[0x80001d00]:xor
	-[0x80001d04]:sd
Current Store : [0x80001d08] : None -- Store: [0x80003720]:0x00000000afb4b213




Last Coverpoint : ['rs1 : x28', 'rd : x26']
Last Code Sequence : 
	-[0x80001cfc]:sm3p0
	-[0x80001d00]:xor
	-[0x80001d04]:sd
Current Store : [0x80001d0c] : None -- Store: [0x80003728]:0xb3e73cbba236ead7




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x28', 'rd : x26', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001d54]:sm3p0
	-[0x80001d58]:xori
	-[0x80001d5c]:sd
Current Store : [0x80001d60] : None -- Store: [0x80003738]:0x0000000047443424




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x28', 'rd : x26', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001d54]:sm3p0
	-[0x80001d58]:xori
	-[0x80001d5c]:sd
Current Store : [0x80001d64] : None -- Store: [0x80003740]:0xffffffffb8bbcbdb




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x28', 'rd : x26', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001dac]:sm3p0
	-[0x80001db0]:add
	-[0x80001db4]:sd
Current Store : [0x80001db8] : None -- Store: [0x80003750]:0x0000000070726122




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x28', 'rd : x26', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001dac]:sm3p0
	-[0x80001db0]:add
	-[0x80001db4]:sd
Current Store : [0x80001dbc] : None -- Store: [0x80003758]:0xb3e73cbb7df4b9e6




Last Coverpoint : ['rs1 : x29', 'rd : x27']
Last Code Sequence : 
	-[0x80001dfc]:sm3p0
	-[0x80001e00]:xor
	-[0x80001e04]:sd
Current Store : [0x80001e08] : None -- Store: [0x80003768]:0x00000000d586d9ab




Last Coverpoint : ['rs1 : x29', 'rd : x27']
Last Code Sequence : 
	-[0x80001dfc]:sm3p0
	-[0x80001e00]:xor
	-[0x80001e04]:sd
Current Store : [0x80001e0c] : None -- Store: [0x80003770]:0x2d13320e95563c4c




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x29', 'rd : x27', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001e4c]:sm3p0
	-[0x80001e50]:xori
	-[0x80001e54]:sd
Current Store : [0x80001e58] : None -- Store: [0x80003780]:0x00000000d52a5538




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x29', 'rd : x27', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001e4c]:sm3p0
	-[0x80001e50]:xori
	-[0x80001e54]:sd
Current Store : [0x80001e5c] : None -- Store: [0x80003788]:0xffffffff2ad5aac7




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x29', 'rd : x27', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001e9c]:sm3p0
	-[0x80001ea0]:add
	-[0x80001ea4]:sd
Current Store : [0x80001ea8] : None -- Store: [0x80003798]:0x000000002d22065a




Last Coverpoint : ['opcode : sm3p0', 'rs1 : x29', 'rd : x27', 'rs1 != rd']
Last Code Sequence : 
	-[0x80001e9c]:sm3p0
	-[0x80001ea0]:add
	-[0x80001ea4]:sd
Current Store : [0x80001eac] : None -- Store: [0x800037a0]:0x2d13320e6df2ec41





```

## Details of STAT5:



## Details of STAT1:

- The first column indicates the signature address and the data at that location in hexadecimal in the following format: 
  ```
  [Address]
  Data
  ```

- The second column captures all the coverpoints which have been captured by that particular signature location

- The third column captures all the insrtuctions since the time a coverpoint was
  hit to the point when a store to the signature was performed. Each line has
  the following format:
  ```
  [PC of instruction] : mnemonic
  ```
- The order in the table is based on the order of signatures occuring in the
  test. These need not necessarily be in increasing or decreasing order of the
  address in the signature region.

|s.no|            signature             |                           coverpoints                            |                              code                              |
|---:|----------------------------------|------------------------------------------------------------------|----------------------------------------------------------------|
|   1|[0x80003010]<br>0x9baab409e9ce59bf|- opcode : sm3p0<br> - rs1 : x3<br> - rd : x1<br> - rs1 != rd<br> |[0x800003dc]:sm3p0<br> [0x800003e0]:xor<br> [0x800003e4]:sd<br> |
|   2|[0x80003058]<br>0x4f0e7329acf6b0ac|- rs1 : x4<br> - rd : x2<br>                                      |[0x800004dc]:sm3p0<br> [0x800004e0]:xor<br> [0x800004e4]:sd<br> |
|   3|[0x800030a0]<br>0xf346190085d9f49f|- rs1 : x5<br> - rd : x3<br>                                      |[0x800005d4]:sm3p0<br> [0x800005d8]:xor<br> [0x800005dc]:sd<br> |
|   4|[0x800030e8]<br>0xd5a6539a1515b62e|- rs1 : x6<br> - rd : x4<br>                                      |[0x800006dc]:sm3p0<br> [0x800006e0]:xor<br> [0x800006e4]:sd<br> |
|   5|[0x80003130]<br>0xbd7bb672b1a509ca|- rs1 : x7<br> - rd : x5<br>                                      |[0x800007e4]:sm3p0<br> [0x800007e8]:xor<br> [0x800007ec]:sd<br> |
|   6|[0x80003178]<br>0x3441a740c4490a21|- rs1 : x8<br> - rd : x6<br>                                      |[0x800008ec]:sm3p0<br> [0x800008f0]:xor<br> [0x800008f4]:sd<br> |
|   7|[0x800031c0]<br>0x58d5d905ee915c98|- rs1 : x9<br> - rd : x7<br>                                      |[0x800009f4]:sm3p0<br> [0x800009f8]:xor<br> [0x800009fc]:sd<br> |
|   8|[0x80003208]<br>0xf909502b81fd5f28|- rs1 : x10<br> - rd : x8<br>                                     |[0x80000aec]:sm3p0<br> [0x80000af0]:xor<br> [0x80000af4]:sd<br> |
|   9|[0x80003250]<br>0xc35a255ff261884d|- rs1 : x11<br> - rd : x9<br>                                     |[0x80000bd4]:sm3p0<br> [0x80000bd8]:xor<br> [0x80000bdc]:sd<br> |
|  10|[0x80003298]<br>0xbed9e518121290f0|- rs1 : x12<br> - rd : x10<br>                                    |[0x80000cdc]:sm3p0<br> [0x80000ce0]:xor<br> [0x80000ce4]:sd<br> |
|  11|[0x800032e0]<br>0x6e5e995fd235139a|- rs1 : x13<br> - rd : x11<br>                                    |[0x80000ddc]:sm3p0<br> [0x80000de0]:xor<br> [0x80000de4]:sd<br> |
|  12|[0x80003328]<br>0x7a9113e5d295e997|- rs1 : x14<br> - rd : x12<br>                                    |[0x80000ed4]:sm3p0<br> [0x80000ed8]:xor<br> [0x80000edc]:sd<br> |
|  13|[0x80003370]<br>0x990c7a8fe49adff7|- rs1 : x15<br> - rd : x13<br>                                    |[0x80000fd4]:sm3p0<br> [0x80000fd8]:xor<br> [0x80000fdc]:sd<br> |
|  14|[0x800033b8]<br>0x2de37f5452135d56|- rs1 : x16<br> - rd : x14<br>                                    |[0x800010cc]:sm3p0<br> [0x800010d0]:xor<br> [0x800010d4]:sd<br> |
|  15|[0x80003400]<br>0xd0bc9a3ac3e3c21c|- rs1 : x17<br> - rd : x15<br>                                    |[0x800011d4]:sm3p0<br> [0x800011d8]:xor<br> [0x800011dc]:sd<br> |
|  16|[0x80003448]<br>0x072cdbff2dc51a2a|- rs1 : x18<br> - rd : x16<br>                                    |[0x800012dc]:sm3p0<br> [0x800012e0]:xor<br> [0x800012e4]:sd<br> |
|  17|[0x80003490]<br>0x971acc3b74bd2e93|- rs1 : x19<br> - rd : x17<br>                                    |[0x800013e4]:sm3p0<br> [0x800013e8]:xor<br> [0x800013ec]:sd<br> |
|  18|[0x800034d8]<br>0x2ab7ea92f7f576a7|- rs1 : x20<br> - rd : x18<br>                                    |[0x800014ec]:sm3p0<br> [0x800014f0]:xor<br> [0x800014f4]:sd<br> |
|  19|[0x80003520]<br>0x6d8e7a4db287d885|- rs1 : x21<br> - rd : x19<br>                                    |[0x800015ec]:sm3p0<br> [0x800015f0]:xor<br> [0x800015f4]:sd<br> |
|  20|[0x80003568]<br>0xa57f886251704b2a|- rs1 : x22<br> - rd : x20<br>                                    |[0x800016e4]:sm3p0<br> [0x800016e8]:xor<br> [0x800016ec]:sd<br> |
|  21|[0x800035b0]<br>0xafb2f00c9b07ed10|- rs1 : x23<br> - rd : x21<br>                                    |[0x800017e4]:sm3p0<br> [0x800017e8]:xor<br> [0x800017ec]:sd<br> |
|  22|[0x800035f8]<br>0x7a9113c25ce4e7ad|- rs1 : x24<br> - rd : x22<br>                                    |[0x800018dc]:sm3p0<br> [0x800018e0]:xor<br> [0x800018e4]:sd<br> |
|  23|[0x80003640]<br>0x24eeb7cf939e1ac3|- rs1 : x25<br> - rd : x23<br>                                    |[0x800019e4]:sm3p0<br> [0x800019e8]:xor<br> [0x800019ec]:sd<br> |
|  24|[0x80003688]<br>0x374b8630f9da381e|- rs1 : x26<br> - rd : x24<br>                                    |[0x80001aec]:sm3p0<br> [0x80001af0]:xor<br> [0x80001af4]:sd<br> |
|  25|[0x800036d0]<br>0xfb24d57dfdbc23ec|- rs1 : x27<br> - rd : x25<br>                                    |[0x80001bf4]:sm3p0<br> [0x80001bf8]:xor<br> [0x80001bfc]:sd<br> |
|  26|[0x80003718]<br>0x3edc9bee01be696c|- rs1 : x28<br> - rd : x26<br>                                    |[0x80001cfc]:sm3p0<br> [0x80001d00]:xor<br> [0x80001d04]:sd<br> |
|  27|[0x80003760]<br>0x0e8b61f752df1cb0|- rs1 : x29<br> - rd : x27<br>                                    |[0x80001dfc]:sm3p0<br> [0x80001e00]:xor<br> [0x80001e04]:sd<br> |