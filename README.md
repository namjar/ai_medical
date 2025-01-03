# 医疗影像 AI 助手 | Medical Imaging AI Assistant

[English](README_EN.md) | 简体中文

基于 Gemini Pro Vision 的医疗影像分析助手，支持多种医疗图像格式的智能分析。

## 功能特点

- 支持多种医疗图像格式 (JPEG, PNG, DICOM)
- 智能识别图像类型
- 提供解剖位置分析
- 生成专业医学发现报告
- 多语言支持 (中文/英文)

## 快速开始

### 环境要求
- Python 3.9+
- pip 包管理器

### 安装步骤

1. 克隆仓库
```bash
git clone https://github.com/namjar/ai_medical.git
cd ai_medical
```

2. **创建虚拟环境**
```bash
  python -m venv .venv
  source .venv/bin/activate  # macOS/Linux
```


3. **安装依赖**
   ```bash
   pip install -r requirements.txt
   ```

3. **配置 API 密钥**
   - 从 [Google AI Studio](https://aistudio.google.com) 获取 Google API 密钥

4. **配置环境变量**
```bash
  export GOOGLE_API_KEY='your-api-key'
  export LANGUAGE_DEFAULT='zh-CN'
   ```

5. **运行应用程序**
   ```bash
   streamlit run ai_medical_imaging.py
   ```

6. **项目结构**

     ai_medical/
  ├── ai_medical_imaging.py  # 主程序
  ├── requirements.txt       # 依赖配置
  ├── locales/              # 多语言支持
  │   └── zh-CN/           
  │       └── translation.json
  └── README.md


## 分析组件

- **图像类型和区域**
  - 识别成像模式
  - 指定解剖区域

- **主要发现**
  - 系统列出观察结果
  - 详细的外观描述
  - 异常高亮

- **诊断评估**
  - 潜在诊断排名
  - 鉴别诊断
  - 严重程度评估

- **患者友好解释**
  - 简化术语
  - 详细的基本原理解释
  - 视觉参考点

## 注意事项

- 使用 Gemini 2.0 Flash 进行分析
- 需要稳定的互联网连接
- API 使用费用适用
- 仅供教育和开发用途
- 不能替代专业的医学诊断

## 免责声明

此工具仅供教育和信息用途。所有分析应由合格的医疗专业人员审核。不要仅根据此分析做出医疗决策。