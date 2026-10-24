# MaterialMind — AI Quality Inspector for Factories

**🏆 Built for: NVIDIA x Nebius Global AI Hackathon**

**Problem**: Manufacturing defects in raw materials cause billions of dollars in waste annually. Inconsistent material quality (micro-cracks, discoloration, foreign particles) only reveals itself downstream, causing costly production failures, recalls, and rework. Quality control teams spend excessive time manually inspecting batches — and still miss subtle anomalies.

**Solution**: Upload a material image; MaterialMind's AI flags visible anomalies, highlights suspicious regions with a heatmap, and produces a natural-language inspection report with defect type, severity, and recommended action.

**Built with**:
- 🤖 **Nemotron 3.5 Lightning** (NVIDIA open-source MoE model, 30B total / 3B active params) for natural language report generation
- 🧠 **Convolutional autoencoder** for computer vision anomaly detection
- 🛰️ **Nebius Token Factory** for scalable, cost-free inference
- 💻 **Streamlit** for the web interface

---

## 🎯 Hackathon Track Alignment

| Track | Alignment | Why It Fits |
|-------|-----------|-------------|
| **Best Apps and Agents** | ✅ Primary fit | Productivity tool anyone would use for quality control; "app someone would actually use" |
| **Personal AI** | ✅ Strong fit | Always-on private assistant keeping data under your control; persistent quality inspection memory |
| **Coding and Agentic Engineering** | ✅ Valid | Agent-based inspection pipeline; CV + LLM agent orchestration |
| **Physical AI** | ✅ Conceptual | Embodied quality agent sensing and acting on material defects; could extend to robotics |

**Key judge criteria addressed**:
- **Technological Implementation**: Uses NVIDIA open-source model (Nemotron 3.5 Lightning) + Nebius infrastructure
- **Design**: Complete coherent product experience — upload → analyze → receive report
- **Potential Impact**: Real problem (manufacturing waste) with measurable solution
- **Quality of Idea**: Creative use of model hierarchy (Lightning for everyday, 3 Ultra for complex decisions)

---

## 🚀 Quick Start

```bash
# 1. Clone
git clone <your-repo-url> materialmind
cd materialmind

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the demo
streamlit run app.py

# 4. Open browser at http://localhost:8510
# 5. Upload a material image (JPG, PNG, BMP, TIFF)
# 6. Get instant results:
#    - Anomaly heatmap highlighting suspicious regions
#    - Natural-language inspection report from Nemotron 3.5 Lightning
#    - Defect type, severity, and recommended action