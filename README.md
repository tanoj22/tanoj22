# Hi, I'm Tanoj 👋

**I build ML and AI systems that make it to production, and I evaluate them honestly.**

Master's student at Northeastern University (graduating **December 2026**), focused on the engineering that turns models into systems people can actually use. Currently a **Graduate Research Assistant in the D2R2 Lab at Northeastern**, building ML models (graph neural networks, interatomic potentials) that predict material properties directly from structure, replacing slow first-principles simulation. Previously an **AI Engineer Intern at ProjectPathAI** (Boston), where I owned the retrieval and grounding layer of a production RAG document assistant.

My work keeps coming back to one question: how do you take modern ML from a notebook to something dependable in production? In practice that means grounded, verifiable retrieval, deep-learning models built and trained from the ground up, and honest evaluation of where models break rather than just in-distribution metrics.

A lot of my recent projects happen to live in biology, chemistry, and materials science, and I'm drawn to **drug discovery and computational biology**. But the core is the same wherever it's applied: production-grade ML engineering.

---

## 🔬 Featured projects

### [Crystal-GNN](https://github.com/tanoj22/crystal-gnn): crystal property prediction from Materials Project
From-scratch **CGCNN-style graph neural network** on roughly 100K Materials Project structures. Cut formation-energy test MAE from 0.049 to **0.0425 eV/atom** (near the original paper's 0.039) by replacing atomic-number embeddings with engineered atom features, then reused the same backbone for metal vs. semiconductor classification at **0.87 accuracy, 0.933 ROC-AUC**. Shipped as a FastAPI/Docker inference service with GitHub Actions CI.
`Python` · `PyTorch Geometric` · `FastAPI` · `Docker`

### [ProtLoc-AI](https://huggingface.co/spaces/Tanoj22/protloc-ai): protein subcellular localization predictor
ESM-2 (650M-parameter protein language model) backbone with a custom **residue-level attention classifier** replacing mean pooling, trained on 28,303 DeepLoc proteins across 11 compartments. Reached **macro F1 0.738, AUROC 0.932** on a held-out test set (n=4,202), lifting F1 on the rarest compartment (Peroxisome) from 0.52 to 0.68. Live demo on HuggingFace Spaces.
`Python` · `PyTorch` · `ESM-2` · `HuggingFace`

### MedAgent: multi-agent biomedical research assistant
A **LangGraph orchestrator** routes plain-English questions to tool-grounded specialist agents (literature, molecule, protein) over hybrid BM25 + dense retrieval, reaching 100% recall@8 on a 150-query benchmark across 25K+ harvested PubMed abstracts. A **three-layer hallucination guard** retries under stricter constraints and refuses rather than guess when it can't ground a claim. Deployed as a Docker container with CI/CD, validated on a 22-case routing/refusal suite.
`Python` · `LangGraph` · `ChromaDB` · `FastAPI` · `Docker`

### DenseNet121 variants for class-imbalanced breast cancer detection
CLAHE preprocessing, EMA weight averaging, and focal loss for mammogram classification. External validation on INbreast surfaced **probability-calibration failure under domain shift**, which I documented as the core blocker for clinical deployment rather than hiding behind in-distribution metrics.
`Python` · `PyTorch` · `DenseNet121` · `OpenCV`

### [Liver tumor segmentation from CT](https://github.com/tanoj22): 2D U-Net pipeline
**Dice 0.78 / IoU 0.70** on 20K balanced DICOM-converted slices, with a chunk-based training strategy designed to run on CPU-only hardware.
`Python` · `PyTorch` · `OpenCV` · `DICOM`

---

## 📄 Publications
- **[Early-Stage Identification of Tomato Leaf Diseases using VGG16 and MobileNet CNNs](https://www.macawpublications.com/Journals/index.php/MIJARCSE/article/view/7)**, Macaw IJARCSE, Nov 2023
- **[A Review and Comprehensive Analysis of Recent Research in Crop Yield Prediction using ML Algorithms](https://ieeexplore.ieee.org/document/10689872)**, IEEE RAICS, Aug 2024

## 🛠️ Tech
**ML/DL:** PyTorch, PyTorch Geometric, Hugging Face Transformers, scikit-learn, OpenCV · **LLM/RAG:** LangGraph, hybrid retrieval (BM25 + dense), RRF, cross-encoder reranking, ChromaDB, pgvector · **Engineering:** Python, SQL, FastAPI, Docker, GitHub Actions (CI/CD), MLflow, DVC, PostgreSQL

## 🎓 Background
**MS, Data Analytics Engineering**, Northeastern University (Dec 2026, GPA 3.89/4.00)
**BTech, Computer Science (AI/ML)**, CVR College of Engineering
**Computer Vision Intern, DRDO (India)** — built an SSD + VGG16 weakly-supervised object-localization framework from scratch in PyTorch, reducing localization loss 89.7% (from 68 to 7) over 46 epochs.

---

## 📫 Get in touch
Happy to talk drug discovery, computational biology, and production ML engineering.

📧 [saitanojs@gmail.com](mailto:saitanojs@gmail.com) · 💼 [LinkedIn](https://linkedin.com/in/saitanojs) · 📞 +1 (857) 397-7730
