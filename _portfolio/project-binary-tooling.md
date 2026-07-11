---
title: "二进制漏洞挖掘工具链（示例）"
excerpt: "结合 fuzzing 与符号执行的自动化漏洞发现工具，聚焦 UAF、堆溢出及缓解绕过。"
collection: portfolio
---

### 概述 / Overview

待补充——用 2~3 句话说明这个项目解决什么问题。方向建议：一套基于覆盖率引导 fuzzing 与符号执行（symbolic execution）联动的二进制漏洞挖掘工具链，针对 C/C++ 目标自动化发现 UAF（use-after-free）、堆溢出（heap overflow）等内存安全缺陷，并辅助生成缓解绕过（mitigation bypass）的利用路径。

### 技术栈 / Stack

- C、Python
- AFL++、libFuzzer
- angr（符号执行 / 约束求解）
- Z3 SMT Solver
- IDA Pro / Ghidra（脚本化逆向分析）
- GDB / pwndbg / GEF（动态调试）

### 我的角色 / My Role

待补充——例如：独立开发，负责 fuzzer harness 编写、符号执行插桩模块设计、crash 自动分类与可利用性判定逻辑实现。

### 成果 / Highlights

- 待补充
- 方向建议：在 N 个开源项目中发现真实漏洞，crash 自动去重与根因分析准确率达 XX%。

### 链接 / Links

- 仓库：待补充
