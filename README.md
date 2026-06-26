# Hi, I'm Tanoj 👋

**I build ML and AI systems that make it to production, and I evaluate them honestly.**

Master's student at Northeastern University (graduating **December 2026**), focused on the engineering that turns models into systems people can actually use. Currently an **AI Engineer Intern at ProjectPathAI** (Boston), building production RAG with hybrid retrieval and multi-layer hallucination defense.

My work keeps coming back to one question: how do you take modern ML from a notebook to something dependable in production? In practice that means grounded, verifiable retrieval, deep-learning models built and trained from the ground up, and honest evaluation of where models break rather than just in-distribution metrics.

A lot of my recent projects happen to live in biology and healthcare, and I'm drawn to **drug discovery and computational biology**. But the core is the same wherever it's applied: production-grade ML engineering.

---

## 🔬 Featured projects

### [ProtLoc-AI](https://huggingface.co/spaces/Tanoj22/protloc-ai): protein localization and variant effect prediction
ESM-2 backbone with a custom **residue-attention classifier** that achieves **3.7× higher mutation sensitivity** than mean-pooled baselines. With no supervision, its attention concentrated on the residues corresponding to known nuclear-localization biology. Validated on disease-relevant variants. Live demo on HuggingFace Spaces.
`Python` · `PyTorch` · `ESM-2` · `HuggingFace` · `Three.js`

### MedAgent: multi-agent biomedical research assistant
A **LangGraph orchestrator** routes plain-English questions to tool-grounded specialist agents over hybrid RAG retrieval, with a **three-layer hallucination defense** that refuses to answer when it can't ground a claim. Production-grade agentic AI for biomedical literature search, deployed with a CI/CD pipeline.
`Python` · `LangGraph` · `ChromaDB` · `FastAPI` · `Docker`

### DenseNet121 variants for class-imbalanced breast cancer detection
CLAHE preprocessing, EMA weight averaging, and focal loss for mammogram classification. External validation on INbreast surfaced **probability-calibration failure under domain shift**, which I documented as the core blocker for clinical deployment rather than hiding behind in-distribution metrics.
`Python` · `PyTorch` · `DenseNet121` · `OpenCV`

### [Liver tumor segmentation from CT](https://github.com/tanoj22): 2D U-Net pipeline
**Dice 0.78 / IoU 0.70** on 20K balanced DICOM-converted slices, with a chunk-based training strategy designed to run on CPU-only hardware.
`Python` · `PyTorch` · `OpenCV` · `DICOM`

---

## 📄 Publications
- **[Early-Stage Identification of Tomato Leaf Diseases using VGG16 and MobileNet CNNs](https://www.macawpublications.com/Journals/index.php/MIJARCSE/article/view/7)**, Macaw IJARCSE
- **[A Review and Comprehensive Analysis of Recent Research in Crop Yield Prediction using ML Algorithms](https://ieeexplore.ieee.org/document/10689872)**, IEEE RAICS

## 🛠️ Tech
**ML/DL:** PyTorch, Hugging Face Transformers, scikit-learn, OpenCV · **LLM/RAG:** LangGraph, hybrid retrieval (BM25 + dense), RRF, cross-encoder reranking, ChromaDB, pgvector · **Engineering:** Python, SQL, FastAPI, Docker, GitHub Actions (CI/CD), MLflow, DVC, PostgreSQL

## 🎓 Background
**MS, Data Analytics Engineering**, Northeastern University (Dec 2026, GPA 3.89/4.00)
**BTech, Computer Science (AI/ML)**, CVR College of Engineering
**Computer Vision Intern, DRDO (India)**, where I built an SSD + VGG16 weakly-supervised object-localization framework from scratch in PyTorch.

---

## 📫 Get in touch
Happy to talk drug discovery, computational biology, and production ML engineering.

📧 [salehundam.s@northeastern.edu](mailto:salehundam.s@northeastern.edu) · 💼 [LinkedIn](https://linkedin.com/in/saitanojs) · 📞 +1 (857) 397-7730
