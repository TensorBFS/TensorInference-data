# Benchmark result

* Pull request commit: [`528e71a0d77ae1756cd54123421ffade2c07b272`](https://github.com/TensorBFS/TensorInference.jl/commit/528e71a0d77ae1756cd54123421ffade2c07b272)
* Pull request: <https://github.com/TensorBFS/TensorInference.jl/pull/25> (Use test/Project.toml in favor of [extras] in Project.toml)

# Judge result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmarks:
    - Target: 30 Jun 2023 - 03:59
    - Baseline: 30 Jun 2023 - 04:03
* Package commits:
    - Target: 9311f3
    - Baseline: 147f9d
* Julia commits:
    - Target: 147bdf
    - Baseline: 147bdf
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

| ID                   | time ratio                   | memory ratio                 |
|----------------------|------------------------------|------------------------------|
| `["map", "map"]`     | 0.80 (5%) :white_check_mark: |                   0.99 (1%)  |
| `["mar", "mar"]`     | 0.00 (5%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["mmap", "mmap-1"]` |                   0.96 (5%)  |                1.07 (1%) :x: |
| `["mmap", "mmap-2"]` | 0.00 (5%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["mmap", "mmap-3"]` | 0.00 (5%) :white_check_mark: | 0.01 (1%) :white_check_mark: |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["map"]`
- `["mar"]`
- `["mmap"]`

## Julia versioninfo

### Target
```
Julia Version 1.9.1
Commit 147bdf428cd (2023-06-07 08:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 22.04.2 LTS
  uname: Linux 5.15.0-1040-azure #47-Ubuntu SMP Thu Jun 1 19:38:24 UTC 2023 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz: 
              speed         user         nice          sys         idle          irq
       #1  2294 MHz       5416 s          0 s        309 s       1999 s          0 s
       #2  2294 MHz       2104 s          0 s        254 s       5326 s          0 s
  Memory: 6.7694854736328125 GB (4931.140625 MB free)
  Uptime: 782.24 sec
  Load Avg:  1.01  1.06  0.75
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, broadwell)
  Threads: 1 on 2 virtual cores
```

### Baseline
```
Julia Version 1.9.1
Commit 147bdf428cd (2023-06-07 08:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 22.04.2 LTS
  uname: Linux 5.15.0-1040-azure #47-Ubuntu SMP Thu Jun 1 19:38:24 UTC 2023 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz: 
              speed         user         nice          sys         idle          irq
       #1  2294 MHz       7453 s          0 s        324 s       2066 s          0 s
       #2  2294 MHz       2173 s          0 s        267 s       7355 s          0 s
  Memory: 6.7694854736328125 GB (4840.7109375 MB free)
  Uptime: 994.29 sec
  Load Avg:  1.0  1.02  0.81
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, broadwell)
  Threads: 1 on 2 virtual cores
```

---
# Target result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmark: 30 Jun 2023 - 3:59
* Package commit: 9311f3
* Julia commit: 147bdf
* Julia command flags: None
* Environment variables: None

## Results
Below is a table of this job's results, obtained by running the benchmarks.
The values listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`, and can be used to
index into the BaseBenchmarks suite to retrieve the corresponding benchmarks.
The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.
An empty cell means that the value was zero.

| ID                   | time            | GC time   | memory         | allocations |
|----------------------|----------------:|----------:|---------------:|------------:|
| `["map", "map"]`     | 173.220 ms (5%) | 12.518 ms | 61.42 MiB (1%) |      159599 |
| `["mar", "mar"]`     |  90.837 ms (5%) |           | 35.21 MiB (1%) |      171880 |
| `["mmap", "mmap-1"]` |  21.460 ms (5%) |           | 10.52 MiB (1%) |       42168 |
| `["mmap", "mmap-2"]` |  42.275 ms (5%) |           | 42.45 MiB (1%) |       44670 |
| `["mmap", "mmap-3"]` | 171.678 ms (5%) | 12.635 ms | 57.25 MiB (1%) |      156823 |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["map"]`
- `["mar"]`
- `["mmap"]`

## Julia versioninfo
```
Julia Version 1.9.1
Commit 147bdf428cd (2023-06-07 08:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 22.04.2 LTS
  uname: Linux 5.15.0-1040-azure #47-Ubuntu SMP Thu Jun 1 19:38:24 UTC 2023 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz: 
              speed         user         nice          sys         idle          irq
       #1  2294 MHz       5416 s          0 s        309 s       1999 s          0 s
       #2  2294 MHz       2104 s          0 s        254 s       5326 s          0 s
  Memory: 6.7694854736328125 GB (4931.140625 MB free)
  Uptime: 782.24 sec
  Load Avg:  1.01  1.06  0.75
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, broadwell)
  Threads: 1 on 2 virtual cores
```

---
# Baseline result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmark: 30 Jun 2023 - 4:3
* Package commit: 147f9d
* Julia commit: 147bdf
* Julia command flags: None
* Environment variables: None

## Results
Below is a table of this job's results, obtained by running the benchmarks.
The values listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`, and can be used to
index into the BaseBenchmarks suite to retrieve the corresponding benchmarks.
The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.
An empty cell means that the value was zero.

| ID                   | time            | GC time    | memory          | allocations |
|----------------------|----------------:|-----------:|----------------:|------------:|
| `["map", "map"]`     | 215.976 ms (5%) |  35.350 ms |  61.88 MiB (1%) |      157959 |
| `["mar", "mar"]`     |   34.757 s (5%) |    1.287 s |   2.37 GiB (1%) |    35573830 |
| `["mmap", "mmap-1"]` |  22.260 ms (5%) |            |   9.86 MiB (1%) |       42139 |
| `["mmap", "mmap-2"]` |   15.949 s (5%) | 330.477 ms | 828.78 MiB (1%) |    12062043 |
| `["mmap", "mmap-3"]` |   99.798 s (5%) |    3.384 s |   5.53 GiB (1%) |    95311908 |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["map"]`
- `["mar"]`
- `["mmap"]`

## Julia versioninfo
```
Julia Version 1.9.1
Commit 147bdf428cd (2023-06-07 08:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 22.04.2 LTS
  uname: Linux 5.15.0-1040-azure #47-Ubuntu SMP Thu Jun 1 19:38:24 UTC 2023 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz: 
              speed         user         nice          sys         idle          irq
       #1  2294 MHz       7453 s          0 s        324 s       2066 s          0 s
       #2  2294 MHz       2173 s          0 s        267 s       7355 s          0 s
  Memory: 6.7694854736328125 GB (4840.7109375 MB free)
  Uptime: 994.29 sec
  Load Avg:  1.0  1.02  0.81
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, broadwell)
  Threads: 1 on 2 virtual cores
```

---
# Runtime information
| Runtime Info | |
|:--|:--|
| BLAS #threads | 1 |
| `BLAS.vendor()` | `lbt` |
| `Sys.CPU_THREADS` | 2 |

`lscpu` output:

    Architecture:                    x86_64
    CPU op-mode(s):                  32-bit, 64-bit
    Address sizes:                   46 bits physical, 48 bits virtual
    Byte Order:                      Little Endian
    CPU(s):                          2
    On-line CPU(s) list:             0,1
    Vendor ID:                       GenuineIntel
    Model name:                      Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz
    CPU family:                      6
    Model:                           79
    Thread(s) per core:              1
    Core(s) per socket:              2
    Socket(s):                       1
    Stepping:                        1
    BogoMIPS:                        4589.37
    Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl xtopology cpuid pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 movbe popcnt aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single pti fsgsbase bmi1 hle avx2 smep bmi2 erms invpcid rtm rdseed adx smap xsaveopt md_clear
    Hypervisor vendor:               Microsoft
    Virtualization type:             full
    L1d cache:                       64 KiB (2 instances)
    L1i cache:                       64 KiB (2 instances)
    L2 cache:                        512 KiB (2 instances)
    L3 cache:                        50 MiB (1 instance)
    NUMA node(s):                    1
    NUMA node0 CPU(s):               0,1
    Vulnerability Itlb multihit:     KVM: Mitigation: VMX unsupported
    Vulnerability L1tf:              Mitigation; PTE Inversion
    Vulnerability Mds:               Mitigation; Clear CPU buffers; SMT Host state unknown
    Vulnerability Meltdown:          Mitigation; PTI
    Vulnerability Mmio stale data:   Vulnerable: Clear CPU buffers attempted, no microcode; SMT Host state unknown
    Vulnerability Retbleed:          Not affected
    Vulnerability Spec store bypass: Vulnerable
    Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
    Vulnerability Spectre v2:        Mitigation; Retpolines, STIBP disabled, RSB filling, PBRSB-eIBRS Not affected
    Vulnerability Srbds:             Not affected
    Vulnerability Tsx async abort:   Mitigation; Clear CPU buffers; SMT Host state unknown
    

| Cpu Property       | Value                                                   |
|:------------------ |:------------------------------------------------------- |
| Brand              | Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz               |
| Vendor             | :Intel                                                  |
| Architecture       | :Broadwell                                              |
| Model              | Family: 0x06, Model: 0x4f, Stepping: 0x01, Type: 0x00   |
| Cores              | 2 physical cores, 2 logical cores (on executing CPU)    |
|                    | No Hyperthreading hardware capability detected          |
| Clock Frequencies  | Not supported by CPU                                    |
| Data Cache         | Level 1:3 : (32, 256, 51200) kbytes                     |
|                    | 64 byte cache line size                                 |
| Address Size       | 48 bits virtual, 46 bits physical                       |
| SIMD               | 256 bit = 32 byte max. SIMD vector size                 |
| Time Stamp Counter | TSC is accessible via `rdtsc`                           |
|                    | TSC increased at every clock cycle (non-invariant TSC)  |
| Perf. Monitoring   | Performance Monitoring Counters (PMC) are not supported |
| Hypervisor         | Yes, Microsoft                                          |

