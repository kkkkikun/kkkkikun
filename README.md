# kikun

鄂尔多斯应用技术学院 · 计算机科学 · 2028 届

关注数据库内核、性能优化与操作系统。正在寻找研发实习机会，远程优先。

## 项目

**[pgvector HNSW 内核优化](https://github.com/kkkkikun/polardb-pgvector-tuning)** · C / PostgreSQL / perf  
PolarDB 数据库创新设计赛作品。通过 perf 分析瓶颈，实现 SQ8 标量量化、SIMD 距离计算与提前终止策略。项目评测中，构建时间降低 54.8%，QPS 提升 8.7%，索引体积缩小 34.1%；仓库包含技术报告与性能分析。

**[VegarOS](https://github.com/kkkkikun/Vegar)** · Rust / io_uring  
基于 StarryOS 的异步操作系统项目，围绕 io_uring 异步 I/O 与串口驱动异步化展开开发，参与全国大学生计算机系统能力大赛内核实现赛道。

**[QuizForge](https://github.com/kkkkikun/QuizForge)** · Python / LLM  
将 Word、PDF 题库转换为单文件答题网页，结合规则解析与 LLM 处理题目提取。

## 上游贡献

参与 [RustSBI](https://github.com/rustsbi/rustsbi) 的 QEMU 启动测试与 CI 建设：

- **RV32 最小 Linux 启动测试** — [PR #434](https://github.com/rustsbi/rustsbi/pull/434)，2026-10-23 合并。补齐 Bare SBI、U-Boot 两条路径，验证 Linux 启动至 BusyBox 用户态，通过串口断言检查架构及 `/proc` 状态。两条路径均通过 GitHub Actions 端到端验证，完成 [Issue #375](https://github.com/rustsbi/rustsbi/issues/375)。
- **openRuyi 启动测试矩阵** — [PR #436](https://github.com/rustsbi/rustsbi/pull/436)，2026-10-25 合并。新增 Server、Workstation labwc、KDE × Bare SBI、U-Boot、EDK II 共 9 组测试，固定镜像与校验和，检查用户态里程碑并保留诊断日志。PR CI 中新增 9 组及既有 Zero 测试合计 10/10 通过；脚本通过 ShellCheck 与 25 组离线自测，完成 [Issue #408](https://github.com/rustsbi/rustsbi/issues/408)。

## 竞赛与学习经历

- 全国大学生计算机系统能力大赛 · PolarDB 数据库创新设计赛：全国优胜奖，决赛第 19 名（3534 支参赛队）。
- 蓝桥杯程序设计大赛：国赛一等奖（2026）。
- 码蹄杯程序设计大赛：省赛金奖（2026）。
- 清华大学开源操作系统训练营（2026 春夏）：在 StarryOS 上实现 io_uring 异步 I/O。

## 技术与工具

C、Rust、Python · PostgreSQL · Linux / WSL · Docker · perf · GitHub Actions  
使用 Claude Code 辅助开发，结合调试、测试和性能分析验证实现。

## 联系方式

[邮箱](mailto:3581957503@qq.com) · [博客](https://blog.kkkkikun.dpdns.org)
