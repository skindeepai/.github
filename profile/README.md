# SkinDeep.ai - Preference Learning in Generative Latent Spaces (PLGL)

<p align="center">
  <img src="https://raw.githubusercontent.com/skindeepai/website/refs/heads/main/favicon-simple.svg" alt="PLGL Logo" width="120" height="120">
</p>

<p align="center">
  <strong>Transform AI with simple ratings. No prompting needed.</strong>
</p>

<p align="center">
  <a href="https://skindeep.ai">Website</a> •
  <a href="https://skindeep.ai/whitepaper.html">Whitepaper</a> •
  <a href="https://skindeep.ai/how-it-works.html">How It Works</a> •
  <a href="https://skindeep.ai/getting-started.html">Documentation</a> •
  <a href="https://skindeep.ai/examples/">Live Demos</a>
</p>

<p align="center">
  <a href="https://github.com/skindeepai/plgl/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a>
</p>

---

## 🎯 What is PLGL?

**PLGL (Preference Learning in Generative Latent Spaces)** is an open-source technology that revolutionizes how humans interact with generative AI. Instead of struggling with prompts, users simply rate AI-generated content with thumbs up/down, and PLGL learns their preferences to generate perfectly personalized results.

### Key Features

- **🚀 1000x Faster** - Direct latent space optimization using Reverse Classification™
- **⚡ 10ms Updates** - Real-time preference learning with SVMs
- **🔒 Privacy-First** - All preference learning happens on-device
- **🌍 Universal** - Works with ANY generative model with a latent space
- **💻 Open Source** - MIT licensed for maximum freedom

## 📦 Repository Structure

This repository contains the complete PLGL ecosystem:

### Core Components

```
/
├── plgl-website/          # Documentation website and demos
├── plgl-core/            # Core Python package (pip installable)
├── examples/             # Example implementations
├── PLGL_Whitepaper.md    # Technical whitepaper
├── ProvisionalPatent.txt # Original 2019 patent filing
└── LAUNCH_WEBSITE.md     # Website deployment guide
```

### Related Repositories

- **[skindeep-mobile](https://github.com/skindeepai/skindeep-mobile)** - Original iOS/Android apps (NativeScript)
- **[skindeep-server](https://github.com/skindeepai/skindeep-server)** - Original backend implementation
- **[plgl-examples](https://github.com/skindeepai/plgl-examples)** - Extended examples collection

## 🚀 Quick Start

### Installation

```bash
# Clone the repository
git clone https://github.com/skindeepai/plgl.git
cd plgl

# Install the Python package
pip install -e plgl-core/
```

### Basic Usage

```python
from plgl import PLGLCore, PreferenceModel

# Initialize with your generative model
plgl = PLGLCore(
    generator=your_model,
    latent_dim=512
)

# Generate initial samples
samples = plgl.generate_samples(n=10)

# Collect user preferences
preferences = []
for sample in samples:
    rating = get_user_rating(sample)  # 👍 or 👎
    preferences.append((sample, rating))

# Update preference model
plgl.update_preferences(preferences)

# Generate optimized content
ideal_content = plgl.generate_optimal()
```

## 🎯 Applications

PLGL transforms any generative AI application:

| Domain | Application | Benefits |
|--------|-------------|----------|
| 🎨 **Creative** | Art, Music, Design | No more prompt engineering |
| 📱 **Social** | Content feeds, Dating | Privacy-preserving personalization |
| 🛍️ **Commerce** | Product recommendations | Visual preference learning |
| 🧬 **Research** | Drug discovery, Materials | Efficient exploration |
| 🏗️ **Design** | Architecture, Interiors | Intuitive customization |
| 🎮 **Gaming** | Level generation, NPCs | Player-adaptive content |

## 📚 Documentation

- **[Getting Started Guide](https://skindeep.ai/getting-started.html)** - Step-by-step implementation
- **[Technical Whitepaper](PLGL_Whitepaper.md)** - In-depth algorithm details
- **[API Reference](https://skindeep.ai/api)** - Complete API documentation
- **[Live Examples](https://skindeep.ai/examples)** - Interactive demos
- **[How It Works](https://skindeep.ai/how-it-works.html)** - Visual explanation

## 🎥 Demo Videos

- **[Technology Overview](https://www.youtube.com/watch?v=M4oQLev_Sk8)** - 5-minute introduction
- **[Technical Deep Dive](https://www.youtube.com/watch?v=-6mAyFJ4_ME)** - Detailed walkthrough
- **[Original App Demo](https://youtube.com/skindeepai)** - 2019 dating app implementation

## 🛠️ Technical Innovation

### Reverse Classification™
Instead of searching through millions of latent vectors, PLGL directly computes the optimal vector that maximizes learned preferences.

### Real-time Learning
SVM-based preference models update in 10ms, enabling truly interactive experiences.

### Multi-modal Support
Handle multiple preference peaks - users can have diverse tastes that change with context.

## 🤝 Contributing

We welcome contributions! PLGL is open source under the MIT license.

### Ways to Help

- 🐛 Report bugs and issues
- 💡 Suggest new features
- 🔧 Submit pull requests
- 📖 Improve documentation
- 🌟 Star the repository
- 📢 Share with others

## 👨‍💻 About the Founder

**Steve Seguin** - Serial entrepreneur and open-source innovator

- 🎥 Creator of VDO.Ninja (100K+ daily users)
- 📺 Chief Innovation Officer at Stage TEN
- 🛍️ Former CTO of SLYCE (TSX:SLC)
- 🎯 Co-founder of HOVR.it (acquired)
- 🌟 20K+ GitHub stars across projects

Steve pioneered PLGL in 2018, years before the generative AI boom, recognizing that the future of AI interaction would move beyond prompting.

## 📄 License

PLGL is released under the [MIT License](LICENSE). You're free to use, modify, and distribute it for any purpose.

## 📬 Contact

- **Website**: [skindeep.ai](https://skindeep.ai)
- **Email**: contact@skindeep.ai
- **GitHub**: [@skindeepai](https://github.com/skindeepai)
- **Founder**: [steveseguin.com](https://steveseguin.com)

---

<p align="center">
  <strong>Join the preference revolution. Make AI truly personal.</strong>
</p>

<p align="center">
  <a href="https://github.com/skindeepai/plgl">
    <img src="https://img.shields.io/badge/Get%20Started-6366F1?style=for-the-badge&logo=github&logoColor=white" alt="Get Started">
  </a>
</p>

---

<p align="center">
  <sub>Built with ❤️ by SkinDeep.ai Inc. Transforming AI interaction since 2018.</sub>
</p>
