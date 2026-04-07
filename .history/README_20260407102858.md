<div align="center">

# 📚 NTU EE6497 Cheat Sheet
## 🧠 Pattern Recognition & Deep Learning

<p align="center">
  <b>A highly compact, LaTeX-based quick reference for the AY2025 examinations.</b>
</p>

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![LaTeX](https://img.shields.io/badge/Language-LaTeX-008080.svg?logo=latex&style=for-the-badge)](https://www.latex-project.org/)
[![Year](https://img.shields.io/badge/Academic%20Year-AY2025-FF6B6B.svg?style=for-the-badge)]()

<br />

<!-- 💡 Tip: You can place a screenshot of the compiled PDF here -->
<!-- <img src="assets/preview.png" alt="Cheat Sheet Preview" width="600" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/> -->

</div>

---

## 📖 About This Repository

This repository hosts the source code for the cheat sheets used in the **AY2025 EE6497 (Pattern Recognition & Deep Learning)** examinations. The content is designed to be concise yet comprehensive, stripping away redundant descriptions to maximize space for complex formulas, block diagrams, and mathematical models.

### ✨ Key Features
- 📐 **Maximized Space**: 4-column ultra-compact layout designed for quick peripheral scanning.
- 🚀 **Exam-Oriented**: Engineered specifically for speed-searching under intense exam conditions.
- 🔄 **Curriculum Aligned**: Synchronized with the latest syllabus and lecture progress.

## 📂 Repository Contents

| Status | Cheat Sheet | Target Coverage |
| :---: | :--- | :--- |
| ✅ | **[`/EE6497_Quiz1_Cheatsheet`](./EE6497_Quiz1_Cheatsheet)** | Fundamental concepts, early-semester topics. |
| ✅ | **[`/EE6497_Quiz2_Cheatsheet`](./EE6497_Quiz2_Cheatsheet)** | Mid-to-late semester advanced topics. |
| 🚧 | **`[EE6497_Final_Exam_Cheatsheet]`** | Comprehensive final exam summary *(Work in progress)*. |

---

## ⚠️ Important Disclaimer

> [!WARNING]
> **Before using these cheat sheets, please ensure you verify the following:**

1. **🎓 Examination Policy**: Academic regulations change frequently. **Strictly verify** if EE6497 is still conducted as an open-book exam for your current semester.
2. **🔍 Accuracy Check**: While every effort has been made to ensure mathematical accuracy, these documents may still contain typos or errata. **Double-check formulas** against official lecture notes.
3. **📅 Syllabus Alignment**: Lecture content evolves. Cross-reference this sheet with your current teaching materials and manually add any missing topics.

---

## 🛠️ Usage & Compilation

You can easily compile these cheat sheets using a local LaTeX environment tailored to your preferences, or simply use an online editor.

### 💻 Local Compilation
Navigate to the specific cheat sheet folder. Ensure you have a full TeX distribution installed (e.g., `TeX Live`, `MacTeX`), and run:

```bash
cd EE6497_Quiz1_Cheatsheet
pdflatex main.tex
```
> **Note:** You may need to run the `pdflatex` command 2-3 times consecutively to correctly resolve internal cross-references and spacing.

### ☁️ Online (Overleaf)
1. Compress the target folder (e.g., `EE6497_Quiz1_Cheatsheet`) into a `.zip` file.
2. Upload to [Overleaf](https://www.overleaf.com/).
3. Set your project compiler to **pdfLaTeX** in the left-hand menu.
4. Hit Compile!

### 🎨 Customization
The projects are modularized to facilitate easy updates:
*   📝 **Content (`main.tex`)**: To add a new topic within the multi-column layout, use the custom macro:
    ```latex
    \bulletPoint{Topic Name}:
    Your derivations or formulas here...
    ```
*   ⚙️ **Configuration (`preamble.tex`)**: Edit this file to manage package imports, alter page margins, tweak fonts, or define new mathematical macros.

---

## 🙌 Acknowledgements

This repository builds upon the excellent architectural foundation of [**2023_NTU_EE7401_Cheat_Sheet**](https://github.com/JiangpengLI86/2023_NTU_EE7401_Cheat_Sheet). 

While the underlying LaTeX structure originates from their fantastic open-source contribution, this repository represents a **significant restructuring and complete rewrite** customized exclusively for the **NTU EE6497 Pattern Recognition & Deep Learning** course. Massive thanks to the original author!

## ⚖️ License

This project is open-sourced under the **MIT License** - see the [`LICENSE`](LICENSE) file for details.

<br/>
<div align="center">
  <b>🌟 Hope this helps you ace the EE6497 exams! Good luck! 🚀</b>
</div>
