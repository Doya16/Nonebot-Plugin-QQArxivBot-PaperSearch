<!-- README language switch -->
[![中文](https://img.shields.io/badge/%E4%B8%AD%E6%96%87-555555?style=for-the-badge)](README.md) [![English](https://img.shields.io/badge/English-1677ff?style=for-the-badge)](README.en.md)
<!-- /README language switch -->

# Nonebot-Plugin Arxiv Paper Search

🔍 A [NoneBot2](https://v2.nonebot.dev/) plugin that retrieves abstracts of the latest arXiv papers in a specified category. Suitable for research discussion groups and AI/ML communities.

---

## 🖼 Example

Example response after sending `.arxiv cs.AI 3` in a QQ group:

![arxiv demo](demo/demo.png)

---

## ✨ Features

- 🧠 Retrieve the latest arXiv papers across all categories.
- 📚 Use `.arxiv list` to view recommended categories.

---

## 🛠 Installation and usage

### Install the plugin

Place `ArxivList.py` in your NoneBot plugins directory, for example at `plugins/arxiv_digest/__init__.py`:

```bash
mkdir -p plugins/arxiv_digest
cp ArxivList.py plugins/arxiv_digest/__init__.py
```

### Install dependencies

```bash
pip install nonebot2[fastapi] nonebot-adapter-onebot httpx
```

---

## 📦 Commands

| Example | Description |
| --- | --- |
| `.arxiv cs.LG 5` | Retrieve the 5 latest papers in cs.LG |
| `.arxiv list` | Show the recommended category list |
| `.公告 your message` | Administrator command: broadcast an announcement to all groups |

Keep the Chinese command keyword `.公告` as shown; replace `your message` with the announcement text.

---

## 📚 Recommended categories

| Category | Description |
| --- | --- |
| cs.AI | Artificial Intelligence |
| cs.CL | Computation and Language |
| cs.CV | Computer Vision and Pattern Recognition |
| cs.LG | Machine Learning |
| stat.ML | Machine Learning (Statistics) |
| cs.RO | Robotics |
| cs.CR | Cryptography and Security |
| cs.NI | Networking and Internet Architecture |

For more categories, see 👉 [arXiv taxonomy](https://arxiv.org/category_taxonomy).

---

## 📃 License

Released under the MIT License. You are welcome to use and modify the project.
