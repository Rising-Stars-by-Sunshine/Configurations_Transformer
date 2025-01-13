# Configurations_Transformer

This repository contains system information and details about the CPU architecture and its features. The information below is useful for developers or researchers working with this specific environment.

## Architecture Overview

- **Architecture**: x86_64
- **CPU op-mode(s)**: 32-bit, 64-bit
- **Address sizes**: 46 bits physical, 48 bits virtual
- **Byte Order**: Little Endian

## CPU Details

- **CPU(s)**: 2
  - **On-line CPU(s) list**: 0,1
- **Vendor ID**: GenuineIntel
- **Model name**: Intel(R) Xeon(R) CPU @ 2.20GHz
- **CPU family**: 6
- **Model**: 79
- **Thread(s) per core**: 2
- **Core(s) per socket**: 1
- **Socket(s)**: 1
- **Stepping**: 0
- **BogoMIPS**: 4399.99

## Cache Details

- **L1d Cache**: 32 KiB (1 instance)
- **L1i Cache**: 32 KiB (1 instance)
- **L2 Cache**: 256 KiB (1 instance)
- **L3 Cache**: 55 MiB (1 instance)

## Virtualization

- **Hypervisor vendor**: KVM
- **Virtualization type**: full

## NUMA

- **NUMA node(s)**: 1
  - **NUMA node0 CPU(s)**: 0,1

## Flags

The following CPU flags are supported:
```
fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl xtopology nonstop_tsc cpuid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single ssbd ibrs ibpb stibp fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rtm rdseed adx smap xsaveopt arat md_clear arch_capabilities
```

## Vulnerabilities

The CPU is affected by several vulnerabilities, as shown below:

- **Gather data sampling**: Not affected
- **Itlb multihit**: Not affected
- **L1tf**: Mitigation; PTE Inversion
- **Mds**: Vulnerable; SMT Host state unknown
- **Meltdown**: Vulnerable
- **Mmio stale data**: Vulnerable
- **Reg file data sampling**: Not affected
- **Retbleed**: Vulnerable
- **Spec rstack overflow**: Not affected
- **Spec store bypass**: Vulnerable
- **Spectre v1**: Vulnerable: __user pointer sanitization and usercopy barriers only; no swapgs barriers
- **Spectre v2**: Vulnerable; IBPB: disabled; STIBP: disabled; PBRSB-eIBRS: Not affected; BHI: Vulnerable (Syscall hardening enabled)
- **Srbds**: Not affected
- **Tsx async abort**: Vulnerable

---

## Usage

This information can be used for:

1. Identifying potential security vulnerabilities.
2. Optimizing software for this specific CPU architecture.
3. Diagnosing performance-related issues in a virtualized environment.

---

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute as per the license terms.
