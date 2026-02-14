## Hi there 👋 I'm Will Domine

- 🔭 Passionate about performance engineering and systems programming, always seeking to optimize and learn.
  
- 🌱 Currently focusing on high-performance systems, SIMD optimization, and cloud-native microservices.
  
- 📚 I'm a junior at the University of Wisconsin-Whitewater, working toward a B.S. in Computer Science, expected to graduate December 2026.

- 💼 Full Stack Engineer Intern at The Boldt Company, working with Azure, Next.js, and Python.

- ⚡ Fun fact: I began coding in Python at 14 and have been hooked ever since!

- 📫 Ways to contact me!

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-blue?style=for-the-badge&logo=LinkedIn&logoColor=white)](https://www.linkedin.com/in/will-domine)
[![Outlook](https://img.shields.io/badge/Outlook-0078D4?style=for-the-badge&logo=microsoft-outlook&logoColor=white)](mailto:willdomine1@outlook.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://www.willdomine.com)

---

## 🚀 Featured Projects

### [AVX2 High-Performance Packet Filter](https://github.com/WillDomine/avx2-packet-filter)

A header-only C++ library utilizing AVX2 SIMD intrinsics to filter network packets with **0.76ns latency**, processing **~1.3 billion packets per second** on Intel Core i9-14900K.

**What makes it fast:**
- 🎯 **2.44x speedup** over scalar implementation by leveraging `_mm256_i32gather_epi32` to process batches of 8 packets in parallel
- 🧠 32-byte aligned packet structures ensuring exactly 2 packets fit per 64-byte CPU cache line, minimizing cache misses
- 🔄 Zero-copy `io_uring` TCP server demonstrating the filter in a production environment

**Performance Comparison:**

| Implementation | Latency | Throughput | Speedup |
|:--------------|:--------|:-----------|:--------|
| Scalar C++ | 1.86 ns | ~0.5 Billion PPS | 1.0x |
| **AVX2 SIMD** | **0.76 ns** | **~1.3 Billion PPS** | **2.44x** |

![C++](https://img.shields.io/badge/C++-20-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![AVX2](https://img.shields.io/badge/AVX2-SIMD-red?style=for-the-badge)
![io_uring](https://img.shields.io/badge/io__uring-Zero--Copy-orange?style=for-the-badge)

---

### [BitMesh Gateway](https://github.com/WillDomine/bitmesh-gateway)

A cloud-native gRPC edge router achieving **44,160 RPS** with **sub-1.3ms latency**. Designed to solve the "Thundering Herd" problem in distributed systems through intelligent connection pooling and zero-allocation request handling.

**Key optimizations:**
- 🚀 **7x performance improvement** over baseline (6,369 RPS → 44,160 RPS on Linux)
- 💾 Zero-allocation hot paths using `sync.Pool` to reuse request contexts, eliminating GC pauses
- 🔌 Thread-safe connection pool with `sync.RWMutex` and double-checked locking to reuse persistent gRPC connections
- ⚙️ O(1) routing logic using bitwise AND operations on binary feature flags instead of string comparisons
- 🐳 Multi-stage Docker build producing a 15MB Alpine image with hot-reloadable YAML configuration

**Performance Benchmarks:**

| Environment | Throughput | Avg Latency | Allocations |
|:-----------|:-----------|:------------|:-----------|
| Standard Request (Baseline) | 6,369 req/s | 7.72 ms | 4 B/op |
| BitMesh (Windows 11) | 21,336 req/s | 2.31 ms | **0 B/op** |
| **BitMesh (Linux/CachyOS)** | **44,160 req/s** | **1.12 ms** | **0 B/op** |

![Go](https://img.shields.io/badge/Go-1.25+-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-High%20Performance-244C5A?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker&logoColor=white)

---

## Programming Languages

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)

## Frameworks

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Nuxt](https://img.shields.io/badge/Nuxt-00DC82?style=for-the-badge&logo=nuxtdotjs&logoColor=white)
![Vue](https://img.shields.io/badge/Vue-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=for-the-badge&logo=google&logoColor=white)

## Technical Tools

![Microsoft Azure](https://img.shields.io/badge/Microsoft%20Azure-0089D6?style=for-the-badge&logo=msazure&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure%20DevOps-0078D4?style=for-the-badge&logo=azuredevops&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4DB33D?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 🏆 Certifications

- **Microsoft Certified: Azure Fundamentals** (Credential ID: 3DF1E0BC8BE25009)

## 🌐 Languages

- 🇺🇸 English (Native)
- 🇯🇵 Japanese (Elementary - Genki I)
