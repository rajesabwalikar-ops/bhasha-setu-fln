# Bhasha-Setu: Open Bilingual School Assessment & FLN Engine 🏫🌐

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

**Bhasha-Setu** is an open-source document automation engine and curriculum schema toolkit designed for bilingual public schools in India (focusing on **Kannada, Urdu, Hindi, and English** mediums). 

Teachers in bilingual government schools spend hundreds of hours manually formatting complex bidirectional (LTR + RTL) tables in Microsoft Word and Excel for **Lesson Based Assessments (LBA)** and **Foundational Literacy and Numeracy (FLN)** tracking. Bhasha-Setu automates this pipeline, converting lightweight JSON question banks into print-ready, state-compliant `.docx` and `.xlsx` files with preserved borders, Nastaliq/Naskh Urdu rendering, and Unicode Indic scripts.

## ✨ Core Features
- **Bidirectional Layout Engine:** Programmatically generates side-by-side Kannada/English (LTR) and Urdu (RTL) assessment tables in `.docx` and `.xlsx` without cell overflow or border corruption.
- **Standardized Curriculum Schemas:** JSON schemas aligned with state learning outcomes (DSERT/NCERT) enforcing strict blueprint constraints (e.g., 10 written + 5 oral mark splits, 4-option matching matrices).
- **Automated FLN Trackers:** Compiles A4 landscape baseline and endline evaluation sheets with pre-configured print areas and bilingual headers.
- **AI-Assisted Translation Validation:** Automated CI hooks to verify grade-level vocabulary appropriateness across regional scripts.

## 🚀 Quick Start
```bash
git clone [https://github.com/YOUR-USERNAME/bhasha-setu-fln.git](https://github.com/YOUR-USERNAME/bhasha-setu-fln.git)
cd bhasha-setu-fln
pip install -r requirements.txt
python src/generators/docx_lba_builder.py --input data/class_5_evs_bilingual.json --output build/
---

**2. Save (Commit) the file:**

1. Look at the **top-right corner** of the GitHub screen and click the green **"Commit changes..."** button.
2. A small pop-up window will appear in the middle of your screen.
3. In the box labeled **Commit message**, delete `Update README.md` and paste this instead:
   `docs: add project overview and architecture to README`
4. Make sure **"Commit directly to the `main` branch"** is selected.
5. Click the green **"Commit changes"** button at the bottom of that pop-up window.

---

### Next Step: Create `requirements.txt` (Takes 30 seconds!)

As soon as you click "Commit changes" above:

1. Click on **`<> Code`** (at the top-left of your screen) to return to the main page of your repository.
2. Click the **"Add file"** button (near the top right, just to the left of the green `<> Code` button) and select **"Create new file"**.
3. In the small box at the top that says **`Name your file...`**, type:
   `requirements.txt`
4. In the big empty text box below, paste these 4 lines:

```text
python-docx>=1.1.0
openpyxl>=3.1.2
jsonschema>=4.21.0
pytest>=8.0.0
