<h1 align="center">Hi, I'm Richel Attafuah <img src="assets/bunny.gif" width="95" alt="cute bunny" /></h1>

<p align="center">
  <b>AI/ML Engineer &amp; Data Scientist</b><br>
  I build ML systems that hold up outside the notebook.<br>
  <sub><i>Richel makes tech easy.</i></sub>
</p>

<p align="center">
  <a href="https://richelcode.github.io"><img src="https://img.shields.io/badge/Portfolio-richelcode.github.io-0C2A4A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/richelattafuah/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/RichelCode"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
  <a href="mailto:richelattafuah@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://medium.com/@richelattafuah"><img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" alt="Medium"></a>
  <a href="https://www.youtube.com/@richelattafuah23"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube"></a>
</p>

---

## Featured Projects

### Spatio-Temporal Prediction of EV Charging Demand

<p align="center">
  <a href="https://richelcode.github.io/ev-charging-demand-demo/">
    <img src="assets/ev-demo.gif" width="880" alt="Interactive dashboard: GraphWaveNet-GRU-LSTM vs Random Forest, with a sensor-outage slider showing the baseline's error diverging as sensors go dark">
  </a>
</p>

Forecasts traffic flow **72 hours ahead across 1,821 Caltrans PeMS sensors** and maps it to EV charging load. The point isn't the clean-data score. It's what happens when the network degrades: **with 30% of sensors offline, the model holds 15.6% lower MAE than a Random Forest baseline, and stays more resilient at all 6 stations.** The baseline's error grows **2.8× faster** as sensors go dark, because the graph reconstructs a dead node from its neighbours while the baseline only sees a dead channel.

**Method:** GraphWaveNet encoder + GRU/LSTM refinement over an adaptive adjacency matrix, evaluated at 12/24/48/72 h horizons, with up to **9.8% MAE improvement** over the base GraphWaveNet at long horizons.

<p align="center">
  <a href="https://richelcode.github.io/ev-charging-demand-demo/"><img src="https://img.shields.io/badge/Live_Demo-Interactive_Dashboard-E8A23D?style=for-the-badge&logo=githubpages&logoColor=white" alt="Live Demo"></a>
  <a href="https://github.com/RichelCode/ev-charging-demand-demo"><img src="https://img.shields.io/badge/Demo_Repo-2E6FB8?style=for-the-badge&logo=github&logoColor=white" alt="Demo Repo"></a>
  <a href="https://github.com/RichelCode/Spatio-Temporal-Prediction-and-Coordination-of-EV-Charging-Demand-for-Power-System-Resilience"><img src="https://img.shields.io/badge/Thesis_Repo-0C2A4A?style=for-the-badge&logo=github&logoColor=white" alt="Thesis Repo"></a>
</p>

**Stack:** `Python` · `PyTorch` · `GraphWaveNet` · `GRU / LSTM` · `Spatio-Temporal Graphs` · `NumPy` · `Gradio`

<br>

### Reading the Grid: Solar-Cell Fault Detection

<p align="center">
  <a href="https://huggingface.co/spaces/RichelCode/reading-the-grid">
    <img src="assets/reading-the-grid.gif" width="880" alt="Live demo: selecting electroluminescence cell images, the model predicting faulty vs healthy with confidence, and a Grad-CAM heatmap in a drag-to-compare view">
  </a>
</p>

Catches **85.4% of faulty solar cells** from electroluminescence scans (84.8% accuracy on a held-out split of 394 cells), and shows you *where* it looked: a Grad-CAM heatmap you drag against the original, so an inspector can confirm the call instead of trusting a bare label. Recall is prioritized over precision (71.4%) on purpose, because a fault missed in the field costs far more than a false alarm a human waves off in review.

**Method:** ImageNet-pretrained ResNet18, fine-tuned on the ELPV dataset with a class-weighted loss. Unfreezing the last residual block lifted faulty recall from **0.72 to 0.85**. Ships as a single Docker container: a FastAPI inference server behind a React front end, deployed on Hugging Face Spaces.

<p align="center">
  <a href="https://huggingface.co/spaces/RichelCode/reading-the-grid"><img src="https://img.shields.io/badge/Live_Demo-Hugging_Face_Space-E8A23D?style=for-the-badge&logo=huggingface&logoColor=white" alt="Live Demo"></a>
  <a href="https://github.com/RichelCode/reading-the-grid"><img src="https://img.shields.io/badge/Repo-0C2A4A?style=for-the-badge&logo=github&logoColor=white" alt="Repo"></a>
</p>

**Stack:** `PyTorch` · `ResNet18` · `Grad-CAM` · `FastAPI` · `React` · `TypeScript` · `Docker` · `Hugging Face Spaces`

---

## Other Work

- **Coherent Hourly Traffic-Flow Forecasting**: hierarchical modeling &amp; reconciliation in R, keeping forecasts coherent across aggregation levels · [repo](https://github.com/RichelCode/Coherent-Hourly-Traffic-Flow-Forecasting-Hierarchical-Modeling-and-Reconciliation-in-R)
- **Multi-Seasonal Forecasting of NYC Bike Demand**: SARIMA vs TBATS vs Fourier-ARIMA on overlapping daily/weekly seasonalities in R · [repo](https://github.com/RichelCode/Multi-Seasonal-Time-Series-Forecasting-of-NYC-Bike-Demand-SARIMA-vs-TBATS-vs-Fourier-ARIMA)
- **Published in *Scientific African* (2024)**: stochastic population growth model for national health &amp; labor planning in Ghana · [paper](https://www.sciencedirect.com/science/article/pii/S2468227624003831)

---

## Recognition

- **2nd Runner-Up, StatsBank Hackathon**
- **First Class Honors Graduate** · 2nd Overall Outstanding Student Award (University of Ghana)
- **ENAR Travel Award** · Diversity Mentorship Program Travel Award · PharmaSUG Award
- **Lilly Leadership Institute (Cohort 14)**: first graduate student selected across Miami University
- **Women in Statistics and Data Science Conference 2025**: presented spatio-temporal forecasting research
- **Published in *Scientific African* (2024)**: [stochastic population growth model](https://www.sciencedirect.com/science/article/pii/S2468227624003831) for national health & labor planning in Ghana

---

## Teaching & Community

- **Graduate Teaching Assistant, STA 261 (Miami University)**: supported 310+ students; weekly R & JMP labs, office hours averaging 15+ visits
- **AI & Student Project Development Faculty Learning Community**: integrating AI tools into teaching across disciplines
- **Social Media & Communications Lead, WiMLDS Accra**: amplifying opportunities for women in AI & ML
- **Technical writer on [Medium](https://medium.com/@richelattafuah)**: Python, ML, and data science career content
- **[YouTube channel](https://www.youtube.com/@richelattafuah23)**: Python & data science (68% avg watch-through, well above platform average)

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## GitHub Activity

<p align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=RichelCode&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true" alt="Richel's GitHub stats">
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=RichelCode&layout=compact&theme=tokyonight&langs_count=8" alt="Top languages">
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=RichelCode&theme=tokyonight" alt="GitHub streak">
</p>

<p align="center"><i>Forecasting the future, one time step at a time.</i></p>
