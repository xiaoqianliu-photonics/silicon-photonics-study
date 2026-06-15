# 硅光子学 4 周高强度自学计划

本计划专为《Silicon Photonics Design: From Devices to Systems》学习指南定制。以 4 周（28 天）为一个完整的学习周期，每天建议投入 2-3 小时。学习重点不仅在于理解原理，更在于培养工程直觉和设计思路。

---

## 📅 第一周：入门与无源器件基础 (Week 1)
**目标**：掌握光在硅波导中的传输原理，理解核心的光学无源分配与输入/输出器件。

* **Day 1: 硅光子学概述与平台**
  * 学习 `01_photonics_foundations.md`
  * 学习 `02_silicon_photonics_platform.md`
  * **行动**：了解 Fabless 模式，熟悉 SOI 材料对波长和温度的敏感性。
* **Day 2-3: 波导与模式分析**
  * 学习 `03_waveguides_and_modes.md`
  * 学习 `04_bends_tapers_and_mode_conversion.md`
  * **行动**：掌握单模条件计算，理解有效折射率方法（EIM），了解弯曲损耗的 trade-off。
* **Day 4-5: 光的分配与 I/O 耦合**
  * 学习 `05_directional_couplers_and_mmi.md`
  * 学习 `06_grating_couplers_and_edge_couplers.md`
  * **行动**：推导耦合方程，对比光栅耦合器和端面耦合器的优缺点及使用场景。
* **Day 6-7: 周末复习与巩固**
  * **行动**：回答 01-06 章的“复习问题”。如果有条件（如 Lumerical 或开源工具），尝试建立一个基础的 2D 硅波导仿真模型。

---

## 📅 第二周：进阶无源器件与有源器件 (Week 2)
**目标**：掌握利用干涉和共振原理进行光滤波的无源器件，并攻克硅光芯片的三大核心有源器件：调制器、探测器和激光光源。

* **Day 1-2: 谐振与干涉**
  * 学习 `07_ring_resonators.md`
  * 学习 `08_interferometers_mzi.md`
  * **行动**：死磕微环的公式（FSR, Q factor），理解 MZI 如何通过相位差实现光强控制。
* **Day 3-4: 光的调制 (Modulation)**
  * 学习 `09_modulators.md`
  * **行动**：深刻理解等离子体色散效应。对比 PN 结耗尽型调制器与热光调制器的带宽与功耗。
* **Day 5: 光的探测 (Detection)**
  * 学习 `10_photodetectors.md`
  * **行动**：掌握锗吸收原理，理解带宽、响应度与暗电流的折中（trade-off）关系。
* **Day 6: 光源挑战 (Light Sources)**
  * 学习 `11_lasers_and_light_sources.md`
  * **行动**：了解为什么硅不能直接发光，对比 Hybrid Silicon 与外部光源方案的系统级考量。
* **Day 7: 周末复习与巩固**
  * **行动**：梳理 07-11 章的知识图谱，重点复习有源器件的工作机制。

---

## 📅 第三周：系统级分析与建模仿真 (Week 3)
**目标**：从单一器件视角拔高到系统链路视角，掌握如何将器件拼接成系统，并学习如何利用仿真工具进行验证。

* **Day 1-2: 波分复用系统 (WDM)**
  * 学习 `12_wdm_filters_and_mux_demux.md`
  * **行动**：对比微环阵列与 AWG 在复用/解复用中的应用。
* **Day 3-4: 系统链路预算 (Link Budget)**
  * 学习 `13_link_budget_and_system_metrics.md`
  * **行动**：完成一次完整的光链路功率预算（Power Penalty），理解插入损耗、串扰对眼图和误码率（BER）的致命影响。
* **Day 5-6: 仿真方法学 (Simulation)**
  * 学习 `14_simulation_methods.md`
  * **行动**：区分 FDTD, EME, BPM 的适用边界。理解如何提取 S 参数并带入光子电路（Circuit）仿真中。
* **Day 7: 周末复习与系统级思考**
  * **行动**：尝试在一张白纸上画出一个完整光收发系统的数据流与光流走向。

---

## 📅 第四周：工程落地、流片测试与总结 (Week 4)
**目标**：掌握真正的“工程师技能”，从画版图到应对流片误差，再到测试与封装。

* **Day 1-2: PDK 与版图设计**
  * 学习 `15_layout_pdk_and_design_rules.md`
  * **行动**：理解工艺设计套件（PDK）的作用，知道 DRC 和 LVS 在光子学设计中的含义。
* **Day 3: 制造工艺波动 (Fabrication Variability)**
  * 学习 `16_fabrication_variability.md`
  * **行动**：理解为什么仿真结果和流片结果总是有偏差？学习如何进行鲁棒性设计。
* **Day 4-5: 封装与测试**
  * 学习 `17_testing_packaging_and_coupling.md`
  * **行动**：了解自动化光学测试平台的搭建，理解可测试性设计（Design for Test）在画版图时的重要性。
* **Day 6: 案例大串讲**
  * 学习 `18_system_design_examples.md`
  * **行动**：通过实际的 WDM 传输机案例，将前 4 周的知识点融会贯通。
* **Day 7: 总复习与查漏补缺**
  * **行动**：回顾 `99_glossary_and_formula_sheet.md`，检查 `README.md` 中每一章的预计掌握内容是否达标。恭喜你完成了这段硬核的学习旅程！

---

> [!TIP]
> 学习硅光子学，**不要把公式当做纯数学来背**，而是要问自己：**“如果我现在要提高这个器件的带宽，我应该调大哪个物理参数？代价是什么？”** 带着这种 Trade-off 的工程直觉去学习，效果会事半功倍！
