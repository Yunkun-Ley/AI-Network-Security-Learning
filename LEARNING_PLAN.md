# 🎓 AI网络攻防全栈学习计划

## 📋 学习路线图

本学习计划分为 **5个阶段**，从基础到进阶，配合实战项目和代码示例。

---

## 🌟 阶段一：基础知识（第1-2周）

### 1.1 AI/ML 基础
- [ ] 神经网络基本原理
- [ ] 深度学习框架对比（PyTorch vs TensorFlow）
- [ ] 常见模型架构（CNN, RNN, Transformer）
- [ ] 模型训练和推理流程

**资源**：
- 📚 深度学习书籍 / 视频教程
- 💻 项目：`01_Basics/` - 基础模型训练示例

### 1.2 网络安全基础
- [ ] 网络攻击类型和防御思路
- [ ] 密码学基础
- [ ] 常见漏洞分类（OWASP Top 10）
- [ ] 渗透测试基本概念

**资源**：
- 📚 网络安全入门资料
- 💻 项目：`02_Network_Security_Basics/` - 安全工具使用

---

## 🎯 阶段二：AI攻击方法（第3-4周）

### 2.1 对抗样本（Adversarial Examples）
- [ ] 对抗样本的定义和分类
  - FGSM（Fast Gradient Sign Method）
  - PGD（Projected Gradient Descent）
  - C&W（Carlini & Wagner）攻击
  - DeepFool
- [ ] 黑盒 vs 白盒攻击
- [ ] 转移性（Transferability）
- [ ] 实际应用案例

**资源**：
- 📚 论文：《Explaining and Harnessing Adversarial Examples》
- 💻 项目：`03_Adversarial_Examples/`
  - `fgsm_attack.py` - FGSM攻击实现
  - `pgd_attack.py` - PGD攻击实现
  - `c_w_attack.py` - C&W攻击实现
  - `black_box_attack.py` - 黑盒攻击示例

### 2.2 数据投毒（Data Poisoning）
- [ ] 投毒攻击原理
- [ ] 后门攻击（Backdoor Attack）
- [ ] 标签翻转攻击
- [ ] 触发器设计

**资源**：
- 📚 论文：《Poison Frogs! Targeted Clean-Label Poisoning Attacks》
- 💻 项目：`04_Data_Poisoning/`
  - `data_poisoning.py` - 数据投毒实现
  - `backdoor_attack.py` - 后门攻击实现
  - `trigger_generation.py` - 触发器生成

### 2.3 模型盗取（Model Extraction）
- [ ] 黑盒查询式模型窃取
- [ ] 白盒模型参数提取
- [ ] 功能模型复制
- [ ] 防御方法

**资源**：
- 📚 论文：《Knockoff Nets: Stealing Functionality of Black-Box Models》
- 💻 项目：`05_Model_Extraction/`
  - `query_based_extraction.py` - 查询式窃取
  - `parameter_extraction.py` - 参数提取

---

## 🛡️ 阶段三：AI防御方法（第5-6周）

### 3.1 对抗训练（Adversarial Training）
- [ ] 对抗训练原理
- [ ] 标准对抗训练
- [ ] 自适应对抗训练
- [ ] 性能权衡

**资源**：
- 📚 论文：《Adversarial Training for Free!》
- 💻 项目：`06_Adversarial_Defense/`
  - `adversarial_training.py` - 对抗训练实现
  - `certified_defense.py` - 认证防御
  - `robust_evaluation.py` - 鲁棒性评估

### 3.2 输入防御
- [ ] 输入净化（Input Sanitization）
- [ ] 特征压缩（Feature Squeezing）
- [ ] JPEG压缩防御
- [ ] 检测对抗样本

**资源**：
- 📚 论文：《Feature Squeezing: Detecting Adversarial Examples in Deep Neural Networks》
- 💻 项目：`07_Input_Defense/`
  - `input_sanitization.py` - 输入净化
  - `adversarial_detection.py` - 对抗样本检测
  - `defense_evaluation.py` - 防御效果评估

### 3.3 模型防御
- [ ] 防御性蒸馏（Defensive Distillation）
- [ ] 梯度掩码（Gradient Masking）
- [ ] 认证防御（Certified Defenses）
- [ ] TRADES防御

**资源**：
- 📚 论文：《Towards Deep Learning Models Resistant to Adversarial Attacks》
- 💻 项目：`08_Model_Defense/`
  - `defensive_distillation.py` - 防御性蒸馏
  - `certified_robustness.py` - 认证鲁棒性

---

## 🔍 阶段四：安全评估与渗透测试（第7-8周）

### 4.1 模型鲁棒性评估
- [ ] 评估指标体系
- [ ] 鲁棒性基准测试
- [ ] 对标准模型的评估
- [ ] 生成鲁棒性报告

