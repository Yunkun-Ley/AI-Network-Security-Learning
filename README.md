# 🛡️ AI网络攻防全栈学习项目

<div align="center">

**一个系统性、全面的AI网络攻防学习路径**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
![Status: Active Development](https://img.shields.io/badge/Status-Active%20Development-brightgreen.svg)

</div>

---

## 📌 项目简介

本项目是一个**全栈式、系统性**的AI安全学习平台，涵盖：

- ✅ **AI攻击方法** — 对抗样本、数据投毒、模型窃取
- ✅ **AI防御机制** — 对抗训练、输入防御、检测方法
- ✅ **安全评估** — 鲁棒性测试、漏洞发现、渗透测试
- ✅ **真实应用** — CV、NLP、推荐系统、自动驾驶等领域的安全

从**基础理论**到**实战项目**，包含代码实现、论文解读、完整的学习教程。

---

## 🎯 学习路线

```
基础知识(2周) → 攻击方法(2周) → 防御方法(2周) → 安全评估(2周) → 综合应用(2周)
    ↓              ↓              ↓              ↓              ↓
 ML/安全基础   FGSM/PGD等    对抗训练      鲁棒性测试    毕业项目
```

**总时间**: 10周（可根据个人进度调整）

---

## 📚 核心模块

### 🔴 阶段一：基础知识
- `01_ML_Fundamentals/` - 深度学习基础
- `02_Network_Security_Basics/` - 网络安全基础

### 🔴 阶段二：攻击方法
- `03_Adversarial_Examples/` - 对抗样本（FGSM、PGD、C&W等）
- `04_Data_Poisoning/` - 数据投毒和后门攻击
- `05_Model_Extraction/` - 模型盗取

### 🟡 阶段三：防御方法
- `06_Adversarial_Defense/` - 对抗防御和鲁棒训练
- `07_Input_Defense/` - 输入防御和异常检测
- `08_Model_Defense/` - 模型级防御

### 🟢 阶段四：安全评估
- `09_Robustness_Evaluation/` - 鲁棒性基准测试
- `10_Vulnerability_Discovery/` - 漏洞发现和隐私审计
- `11_Penetration_Testing/` - 渗透测试框架

### 🔵 阶段五：综合应用
- `12_Security_System_Design/` - 完整的安全系统设计
- `13_Real_World_Cases/` - 真实应用场景（CV、NLP、推荐系统、自动驾驶等）
- `14_Capstone_Project/` - 毕业项目模板

---

## 🚀 快速开始

### 环境配置

```bash
# 克隆项目
git clone https://github.com/Yunkun-Ley/AI-Network-Security-Learning.git
cd AI-Network-Security-Learning

# 创建虚拟环境
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 安装依赖
pip install -r requirements.txt
```

### 第一个攻击示例

```bash
# 运行FGSM攻击示例
cd 02_Attack_Methods/03_Adversarial_Examples
python fgsm_attack.py
```

### 学习Jupyter Notebook

```bash
# 启动Jupyter
jupyter notebook

# 打开任何.ipynb文件开始学习
```

---

## 📖 学习指南

### 推荐学习顺序

1. **第1周** - 阅读 `LEARNING_PLAN.md` 和 `docs/tutorials/setup_environment.md`
2. **第2-3周** - 完成阶段一和二的所有代码示例
3. **第4-5周** - 学习防御方法并进行对比实验
4. **第6-7周** - 进行安全评估和基准测试
5. **第8-10周** - 完成毕业项目

### 核心文档

- 📋 **[LEARNING_PLAN.md](./LEARNING_PLAN.md)** - 详细的学习计划和时间安排
- 📁 **[PROJECT_STRUCTURE.md](./PROJECT_STRUCTURE.md)** - 项目目录结构说明
- 📚 **[RESOURCES.md](./RESOURCES.md)** - 学习资源和参考论文
- 📖 **[docs/](./docs/)** - 详细教程和概念讲解

---

## 💻 代码示例

### 对抗样本攻击

```python
from attack_methods import FGSM, PGD

# FGSM攻击
fgsm = FGSM(model, eps=0.3)
adversarial_image = fgsm.attack(image)

# PGD攻击
pgd = PGD(model, eps=0.3, alpha=0.01, steps=40)
adversarial_image = pgd.attack(image)
```

### 对抗训练

```python
from defense_methods import AdversarialTraining

# 对抗训练
trainer = AdversarialTraining(model, attack_method='pgd')
trainer.train(train_loader, epochs=100)
```

### 鲁棒性评估

```python
from evaluation import RobustnessEvaluator

# 评估模型鲁棒性
evaluator = RobustnessEvaluator(model)
report = evaluator.evaluate(test_loader, attack_methods=['fgsm', 'pgd', 'c_w'])
print(report)
```

---

## 📊 项目特点

| 特点 | 说明 |
|------|------|
| 🎓 **系统性** | 从基础到进阶，循序渐进的学习路径 |
| 💻 **代码完整** | 每个方法都有完整的Python实现 |
| 📚 **文档齐全** | 包含教程、论文、案例研究等详细文档 |
| 🧪 **可复现** | 所有实验都可以复现，包含数据集和预训练模型 |
| 🏆 **实战性** | 涵盖真实应用场景（CV、NLP、推荐系统等） |
| 🚀 **持续更新** | 定期更新最新的攻防方法和研究成果 |

---

## 📄 核心论文

项目参考了以下重要论文（详见 [RESOURCES.md](./RESOURCES.md)）：

- **Goodfellow et al.** - "Explaining and Harnessing Adversarial Examples" (ICLR 2015)
- **Madry et al.** - "Towards Deep Learning Models Resistant to Adversarial Attacks" (ICLR 2018)
- **Carlini & Wagner** - "Towards Evaluating the Robustness of Neural Networks" (S&P 2017)
- **Shokri et al.** - "Membership Inference Attacks Against Machine Learning Models" (S&P 2017)
- **Zhang et al.** - "Theoretically Principled Trade-off between Robustness and Accuracy" (ICML 2019)

---

## 🛠️ 技术栈

- **深度学习框架**: PyTorch, TensorFlow
- **对抗攻击库**: ART (Adversarial Robustness Toolbox), Foolbox
- **评估工具**: AutoAttack, RobustBench
- **数据集**: CIFAR-10, ImageNet, MNIST
- **编程语言**: Python 3.8+

---

## 📋 项目计划

- [x] 项目初始化和结构设计
- [ ] 完成阶段一（基础知识）
- [ ] 完成阶段二（攻击方法）
- [ ] 完成阶段三（防御方法）
- [ ] 完成阶段四（安全评估）
- [ ] 完成阶段五（综合应用）
- [ ] 添加更多实验和案例
- [ ] 发布学习指南和最佳实践

---

## 🤝 如何贡献

欢迎贡献！你可以：

1. 📝 补充文档和教程
2. 💻 提交新的攻防方法实现
3. 🐛 报告bug和改进建议
4. 📚 分享学习心得和案例研究
5. 🧪 添加测试用例

---

## 📞 交流讨论

- 💬 [Issues](https://github.com/Yunkun-Ley/AI-Network-Security-Learning/issues) - 提问和讨论
- 🌟 如果有帮助，请给个Star支持一下！

---

## 📜 许可证

本项目采用 **MIT** 许可证。

---

## 🎓 学习成果

完成本项目学习后，你将能够：

- ✅ 理解AI安全的基本概念和威胁模型
- ✅ 掌握主要的对抗攻击方法及其实现
- ✅ 设计和部署有效的防御机制
- ✅ 进行模型的安全评估和渗透测试
- ✅ 在实际应用中应用AI安全知识
- ✅ 设计完整的AI安全系统架构
- ✅ 跟踪和理解最新的AI安全研究

---

<div align="center">

**准备好开始学习了吗？** 👇

[📖 开始学习](./LEARNING_PLAN.md) | [📁 查看结构](./PROJECT_STRUCTURE.md) | [📚 学习资源](./RESOURCES.md)

⭐ **如果项目对你有帮助，请给个Star！** ⭐

</div>

---

**最后更新**: 2026年9月  
**维护者**: Yunkun-Ley  
**项目状态**: 🟢 活跃开发中
