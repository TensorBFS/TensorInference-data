# Benchmark result

* Pull request commit: [`4a14c7cba48863c52f336fcf3517352c4b62b7ad`](https://github.com/TensorBFS/TensorInference.jl/commit/4a14c7cba48863c52f336fcf3517352c4b62b7ad)
* Pull request: <https://github.com/TensorBFS/TensorInference.jl/pull/26> (Add tropicalgemm and precompile)

# Judge result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmarks:
    - Target: 30 Jun 2023 - 08:49
    - Baseline: 30 Jun 2023 - 08:52
* Package commits:
    - Target: bbde0c
    - Baseline: f6298c
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
| `["map", "map"]`     |                2.32 (5%) :x: |                2.54 (1%) :x: |
| `["mar", "mar"]`     | 0.00 (5%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["mmap", "mmap-1"]` | 0.83 (5%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["mmap", "mmap-2"]` | 0.00 (5%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["mmap", "mmap-3"]` | 0.00 (5%) :white_check_mark: | 0.00 (1%) :white_check_mark: |

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
  CPU: Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz: 
              speed         user         nice          sys         idle          irq
       #1  2793 MHz       2978 s          0 s        185 s       4045 s          0 s
       #2  2793 MHz       3649 s          0 s        254 s       3314 s          0 s
  Memory: 6.7694854736328125 GB (4690.9609375 MB free)
  Uptime: 728.44 sec
  Load Avg:  1.0  1.0  0.65
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, icelake-server)
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
  CPU: Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz: 
              speed         user         nice          sys         idle          irq
       #1  2793 MHz       4928 s          0 s        208 s       4117 s          0 s
       #2  2793 MHz       3725 s          0 s        263 s       5265 s          0 s
  Memory: 6.7694854736328125 GB (4026.0234375 MB free)
  Uptime: 932.93 sec
  Load Avg:  1.0  1.0  0.73
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, icelake-server)
  Threads: 1 on 2 virtual cores
```

---
# Target result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmark: 30 Jun 2023 - 8:49
* Package commit: bbde0c
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

| ID                   | time            | GC time  | memory         | allocations |
|----------------------|----------------:|---------:|---------------:|------------:|
| `["map", "map"]`     | 165.493 ms (5%) | 6.550 ms | 92.24 MiB (1%) |      156343 |
| `["mar", "mar"]`     |  55.277 ms (5%) |          | 43.18 MiB (1%) |      170209 |
| `["mmap", "mmap-1"]` |  14.563 ms (5%) |          | 14.03 MiB (1%) |       41767 |
| `["mmap", "mmap-2"]` |  30.935 ms (5%) |          | 51.03 MiB (1%) |       44280 |
| `["mmap", "mmap-3"]` |  72.130 ms (5%) |          | 37.29 MiB (1%) |      154815 |

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
  CPU: Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz: 
              speed         user         nice          sys         idle          irq
       #1  2793 MHz       2978 s          0 s        185 s       4045 s          0 s
       #2  2793 MHz       3649 s          0 s        254 s       3314 s          0 s
  Memory: 6.7694854736328125 GB (4690.9609375 MB free)
  Uptime: 728.44 sec
  Load Avg:  1.0  1.0  0.65
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, icelake-server)
  Threads: 1 on 2 virtual cores
```

---
# Baseline result
# Benchmark Report for */home/runner/work/TensorInference.jl/TensorInference.jl*

## Job Properties
* Time of benchmark: 30 Jun 2023 - 8:52
* Package commit: f6298c
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

| ID                   | time           | GC time    | memory          | allocations |
|----------------------|---------------:|-----------:|----------------:|------------:|
| `["map", "map"]`     | 71.274 ms (5%) |            |  36.28 MiB (1%) |      158512 |
| `["mar", "mar"]`     |  24.087 s (5%) | 590.684 ms |   2.25 GiB (1%) |    33980607 |
| `["mmap", "mmap-1"]` | 17.497 ms (5%) |            |  22.43 MiB (1%) |       43753 |
| `["mmap", "mmap-2"]` |  11.752 s (5%) | 144.480 ms | 863.44 MiB (1%) |    11388868 |
| `["mmap", "mmap-3"]` | 118.244 s (5%) |    3.182 s |   8.55 GiB (1%) |   161155816 |

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
  CPU: Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz: 
              speed         user         nice          sys         idle          irq
       #1  2793 MHz       4928 s          0 s        208 s       4117 s          0 s
       #2  2793 MHz       3725 s          0 s        263 s       5265 s          0 s
  Memory: 6.7694854736328125 GB (4026.0234375 MB free)
  Uptime: 932.93 sec
  Load Avg:  1.0  1.0  0.73
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, icelake-server)
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
    Model name:                      Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz
    CPU family:                      6
    Model:                           106
    Thread(s) per core:              1
    Core(s) per socket:              2
    Socket(s):                       1
    Stepping:                        6
    BogoMIPS:                        5586.87
    Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl xtopology cpuid pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 movbe popcnt aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single pti fsgsbase bmi1 hle avx2 smep bmi2 erms invpcid rtm avx512f avx512dq rdseed adx smap clflushopt avx512cd avx512bw avx512vl xsaveopt xsavec xsaves md_clear
    Hypervisor vendor:               Microsoft
    Virtualization type:             full
    L1d cache:                       96 KiB (2 instances)
    L1i cache:                       64 KiB (2 instances)
    L2 cache:                        2.5 MiB (2 instances)
    L3 cache:                        48 MiB (1 instance)
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
| Brand              | Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz           |
| Vendor             | :Intel                                                  |
| Architecture       | :UnknownIntel                                           |
| Model              | Family: 0x06, Model: 0x6a, Stepping: 0x06, Type: 0x00   |
| Cores              | 2 physical cores, 2 logical cores (on executing CPU)    |
|                    | No Hyperthreading hardware capability detected          |
| Clock Frequencies  | Not supported by CPU                                    |
| Data Cache         | Level 1:3 : (48, 1280, 49152) kbytes                    |
|                    | 64 byte cache line size                                 |
| Address Size       | 48 bits virtual, 46 bits physical                       |
| SIMD               | 512 bit = 64 byte max. SIMD vector size                 |
| Time Stamp Counter | TSC is accessible via `rdtsc`                           |
|                    | TSC increased at every clock cycle (non-invariant TSC)  |
| Perf. Monitoring   | Performance Monitoring Counters (PMC) are not supported |
| Hypervisor         | Yes, Microsoft                                          |