**资源**：
- 💻 项目：`09_Robustness_Evaluation/`
  - `benchmark_suite.py` - 基准测试套件
  - `robustness_metrics.py` - 鲁棒性指标
  - `evaluation_report.py` - 生成评估报告

### 4.2 漏洞发现与利用
- [ ] 模型推断攻击（Membership Inference）
- [ ] 隐私泄露（Privacy Leakage）
- [ ] 模型反演攻击（Model Inversion）
- [ ] 隐私审计

**资源**：
- 📚 论文：《Membership Inference Attacks Against Machine Learning Models》
- 💻 项目：`10_Vulnerability_Discovery/`
  - `membership_inference.py` - 成员推断攻击
  - `privacy_leakage_test.py` - 隐私泄露检测
  - `model_inversion.py` - 模型反演攻击

### 4.3 渗透测试框架
- [ ] AI模型的安全测试
- [ ] API安全测试
- [ ] 部署环境安全评估
- [ ] 自动化测试工具

**资源**：
- 💻 项目：`11_Penetration_Testing/`
  - `model_api_test.py` - API安全测试
  - `input_validation_test.py` - 输入验证测试
  - `resource_abuse_test.py` - 资源滥用测试

---

## 🚀 阶段五：综合应用与实战（第9-10周）

### 5.1 完整安全系统设计
- [ ] AI模型安全架构设计
- [ ] 多层防御体系搭建
- [ ] 安全监控和告警
- [ ] 应急响应机制

**资源**：
- 💻 项目：`12_Security_System_Design/`
  - `security_architecture.py` - 安全架构
  - `monitoring_system.py` - 监控系统
  - `incident_response.py` - 应急响应

### 5.2 真实场景案例分析
- [ ] 计算机视觉模型攻防
- [ ] NLP模型攻防
- [ ] 推荐系统安全
- [ ] 自动驾驶安全

**资源**：
- 💻 项目：`13_Real_World_Cases/`
  - `cv_security/` - 计算机视觉安全
  - `nlp_security/` - NLP安全
  - `recommendation_security/` - 推荐系统安全
  - `autonomous_driving_security/` - 自动驾驶安全

### 5.3 毕业项目
- [ ] 选择一个实际问题
- [ ] 设计完整的攻防方案
- [ ] 实现和验证
- [ ] 撰写技术报告

**资源**：
- 💻 项目：`14_Capstone_Project/`
  - 项目提案
  - 实现代码
  - 技术报告
  - 演示和测试

---

## 📚 学习资源汇总

### 核心论文
1. **对抗样本基础**
   - Goodfellow et al., "Explaining and Harnessing Adversarial Examples" (ICLR 2015)
   - Madry et al., "Towards Deep Learning Models Resistant to Adversarial Attacks" (ICLR 2018)

2. **防御方法**
   - Papernot et al., "Defensive Distillation is not Robust to Adversarial Examples" (2016)
   - Zhang et al., "Theoretically Principled Trade-off between Robustness and Accuracy" (ICML 2019)

3. **模型安全**
   - Shokri et al., "Membership Inference Attacks Against Machine Learning Models" (S&P 2017)
   - Fredrikson et al., "Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures" (CCS 2015)

### 开源工具库
- **Adversarial Robustness Toolbox (ART)** - IBM的对抗鲁棒性工具包
- **CleverHans** - OpenAI对抗样本库
- **FGSM/PGD** - PyTorch实现
- **Foolbox** - 对抗样本生成框架

### 学习社区
- arXiv (cs.CR, cs.AI)
- GitHub (adversarial-examples, AI-security)
- Kaggle (竞赛和数据集)
- 学术会议 (ICLR, ICML, S&P, CCS)

---

## 🎯 学习建议

### ✅ 推荐做法
1. **边学边做** - 每个阶段配合代码实践
2. **重视论文** - 理解原理而非盲目编码
3. **复现实验** - 按论文复现攻防方法
4. **做笔记** - 记录关键概念和发现
5. **参与讨论** - 在社区分享想法

### ⏱️ 时间估计
- 基础知识：2周
- 攻击方法：2周
- 防御方法：2周
- 评估与测试：2周
- 综合应用：2周

**总计：10周（可根据个人进度调整）**

### 🏆 学习目标
- [ ] 理解AI安全的基本概念和威胁模型
- [ ] 掌握主要攻击方法的实现和原理
- [ ] 学会设计和部署防御机制
- [ ] 能够进行安全评估和渗透测试
- [ ] 能够设计完整的AI安全系统

---

## 📞 遇到问题？

- 查看 `RESOURCES.md` 获取详细资源
- 在 `issues/` 中提问和讨论
- 查看 `docs/` 中的详细教程
- 贡献你的学习成果！

---

**开始学习吧！🚀 选择一个阶段，从 `01_Basics/` 开始！**
