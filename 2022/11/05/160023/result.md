# Benchmark result

* Pull request commit: [`29606cbc5688148e013e1f436ac5ce2fa32c1a6e`](https://github.com/TensorBFS/TensorInference.jl/commit/29606cbc5688148e013e1f436ac5ce2fa32c1a6e)
* Pull request: <https://github.com/TensorBFS/TensorInference.jl/pull/19> (Run benchmarks in CI and push results to TensorBFS/TensorInference-data)

# Judge result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmarks:
    - Target: 5 Nov 2022 - 15:59
    - Baseline: 5 Nov 2022 - 15:59
* Package commits:
    - Target: 6026c4
    - Baseline: ab5b04
* Julia commits:
    - Target: 36034a
    - Baseline: 36034a
* Julia command flags:
    - Target: None
    - Baseline: None
* Environment variables:
    - Target: None
    - Baseline: None

## Results
A ratio greater than `1.0` denotes a possible regression (marked with :x:), while a ratio less
than `1.0` denotes a possible improvement (marked with :white_check_mark:). Only significant results - results
that indicate possible regressions or improvements - are shown below (thus, an empty table means that all
benchmark results remained invariant between builds).

| ID | time ratio | memory ratio |
|----|------------|--------------|

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:


## Julia versioninfo

### Target
```
Julia Version 1.8.2
Commit 36034abf260 (2022-09-29 15:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 20.04.5 LTS
  uname: Linux 5.15.0-1022-azure #27~20.04.1-Ubuntu SMP Mon Oct 17 02:03:50 UTC 2022 x86_64 x86_64
  CPU: Intel(R) Xeon(R) Platinum 8272CL CPU @ 2.60GHz: 
              speed         user         nice          sys         idle          irq
       #1  2593 MHz       2208 s          2 s        197 s       3451 s          0 s
       #2  2593 MHz       1225 s          0 s        184 s       4470 s          0 s
  Memory: 6.78125 GB (5016.171875 MB free)
  Uptime: 595.35 sec
  Load Avg:  1.02  0.81  0.4
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-13.0.1 (ORCJIT, skylake-avx512)
  Threads: 1 on 2 virtual cores
```

### Baseline
```
Julia Version 1.8.2
Commit 36034abf260 (2022-09-29 15:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 20.04.5 LTS
  uname: Linux 5.15.0-1022-azure #27~20.04.1-Ubuntu SMP Mon Oct 17 02:03:50 UTC 2022 x86_64 x86_64
  CPU: Intel(R) Xeon(R) Platinum 8272CL CPU @ 2.60GHz: 
              speed         user         nice          sys         idle          irq
       #1  2593 MHz       2251 s          2 s        202 s       3572 s          0 s
       #2  2593 MHz       1348 s          0 s        189 s       4513 s          0 s
  Memory: 6.78125 GB (5411.0078125 MB free)
  Uptime: 612.38 sec
  Load Avg:  1.01  0.82  0.41
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-13.0.1 (ORCJIT, skylake-avx512)
  Threads: 1 on 2 virtual cores
```

---
# Target result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmark: 5 Nov 2022 - 15:59
* Package commit: 6026c4
* Julia commit: 36034a
* Julia command flags: None
* Environment variables: None

## Results
Below is a table of this job's results, obtained by running the benchmarks.
The values listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`, and can be used to
index into the BaseBenchmarks suite to retrieve the corresponding benchmarks.
The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.
An empty cell means that the value was zero.

| ID                   | time            | GC time    | memory         | allocations |
|----------------------|----------------:|-----------:|---------------:|------------:|
| `["map", "map"]`     | 257.285 ms (5%) |   8.025 ms | 91.14 MiB (1%) |      158842 |
| `["mar", "mar"]`     |  58.910 ms (5%) |            | 34.74 MiB (1%) |      182389 |
| `["mmap", "mmap-1"]` | 140.855 ms (5%) |            | 35.84 MiB (1%) |       78690 |
| `["mmap", "mmap-2"]` |    2.879 s (5%) | 210.814 ms |  1.59 GiB (1%) |       81587 |
| `["mmap", "mmap-3"]` | 383.685 ms (5%) |   8.282 ms | 77.52 MiB (1%) |      156765 |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["map"]`
- `["mar"]`
- `["mmap"]`

## Julia versioninfo
```
Julia Version 1.8.2
Commit 36034abf260 (2022-09-29 15:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 20.04.5 LTS
  uname: Linux 5.15.0-1022-azure #27~20.04.1-Ubuntu SMP Mon Oct 17 02:03:50 UTC 2022 x86_64 x86_64
  CPU: Intel(R) Xeon(R) Platinum 8272CL CPU @ 2.60GHz: 
              speed         user         nice          sys         idle          irq
       #1  2593 MHz       2208 s          2 s        197 s       3451 s          0 s
       #2  2593 MHz       1225 s          0 s        184 s       4470 s          0 s
  Memory: 6.78125 GB (5016.171875 MB free)
  Uptime: 595.35 sec
  Load Avg:  1.02  0.81  0.4
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-13.0.1 (ORCJIT, skylake-avx512)
  Threads: 1 on 2 virtual cores
```

---
# Baseline result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmark: 5 Nov 2022 - 15:59
* Package commit: ab5b04
* Julia commit: 36034a
* Julia command flags: None
* Environment variables: None

## Results
Below is a table of this job's results, obtained by running the benchmarks.
The values listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`, and can be used to
index into the BaseBenchmarks suite to retrieve the corresponding benchmarks.
The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.
An empty cell means that the value was zero.

| ID                      | time           | GC time | memory         | allocations |
|-------------------------|---------------:|--------:|---------------:|------------:|
| `["marginals", "test"]` | 47.871 ms (5%) |         | 15.76 MiB (1%) |           7 |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["marginals"]`

## Julia versioninfo
```
Julia Version 1.8.2
Commit 36034abf260 (2022-09-29 15:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 20.04.5 LTS
  uname: Linux 5.15.0-1022-azure #27~20.04.1-Ubuntu SMP Mon Oct 17 02:03:50 UTC 2022 x86_64 x86_64
  CPU: Intel(R) Xeon(R) Platinum 8272CL CPU @ 2.60GHz: 
              speed         user         nice          sys         idle          irq
       #1  2593 MHz       2251 s          2 s        202 s       3572 s          0 s
       #2  2593 MHz       1348 s          0 s        189 s       4513 s          0 s
  Memory: 6.78125 GB (5411.0078125 MB free)
  Uptime: 612.38 sec
  Load Avg:  1.01  0.82  0.41
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-13.0.1 (ORCJIT, skylake-avx512)
  Threads: 1 on 2 virtual cores
```

---
# Runtime information
| Runtime Info | |
|:--|:--|
| BLAS #threads | 1 |
| `BLAS.vendor()` | `openblas64` |
| `Sys.CPU_THREADS` | 2 |

`lscpu` output:

    Architecture:                    x86_64
    CPU op-mode(s):                  32-bit, 64-bit
    Byte Order:                      Little Endian
    Address sizes:                   46 bits physical, 48 bits virtual
    CPU(s):                          2
    On-line CPU(s) list:             0,1
    Thread(s) per core:              1
    Core(s) per socket:              2
    Socket(s):                       1
    NUMA node(s):                    1
    Vendor ID:                       GenuineIntel
    CPU family:                      6
    Model:                           85
    Model name:                      Intel(R) Xeon(R) Platinum 8272CL CPU @ 2.60GHz
    Stepping:                        7
    CPU MHz:                         2593.905
    BogoMIPS:                        5187.81
    Hypervisor vendor:               Microsoft
    Virtualization type:             full
    L1d cache:                       64 KiB
    L1i cache:                       64 KiB
    L2 cache:                        2 MiB
    L3 cache:                        35.8 MiB
    NUMA node0 CPU(s):               0,1
    Vulnerability Itlb multihit:     KVM: Mitigation: VMX unsupported
    Vulnerability L1tf:              Mitigation; PTE Inversion
    Vulnerability Mds:               Mitigation; Clear CPU buffers; SMT Host state unknown
    Vulnerability Meltdown:          Mitigation; PTI
    Vulnerability Mmio stale data:   Vulnerable: Clear CPU buffers attempted, no microcode; SMT Host state unknown
    Vulnerability Retbleed:          Vulnerable
    Vulnerability Spec store bypass: Vulnerable
    Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
    Vulnerability Spectre v2:        Mitigation; Retpolines, STIBP disabled, RSB filling, PBRSB-eIBRS Not affected
    Vulnerability Srbds:             Not affected
    Vulnerability Tsx async abort:   Mitigation; Clear CPU buffers; SMT Host state unknown
    Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl xtopology cpuid pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 movbe popcnt aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single pti fsgsbase bmi1 hle avx2 smep bmi2 erms invpcid rtm avx512f avx512dq rdseed adx smap clflushopt avx512cd avx512bw avx512vl xsaveopt xsavec xsaves md_clear
    

| Cpu Property       | Value                                                   |
|:------------------ |:------------------------------------------------------- |
| Brand              | Intel(R) Xeon(R) Platinum 8272CL CPU @ 2.60GHz          |
| Vendor             | :Intel                                                  |
| Architecture       | :Skylake                                                |
| Model              | Family: 0x06, Model: 0x55, Stepping: 0x07, Type: 0x00   |
| Cores              | 2 physical cores, 2 logical cores (on executing CPU)    |
|                    | No Hyperthreading hardware capability detected          |
| Clock Frequencies  | Not supported by CPU                                    |
| Data Cache         | Level 1:3 : (32, 1024, 36608) kbytes                    |
|                    | 64 byte cache line size                                 |
| Address Size       | 48 bits virtual, 46 bits physical                       |
| SIMD               | 512 bit = 64 byte max. SIMD vector size                 |
| Time Stamp Counter | TSC is accessible via `rdtsc`                           |
|                    | TSC increased at every clock cycle (non-invariant TSC)  |
| Perf. Monitoring   | Performance Monitoring Counters (PMC) are not supported |
| Hypervisor         | Yes, Microsoft                                          |

