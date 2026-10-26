# kikun

鄂尔多斯应用技术学院 · 计算机科学 · 2028 届

关注数据库内核、性能优化与操作系统。正在寻找研发实习机会，远程优先。

## 代表项目

**[pgvector HNSW 内核优化](https://github.com/kkkkikun/polardb-pgvector-tuning)** · C / PostgreSQL / perf  
PolarDB 数据库创新设计赛作品。通过 perf 定位瓶颈，结合 SQ8 标量量化、SIMD 距离计算、访存优化与提前终止策略改进 HNSW。项目评测使用 1000 万条 200 维向量，在 Recall ≥ 0.85 的约束下，构建时间降低 **54.8%**、QPS 提升 **8.7%**、索引体积缩小 **34.1%**。仓库包含技术报告、性能分析与复现说明。

**[QuizForge](https://github.com/kkkkikun/QuizForge)** · Python / React / Pyodide  
将 Word、PDF、文本题库转换为离线答题网页，提供 Python CLI、React/PWA 站点与浏览器内转换，结合规则解析、可选 LLM 兜底和发布前数据校验。v0.2.0 增加图片抽取、模拟考试与进度迁移，并接入 Python 回归、前端测试和 Playwright 冒烟测试。[在线体验](https://kkkkikun.github.io/QuizForge/)

**[牵线 · 聚会筹办守护](https://github.com/kkkkikun/qianxian-guardian)** · Splash / OctoSense / Matrix  
运行于 OctoSense 的活动筹办小程序：从群消息生成提案，经用户确认后执行，覆盖冲突检查、AA 对账、日历导出与操作审计。v0.10.1 已签名发布，仓库记录 **40/40 端到端回归、12/12 操作覆盖**，并提供真实宿主运行、双实例协作与演示材料。[验收证据](https://github.com/kkkkikun/qianxian-guardian/blob/master/evidence/finals-verification-map.md)

## 上游贡献

参与 [RustSBI](https://github.com/rustsbi/rustsbi) 的 QEMU 启动测试与 CI 建设，以下 PR 均已合并：

- **RV32 最小 Linux 启动测试** — [#434](https://github.com/rustsbi/rustsbi/pull/434)，2026-10-23。补齐 Bare SBI、U-Boot 两条路径，验证 Linux 启动至 BusyBox 用户态，通过串口断言检查架构及 `/proc` 状态。两条路径均通过 GitHub Actions 端到端验证，完成 [Issue #375](https://github.com/rustsbi/rustsbi/issues/375)。
- **openRuyi 启动测试矩阵** — [#436](https://github.com/rustsbi/rustsbi/pull/436)，2026-10-25。新增 Server、Workstation labwc、KDE × Bare SBI、U-Boot、EDK II 共 9 组测试，固定镜像与校验和，检查用户态里程碑并保留诊断日志。PR CI 中新增 9 组及既有 Zero 测试合计 **10/10 通过**；脚本通过 ShellCheck 与 25 组离线自测，完成 [Issue #408](https://github.com/rustsbi/rustsbi/issues/408)。
- **构建脚本清理** — [#435](https://github.com/rustsbi/rustsbi/pull/435)，2026-10-22。移除 `rust-objcopy` 中冗余的固定架构参数，通过 xtask 测试，并验证 RV32/RV64 固件二进制输出与修改前逐字节一致。

## 竞赛与学习经历

- 全国大学生计算机系统能力大赛 · PolarDB 数据库创新设计赛：全国优胜奖，决赛第 19 名（3534 支参赛队）。
- 蓝桥杯程序设计大赛：国赛一等奖（2026）。
- 码蹄杯程序设计大赛：省赛金奖（2026）。
- 清华大学开源操作系统训练营（2026 春夏）：在 StarryOS 上实现 io_uring 异步 I/O。
- [VegarOS](https://github.com/kkkkikun/Vegar/tree/latest-oscamp)：基于 StarryOS 的操作系统实践，涉及测试框架集成、LTP 测试管理与 LoongArch64 兼容性修复。

## 技术与工具

C、Rust、Python · PostgreSQL · Linux / WSL · Docker · perf · GitHub Actions  
使用 Claude Code 辅助开发，结合调试、测试和性能分析验证实现。

## 联系方式

[邮箱](mailto:3581957503@qq.com) · [博客](https://blog.kkkkikun.dpdns.org)
