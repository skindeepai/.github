# SkinDeep.ai

<p align="center">
  <img src="https://raw.githubusercontent.com/skindeepai/website/main/favicon.svg" alt="SkinDeep logo" width="96" height="96">
</p>

SkinDeep is an independent research lab working on preference learning, direct model outputs, and ways to reduce model computation.

The work began with an app that learned what people liked from ratings of generated faces. Today we also test models that return labels or coordinates, and methods that stop processing early or ask a larger model for help.

---

## 🎯 Research topics

- **[Learning personal preferences](https://skindeep.ai/preferences.html)** — Learn from ratings to score candidates, suggest new ones, or make a constrained edit.
- **[Decisions without a written reply](https://skindeep.ai/decisions.html)** — Read a model's internal representation with a trained classifier to return a category, such as a moderation label or support topic.
- **[Stopping early](https://skindeep.ai/adaptive.html)** — Test earlier classifier checkpoints and small-model fallbacks, measuring both time saved and mistakes.
- **[Image to coordinates](https://skindeep.ai/coordinates.html)** — Explore predicting where to click directly from a screenshot.

These are experiments, with task-specific results and limitations. The [results](https://skindeep.ai/results.html) include datasets, methods, timings, and unsuccessful tests.

## 📦 Repositories

- **[website](https://github.com/skindeepai/website)** — Current research website, browser demos, experiment code, and evidence.
- **[skindeep-mobile](https://github.com/skindeepai/skindeep-mobile)** — Original iOS/Android apps (NativeScript).
- **[skindeep-server](https://github.com/skindeepai/skindeep-server)** — Original backend implementation.

## 📚 Documentation and demos

- **[Browser demos](https://skindeep.ai/demo-directory.html)** — Try the approaches and follow links to matching results.
- **[How preference learning works](https://skindeep.ai/how-it-works.html)** — From ratings to scores, suggestions, and edits.
- **[Research FAQ](https://skindeep.ai/research.html)** — Questions, findings, and what remains unproven.
- **[Original work and history](https://skindeep.ai/history.html)** — The starting point for SkinDeep and its preference-learning approach.

## 🛠️ Original preference-learning work

**PLGL (Preference Learning in Generative Latent Spaces)** remains part of SkinDeep's research. Users rate generated examples, and a small model learns preferences over the numbers that control a compatible generator.

### Reverse classification

Use the learned preference model to find a bounded latent vector with a high predicted score, or a small change toward a desired score. A higher predicted score still needs to be checked against what the person actually likes.

### Interactive learning

Small preference models, including SVMs, can update as new ratings arrive. Local learning is one way to keep preference data on the user's device.

### Multiple preferences

A person can like several different styles. Modeling multiple preference regions is an approach to representing that variety instead of reducing it to one average.

## 👨‍💻 About the Founder

**Steve Seguin** - Serial entrepreneur and open-source innovator

- 🎥 Creator of VDO.Ninja (100K+ daily users)
- 💼 Principal Engineer at eBay
- 📺 Chief Innovation Officer at Stage TEN
- 🛍️ Former CTO of SLYCE (TSX:SLC)
- 🎯 Co-founder of HOVR.it (acquired)
- 🌟 20K+ GitHub stars across projects

Steve began SkinDeep's preference-learning work in 2018. That original work continues alongside the broader research.

## 📄 License

The [website and research code](https://github.com/skindeepai/website/blob/main/LICENSE) are MIT licensed. See individual repositories, models, and datasets for their respective licenses.

## 📬 Contact

- **Website**: [skindeep.ai](https://skindeep.ai)
- **Email**: contact@skindeep.ai
- **GitHub**: [@skindeepai](https://github.com/skindeepai)
- **Founder**: [steveseguin.com](https://steveseguin.com)
