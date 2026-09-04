# 📁 项目结构说明

```
AI-Network-Security-Learning/
│
├── 📖 LEARNING_PLAN.md           # 学习计划（总体路线图）
├── 📖 PROJECT_STRUCTURE.md       # 本文件（项目结构）
├── 📖 RESOURCES.md               # 学习资源汇总
├── README.md                     # 项目说明
├── .gitignore
│
├── 01_Basics/                    # 阶段一：基础知识
│   ├── 01_ML_Fundamentals/       # ML基础
│   │   ├── neural_networks_basics.py
│   │   ├── deep_learning_overview.md
│   │   └── model_training_tutorial.ipynb
│   │
│   └── 02_Network_Security_Basics/
│       ├── network_protocols.md
│       ├── common_attacks.md
│       └── security_tools_guide.md
│
├── 02_Attack_Methods/            # 阶段二：攻击方法
│   ├── 03_Adversarial_Examples/  # 对抗样本
│   │   ├── fgsm_attack.py        # FGSM攻击
│   │   ├── pgd_attack.py         # PGD攻击
│   │   ├── c_w_attack.py         # C&W攻击
│   │   ├── deepfool_attack.py    # DeepFool攻击
│   │   ├── black_box_attack.py   # 黑盒攻击
│   │   ├── adversarial_examples.ipynb
│   │   └── README.md
│   │
│   ├── 04_Data_Poisoning/        # 数据投毒
│   │   ├── data_poisoning.py
│   │   ├── backdoor_attack.py
│   │   ├── trigger_generation.py
│   │   ├── label_flipping.py
│   │   └── README.md
│   │
│   └── 05_Model_Extraction/      # 模型窃取
│       ├── query_based_extraction.py
│       ├── parameter_extraction.py
│       ├── functional_copying.py
│       └── README.md
│
├── 03_Defense_Methods/           # 阶段三：防御方法
│   ├── 06_Adversarial_Defense/   # 对抗防御
│   │   ├── adversarial_training.py
│   │   ├── certified_defense.py
│   │   ├── robust_training.py
│   │   ├── robust_evaluation.py
│   │   └── README.md
│   │
│   ├── 07_Input_Defense/         # 输入防御
│   │   ├── input_sanitization.py
│   │   ├── feature_squeezing.py
│   │   ├── adversarial_detection.py
│   │   ├── defense_evaluation.py
│   │   └── README.md
│   │
│   └── 08_Model_Defense/         # 模型防御
│       ├── defensive_distillation.py
│       ├── gradient_masking.py
│       ├── certified_robustness.py
│       ├── trades_defense.py
│       └── README.md
│
├── 04_Security_Assessment/       # 阶段四：评估与测试
│   ├── 09_Robustness_Evaluation/ # 鲁棒性评估
│   │   ├── benchmark_suite.py
│   │   ├── robustness_metrics.py
│   │   ├── evaluation_framework.py
│   │   ├── evaluation_report_generator.py
│   │   └── README.md
│   │
│   ├── 10_Vulnerability_Discovery/
│   │   ├── membership_inference.py
│   │   ├── privacy_leakage_test.py
│   │   ├── model_inversion.py
│   │   ├── privacy_audit.py
│   │   └── README.md
│   │
│   └── 11_Penetration_Testing/
│       ├── model_api_test.py
│       ├── input_validation_test.py
│       ├── resource_abuse_test.py
│       ├── denial_of_service_test.py
│       └── README.md
│
├── 05_Practical_Applications/    # 阶段五：综合应用
│   ├── 12_Security_System_Design/
│   │   ├── security_architecture.py
│   │   ├── monitoring_system.py
│   │   ├── incident_response.py
│   │   ├── defense_pipeline.py
│   │   └── README.md
│   │
│   ├── 13_Real_World_Cases/      # 真实案例
│   │   ├── cv_security/          # 计算机视觉安全
│   │   │   ├── image_adversarial_attack.py
│   │   │   ├── object_detection_evasion.py
│   │   │   ├── face_recognition_attack.py
│   │   │   └── cv_defense.py
│   │   │
│   │   ├── nlp_security/         # NLP安全
│   │   │   ├── text_adversarial_attack.py
│   │   │   ├── prompt_injection.py
│   │   │   ├── model_poisoning_nlp.py
│   │   │   └── nlp_defense.py
│   │   │
│   │   ├── recommendation_security/  # 推荐系统安全
│   │   │   ├── poisoning_attack.py
│   │   │   ├── manipulation_detection.py
│   │   │   └── robust_recommendation.py
│   │   │
│   │   └── autonomous_driving_security/  # 自动驾驶安全
│   │       ├── adversarial_perturbation.py
│   │       ├── sensor_attack.py
│   │       └── safety_verification.py
│   │
│   └── 14_Capstone_Project/      # 毕业项目模板
│       ├── project_proposal.md
│       ├── implementation/
│       ├── experiments/
│       ├── results/
│       └── technical_report.md
│
├── docs/                         # 文档和教程
│   ├── tutorials/                # 教程
│   │   ├── setup_environment.md
│   │   ├── pytorch_basics.md
│   │   ├── adversarial_attack_guide.md
│   │   ├── defense_implementation_guide.md
│   │   └── evaluation_methodology.md
│   │
│   ├── concepts/                 # 概念讲解
│   │   ├── threat_models.md
│   │   ├── attack_taxonomy.md
│   │   ├── defense_mechanisms.md
│   │   └── evaluation_metrics.md
│   │
│   └── case_studies/             # 案例研究
│       ├── imagenet_adversarial_attacks.md
│       ├── bert_poisoning_attacks.md
│       └── real_world_security_incidents.md
│
├── tests/                        # 测试代码
│   ├── test_adversarial_attacks.py
│   ├── test_defense_mechanisms.py
│   ├── test_evaluation_metrics.py
│   └── test_security_assessment.py
│
├── utils/                        # 工具和辅助代码
│   ├── data_loader.py
│   ├── model_utils.py
│   ├── attack_utils.py
│   ├── defense_utils.py
│   ├── visualization.py
│   └── logger.py
│
├── datasets/                     # 数据集存放位置
│   ├── README.md                 # 数据集说明和下载指南
│   ├── cifar10/
│   ├── imagenet/
│   └── mnist/
│
├── models/                       # 预训练模型存放位置
│   ├── README.md
│   ├── pretrained_resnet50.pth
│   └── pretrained_bert.pt
│
├── results/                      # 实验结果存放
│   ├── attack_results/
│   ├── defense_evaluation/
│   ├── robustness_reports/
│   └── security_assessments/
│
├── requirements.txt              # Python依赖
├── setup.py                      # 项目安装脚本
└── LICENSE                       # MIT许可证
```

