# 👻 Ghost_in_the_pic

A powerful AI-driven deepfake software designed for creative professionals in the media industry. Ghost_in_the_pic enables artists to animate custom characters, create engaging content, and develop models for various creative applications.

## ⚠️ Important Disclaimer

**This software is designed to be a productive tool for the AI-generated media industry.** We are committed to ethical development and responsible use of AI technology.

### 🎯 Intended Use Cases
- **Character Animation**: Animate custom characters for creative projects
- **Content Creation**: Develop engaging media content
- **Fashion & Design**: Create models for clothing and product design
- **Educational**: Learn about AI and computer vision technologies

### 🛡️ Built-in Safety Features
- **Content Filtering**: Automatic detection and blocking of inappropriate media
- **Nudity Detection**: Prevents processing of explicit content
- **Sensitive Material Protection**: Blocks graphic content and sensitive footage
- **Ethical Compliance**: Continuous monitoring for responsible usage

## 📋 Ethical Use Guidelines

### ✅ Responsible Usage
- **Obtain Consent**: Always get permission when using real person's likeness
- **Clear Labeling**: Mark all deepfake content when sharing publicly
- **Legal Compliance**: Follow all local and international laws
- **Respect Privacy**: Honor individuals' rights and dignity

### ❌ Prohibited Uses
- Creating content without consent
- Generating inappropriate or harmful material
- Violating privacy or defamation laws
- Using for malicious purposes

**By using this software, you agree to these ethical guidelines and commit to responsible usage.**

## 🚀 Installation

### Prerequisites

Ensure you have the following installed on your system:

- **Python 3.11** (recommended)
- **pip** (Python package installer)
- **git** (version control)
- **ffmpeg** - Install with: `iex (irm ffmpeg.tc.ht)` (Windows)
- **Visual Studio 2022 Runtimes** (Windows users)

### Quick Setup

> ⚠️ **Note**: This installation requires technical skills and is not recommended for beginners. Consider downloading the quickstart version if available.

#### 1. Clone the Repository
```bash
git clone https://github.com/hacksider/Deep-Live-Cam.git
cd Deep-Live-Cam
```

#### 2. Download Required Models
Download the following model files and place them in the `models` folder:
- [GFPGANv1.4](https://github.com/TencentARC/GFPGAN/releases/download/v1.3.0/GFPGANv1.4.pth)
- [inswapper_128_fp16.onnx](https://drive.google.com/file/d/1HvZ4MAtzlY74Dk4ASGIS9L6Rg5oZdqvu/view)

#### 3. Set Up Virtual Environment

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

**Linux/macOS:**
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

#### 4. Basic Usage
```bash
python run.py
```

> 📥 **First Run**: Initial execution will download additional models (~300MB)

## ⚡ GPU Acceleration

### NVIDIA CUDA Support

For enhanced performance on NVIDIA GPUs:

1. **Install CUDA Toolkit 12.8.0**
2. **Install cuDNN v8.9.7** for CUDA 12.x
   - Download from NVIDIA Developer Portal
   - Add cuDNN bin directory to system PATH
3. **Install GPU dependencies:**
```bash
pip install -U torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu128
pip uninstall onnxruntime onnxruntime-gpu
pip install onnxruntime-gpu==1.21.0
```

**Run with CUDA:**
```bash
python run.py --execution-provider cuda
```

### Apple Silicon Support (M1/M2/M3)

For Apple Silicon Macs:

1. **Ensure Python 3.10 is installed**
2. **Install CoreML dependencies:**
```bash
pip uninstall onnxruntime onnxruntime-silicon
pip install onnxruntime-silicon==1.13.1
```

**Run with CoreML:**
```bash
python3.10 run.py --execution-provider coreml
```

## 🛠️ System Requirements

### Minimum Requirements
- **OS**: Windows 10/11, macOS 10.15+, Ubuntu 18.04+
- **RAM**: 8GB minimum, 16GB recommended
- **Storage**: 5GB free space
- **Python**: 3.10 or 3.11

### Recommended for Best Performance
- **GPU**: NVIDIA RTX 3060 or better / Apple M1 Pro or better
- **RAM**: 32GB for large projects
- **Storage**: SSD with 10GB+ free space

## 📖 Usage Guide

1. **Launch the application**
2. **Select source image** (the face you want to use)
3. **Choose target media** (video or image to modify)
4. **Configure settings** as needed
5. **Process and export** your creation

## 🤝 Contributing

We welcome contributions from the community! Please ensure all contributions align with our ethical guidelines and safety standards.

## ⚖️ Legal & Compliance

- We adhere to all relevant laws and ethical guidelines
- We reserve the right to shut down the project or add watermarks if legally required
- Users are solely responsible for their use of this software
- We are not liable for misuse or illegal applications

## 📞 Support & Contact

For technical support, ethical concerns, or general inquiries, please open an issue on this repository.

## 📄 License

This project is licensed under [AGPL-3.0 license](https://github.com/Saurav-Astro/Ghost_in_the_pic/blob/main/LICENSE) - see the LICENSE file for details.

---

**Remember**: With great power comes great responsibility. Use Ghost_in_the_pic ethically and help us maintain a positive impact in the AI community.

*Ghost_in_the_pic - Bringing imagination to life, responsibly.*
