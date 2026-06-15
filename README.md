[README.md](https://github.com/user-attachments/files/28941713/README.md)
# 硅光子学与集成光子系统学习指南 (Silicon Photonics Study Guide)

欢迎来到《Silicon Photonics Design: From Devices to Systems》的学习库！本仓库根据“从器件到系统”的学习逻辑，将原书重构为适合自学、具有结构化总结的 Markdown 知识库。

## 学习路线与目录结构

为了实现最高效的自学，我们将庞杂的原书内容按照**逻辑依赖**分为三个学习阶段。建议严格按照以下顺序进行学习：

### 📁 阶段一：入门（物理基础与波导）
本阶段聚焦于硅光子学的基本物理概念、材料特性，以及光如何在硅波导中传输。
* **[`01_photonics_foundations.md`](01_photonics_foundations.md)**
  * **文件主题**：光学基础与硅光子学简介
  * **预计掌握**：光在介质中的传播、折射率、全反射等基础概念，了解为什么选择硅基光子学以及 Fabless 模式的意义。
* **[`02_silicon_photonics_platform.md`](02_silicon_photonics_platform.md)**
  * **文件主题**：SOI（Silicon-On-Insulator）平台与材料特性
  * **预计掌握**：硅、二氧化硅的光学特性，SOI 的结构优势及波长/温度依赖性。
* **[`03_waveguides_and_modes.md`](03_waveguides_and_modes.md)**
  * **文件主题**：硅波导结构与模式分析
  * **预计掌握**：平板波导、条形/脊形波导原理，单模/多模条件，有效折射率方法（Effective Index Method）。
* **[`04_bends_tapers_and_mode_conversion.md`](04_bends_tapers_and_mode_conversion.md)**
  * **文件主题**：弯曲波导、渐变器与模式转换
  * **预计掌握**：波导弯曲损耗（Bend Loss）、波导尺寸过渡设计（Tapers）以及模场匹配问题。

### 📁 阶段二：进阶（器件设计与建模）
本阶段深入探讨实现光分配、滤波、调控和探测的关键无源与有源器件原理。
* **[`05_directional_couplers_and_mmi.md`](05_directional_couplers_and_mmi.md)**
  * **文件主题**：定向耦合器与多模干涉仪 (MMI)
  * **预计掌握**：光场耦合理论，超模分析，定向耦合器设计及 MMI 的自成像原理。
* **[`06_grating_couplers_and_edge_couplers.md`](06_grating_couplers_and_edge_couplers.md)**
  * **文件主题**：光栅耦合器与端面耦合器（Optical I/O）
  * **预计掌握**：光纤到芯片的耦合挑战，光栅设计公式，端面纳米悬臂耦合器的设计与对准公差。
* **[`07_ring_resonators.md`](07_ring_resonators.md)**
  * **文件主题**：微环谐振器
  * **预计掌握**：微环谐振方程、FSR、Q值、Finesse等核心指标，及其在滤波和传感中的应用。
* **[`08_interferometers_mzi.md`](08_interferometers_mzi.md)**
  * **文件主题**：马赫-曾德尔干涉仪 (MZI)
  * **预计掌握**：MZI 的相位干涉原理、消光比计算及其在光开关和调制中的基础作用。
* **[`09_modulators.md`](09_modulators.md)**
  * **文件主题**：硅光调制器
  * **预计掌握**：等离子体色散效应（Plasma Dispersion Effect），PN 结耗尽型调制器、热光调制器及微环/MZI调制器架构。
* **[`10_photodetectors.md`](10_photodetectors.md)**
  * **文件主题**：锗硅光探测器
  * **预计掌握**：探测器带宽、响应度、暗电流指标，PIN 结与雪崩光电探测器（APD）原理。
* **[`11_lasers_and_light_sources.md`](11_lasers_and_light_sources.md)**
  * **文件主题**：激光器与片上光源
  * **预计掌握**：硅基发光挑战，混合集成（Hybrid Silicon Lasers）、单片外延生长与外部共封装光源方案。

### 📁 阶段三：系统（链路、仿真、封装与设计流程）
将单一器件整合成具备完整功能的芯片系统，考虑实际工程、流片工艺与测试环节。
* **[`12_wdm_filters_and_mux_demux.md`](12_wdm_filters_and_mux_demux.md)**
  * **文件主题**：波分复用滤波器与复用/解复用器
  * **预计掌握**：使用串联微环、阵列波导光栅（AWG）或级联 MZI 实现波分复用系统的架构。
* **[`13_link_budget_and_system_metrics.md`](13_link_budget_and_system_metrics.md)**
  * **文件主题**：链路预算与系统级指标
  * **预计掌握**：光功率预算计算，插入损耗、串扰、灵敏度、眼图及误码率（BER）在系统中的权衡。
* **[`14_simulation_methods.md`](14_simulation_methods.md)**
  * **文件主题**：仿真与建模方法学
  * **预计掌握**：FDTD, EME, BPM 等光学仿真算法的适用场景，以及从器件 S 参数到光子电路（Circuit）的联合仿真。
* **[`15_layout_pdk_and_design_rules.md`](15_layout_pdk_and_design_rules.md)**
  * **文件主题**：版图设计、PDK 与设计规则
  * **预计掌握**：工艺设计套件（PDK）的作用，GDS 版图绘制，DRC/LVS 检查流程及布线策略。
* **[`16_fabrication_variability.md`](16_fabrication_variability.md)**
  * **文件主题**：制造工艺与参数波动
  * **预计掌握**：光刻容差、刻蚀不均匀性对器件性能（特别是微环和光栅）的影响及鲁棒性设计（Corner Analysis）。
* **[`17_testing_packaging_and_coupling.md`](17_testing_packaging_and_coupling.md)**
  * **文件主题**：测试、封装与接口
  * **预计掌握**：自动化光学/电学探针台测试方案，光纤阵列与芯片的封装对准技术，以及可测试性设计（Design for Test）。
* **[`18_system_design_examples.md`](18_system_design_examples.md)**
  * **文件主题**：系统级设计实例
  * **预计掌握**：案例分析（如基于微环的 WDM 发射机），串联知识点，建立完整的系统工程直觉。

### 📚 附录与学习管理
* **[`00_learning_plan.md`](00_learning_plan.md)**：专为您设计的为期 4 周学习打卡计划。
* **[`19_migration_to_lithium_niobate.md`](19_migration_to_lithium_niobate.md)**：薄膜铌酸锂 (LNOI) 迁移指南（**特别增补**：详细对比硅光与铌酸锂的物理特性、干涉复用继承机制与微波电极重构思路）。
* **[`99_glossary_and_formula_sheet.md`](99_glossary_and_formula_sheet.md)**：全书核心物理公式速查表与光子学术语大辞典（A-Z）。

## 如何使用本文档？
1. 请先阅读 `00_learning_plan.md` 了解时间安排。
2. 按照 01 到 18 的顺序阅读各个 `.md` 文件。
3. 重点关注每章结尾的 **复习问题** 和 **学习检查清单**，确保自己已经达到该章的学习目标。
4. 本指南为提炼与总结，部分深度细节或特殊图表可能需要您结合原书或参考相关文献进行阅读。