---

## 📂 各目录详细说明

### 阶段划分

| 阶段 | 目录 | 内容 | 时间 |
|------|------|------|------|
| 一 | `01_Basics/` | AI/ML基础 + 网络安全基础 | 2周 |
| 二 | `02_Attack_Methods/` | 对抗样本、数据投毒、模型窃取 | 2周 |
| 三 | `03_Defense_Methods/` | 对抗训练、输入防御、模型防御 | 2周 |
| 四 | `04_Security_Assessment/` | 鲁棒性评估、漏洞发现、渗透测试 | 2周 |
| 五 | `05_Practical_Applications/` | 综合应用、真实案例、毕业项目 | 2周 |

### 关键子目录

**`03_Adversarial_Examples/`** - 对抗样本学习
- 包含FGSM、PGD、C&W等主要攻击方法
- 包含黑盒攻击和白盒攻击示例
- Jupyter notebook供交互式学习

**`06_Adversarial_Defense/`** - 对抗防御
- 对抗训练实现
- 认证防御方法
- 鲁棒性评估工具

**`13_Real_World_Cases/`** - 真实应用场景
- 计算机视觉安全
- NLP安全
- 推荐系统安全
- 自动驾驶安全

**`docs/`** - 文档和理论
- 详细的教程和指南
- 概念讲解
- 案例研究

---

## 🚀 快速开始

1. **选择学习阶段** → 打开对应目录
2. **阅读README** → 了解该阶段内容
3. **学习代码** → 阅读实现代码并理解
4. **运行示例** → 执行.ipynb或.py文件
5. **修改实验** → 尝试调整参数和方法
6. **完成练习** → 按要求完成学习任务

---

## 📋 学习检查清单

- [ ] 完成阶段一基础知识学习
- [ ] 复现阶段二主要攻击方法
- [ ] 实现阶段三防御机制
- [ ] 进行阶段四安全评估
- [ ] 完成阶段五毕业项目

---

**准备好了吗？从 `01_Basics/` 开始你的AI安全之旅吧！** 🎯
