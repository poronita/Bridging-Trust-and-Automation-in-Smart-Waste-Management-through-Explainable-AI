<!DOCTYPE html>
<html lang="en">


<body>

<h1>Bridging Trust and Automation in Smart Waste Management through Explainable AI</h1>

<p>
A deep learning–based waste image classification framework integrating calibration,
explainable AI, and semantic analysis to support reliable and deployment-aware
Organic vs Recycling waste segregation.
</p>

<hr>

<h2>Project Overview</h2>

<p>
This repository contains the implementation code developed for a Master’s dissertation
submitted as part of the MSc in Artificial Intelligence and Machine Learning at
Liverpool John Moores University (LJMU).
</p>

<p>
The project investigates automated waste classification with a focus on
<strong>trustworthiness, interpretability, and real-world deployment suitability</strong>.
Rather than treating waste classification as a closed accuracy optimisation task,
the study frames it as a reliability-sensitive decision support system operating
under realistic uncertainty and visual ambiguity.
</p>

---

<h2>Technologies Used</h2>

<ul>
    <li><strong>Programming Language:</strong> Python</li>
    <li><strong>Deep Learning Frameworks:</strong> PyTorch, Torchvision</li>
    <li><strong>Data Processing:</strong> NumPy, Pandas</li>
    <li><strong>Model Evaluation:</strong> Scikit-learn</li>
    <li><strong>Visualisation:</strong> Matplotlib, Seaborn</li>
    <li><strong>Explainable AI:</strong> Grad-CAM, LIME</li>
    <li><strong>Uncertainty Estimation:</strong> Monte Carlo Dropout</li>
    <li><strong>Vision–Language Models:</strong> CLIP</li>
    <li><strong>Environment:</strong> Jupyter Notebook</li>
</ul>

---

<h2>Dataset Information</h2>

<p>
The experiments utilise a publicly available waste image dataset containing material-level
annotations such as plastic, glass, metal, paper, cardboard, organic waste, and trash.
</p>

<p>
For this study, material-level labels are mapped to a binary classification task:
</p>

<ul>
    <li><strong>Organic</strong></li>
    <li><strong>Recycling</strong></li>
</ul>

<p>
This formulation aligns with real-world waste management workflows, where coarse
segregation is typically performed prior to downstream material recovery.
</p>

<p>
Due to licensing and size constraints, the dataset is not included in this repository.
Users must obtain the dataset independently and configure dataset paths accordingly.
</p>

---

<h2>What is Explainable AI (XAI)?</h2>

<p>
Explainable Artificial Intelligence (XAI) refers to techniques that make the decisions
of machine learning models transparent and interpretable to human users.
</p>

<p>
In high-stakes or public-facing domains such as waste management, opaque
black-box models can undermine trust and operational reliability. XAI methods
help reveal <em>why</em> a model makes a particular prediction, rather than only
reporting the predicted class.
</p>

<p>
This project uses XAI not merely for visual illustration, but as an
<strong>analytical tool</strong> to diagnose error patterns, confidence misalignment,
and dataset-driven ambiguity.
</p>

---

<h2>Methodology (Summary)</h2>

<p>
The methodological pipeline consists of the following stages:
</p>

<ul>
    <li>Data preprocessing and augmentation</li>
    <li>Transfer learning using multiple CNN architectures</li>
    <li>Binary Organic/Recycling classification</li>
    <li>Performance evaluation using standard metrics</li>
    <li>Model calibration and uncertainty estimation</li>
    <li>Explainability analysis using Grad-CAM and LIME</li>
    <li>Semantic exploration using CLIP</li>
</ul>

<p>
All models are evaluated under consistent experimental conditions to enable
meaningful comparison.
</p>

---

<h2>Analysis and Results (Summary)</h2>

<p>
The analysis examines not only classification accuracy, but also:
</p>

<ul>
    <li>Misclassification asymmetry</li>
    <li>Confidence reliability and calibration</li>
    <li>Computational efficiency</li>
    <li>Explanation consistency across XAI methods</li>
</ul>

<p>
Results indicate that no single architecture dominates across all evaluation dimensions.
Instead, trade-offs emerge between accuracy, calibration stability, and efficiency,
highlighting the importance of holistic model assessment.
</p>

---

<h2>Discussion (Summary)</h2>

<p>
The findings suggest that many misclassifications are driven by intrinsic dataset
ambiguity rather than architectural limitations. Visual texture overlap, object
fragmentation, and contamination play a significant role in classification errors.
</p>

<p>
Explainability and calibration analysis demonstrate that high accuracy alone is
insufficient for deployment-ready systems. Reliable confidence estimation and
transparent decision-making are essential for trustworthy automation.
</p>

---

<h2>Repository Structure</h2>

<pre>
.
├── waste-classification-organic-recycling.ipynb
├── data/            (dataset not included)
├── models/          (saved model checkpoints)
├── outputs/         (plots and visualisations)
├── README.html
</pre>

---

<h2>Reproducibility</h2>

<p>
The notebook is organised sequentially to support step-by-step execution.
Pseudocode describing the logical workflow is provided in the accompanying thesis
to enhance methodological transparency.
</p>

---

<h2>Acknowledgements</h2>

<p>
This work was completed as part of the MSc Artificial Intelligence and Machine Learning
programme at Liverpool John Moores University.
</p>

<p>
The author acknowledges the guidance of academic supervisors, the support of peers,
and the availability of open-source tools and datasets that enabled this research.
</p>

---

<h2>Author Information</h2>

<p>
<strong>Bhatti Prathvi Ghanshyambhai</strong><br>
MSc Artificial Intelligence and Machine Learning<br>
Liverpool John Moores University
</p>

<p>
🔗 LinkedIn:
<a href="https://linkedin.com/in/prathvibhatti08" target="_blank">
linkedin.com/in/prathvibhatti08
</a>
</p>

<p>
🔗 GitHub:
<a href="https://github.com/poronita" target="_blank">
github.com/poronita
</a>
</p>

<footer>
<p>
This repository is provided for academic and research purposes only.
If you reference or reuse this work, please cite the associated dissertation.
</p>
</footer>

</body>
</html>
