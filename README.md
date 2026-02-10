<!DOCTYPE html>
<html lang="en">


<body>

<h1>Bridging Trust and Automation in Smart Waste Management through Explainable AI</h1>

<p>
A deep learning–based waste image classification framework integrating calibration,
explainable artificial intelligence, and semantic analysis to support reliable and
deployment-aware Organic versus Recycling waste segregation.
</p>

<hr>

<h2>Project Overview</h2>

<p>
This repository contains the implementation code developed for the Master’s dissertation
titled <em>“Bridging Trust and Automation in Smart Waste Management through Explainable AI”</em>,
submitted in partial fulfilment of the requirements for the MSc in Artificial Intelligence
and Machine Learning at Liverpool John Moores University (LJMU).
</p>

<p>
The project investigates automated waste image classification with an emphasis on
<strong>trustworthiness, interpretability, and reliability</strong>, rather than focusing solely
on maximising classification accuracy. Waste classification is framed as a
deployment-oriented decision support problem operating under real-world visual ambiguity,
class imbalance, and uncertainty.
</p>

<hr>

<h2>Technologies Used</h2>

<ul>
    <li><strong>Programming Language:</strong> Python</li>
    <li><strong>Deep Learning Frameworks:</strong> PyTorch, Torchvision</li>
    <li><strong>Data Processing:</strong> NumPy, Pandas</li>
    <li><strong>Evaluation and Metrics:</strong> Scikit-learn</li>
    <li><strong>Visualisation:</strong> Matplotlib, Seaborn</li>
    <li><strong>Explainable AI (XAI):</strong> Grad-CAM, LIME</li>
    <li><strong>Uncertainty Estimation:</strong> Monte Carlo Dropout</li>
    <li><strong>Vision–Language Models:</strong> CLIP</li>
    <li><strong>Execution Environment:</strong> Jupyter Notebook</li>
</ul>

<hr>

<h2>Dataset Information</h2>

<p>
This study uses the publicly available <strong>Waste Classification Dataset</strong> hosted on Kaggle:
</p>

<p>
<a href="https://www.kaggle.com/datasets/techsash/waste-classification-data/data" target="_blank">
https://www.kaggle.com/datasets/techsash/waste-classification-data
</a>
</p>

<p>
The dataset contains labelled images representing common waste materials, including:
plastic, glass, metal, paper, cardboard, organic waste, and trash. Images exhibit
realistic variability in lighting, background, orientation, and object condition,
reflecting challenges encountered in practical waste management settings.
</p>

<p>
For the purposes of this research, material-level labels are mapped to a binary
classification task:
</p>

<ul>
    <li><strong>Organic</strong></li>
    <li><strong>Recycling</strong></li>
</ul>

<p>
This binary formulation aligns with operational waste segregation pipelines, where
coarse separation is typically performed prior to downstream material recovery or
manual inspection.
</p>

<p>
The dataset itself is not included in this repository due to licensing and size
constraints. Users must download the dataset independently from Kaggle and configure
the dataset path within the notebook before execution.
</p>

<hr>

<h2>What is Explainable Artificial Intelligence (XAI)?</h2>

<p>
Explainable Artificial Intelligence (XAI) refers to a set of techniques designed to make
the decision-making processes of machine learning models transparent and interpretable
to human users.
</p>

<p>
In public-facing and environmental domains such as waste management, opaque “black-box”
models can undermine trust and limit real-world adoption. XAI techniques enable users
to understand which image regions or features influence model predictions and whether
those predictions are based on semantically meaningful cues.
</p>

<p>
In this project, XAI is used not merely for visual illustration, but as an
<strong>analytical tool</strong> to examine model behaviour, diagnose failure modes, and assess
confidence reliability.
</p>

<hr>

<h2>Methodology (Summary)</h2>

<p>
The experimental framework follows a structured, reproducible pipeline consisting of:
</p>

<ul>
    <li>Data preprocessing and augmentation</li>
    <li>Transfer learning using multiple CNN architectures</li>
    <li>Binary Organic/Recycling classification</li>
    <li>Performance evaluation using standard classification metrics</li>
    <li>Model calibration and uncertainty estimation</li>
    <li>Explainability analysis using Grad-CAM and LIME</li>
    <li>Semantic exploration using CLIP-based vision–language representations</li>
</ul>

<p>
All models are trained and evaluated under consistent experimental conditions to ensure
fair comparison and robust interpretation of results.
</p>

<hr>

<h2>Analysis (Brief Overview)</h2>

<p>
The analysis goes beyond aggregate accuracy and examines how models behave under
conditions of visual ambiguity and class overlap. Confusion matrices, ROC curves,
and precision–recall curves are used to assess classification behaviour across classes.
</p>

<p>
Calibration analysis evaluates whether predicted confidence scores align with empirical
correctness, using Expected Calibration Error and reliability diagrams. Uncertainty
estimation highlights cases where model predictions are less reliable.
</p>

<p>
Explainability analysis reveals that many misclassifications are driven by texture
ambiguity, object fragmentation, and contextual bias rather than architectural
limitations. These findings suggest dataset-level challenges that are critical for
deployment-aware evaluation.
</p>

<hr>

<h2>Discussion (Brief)</h2>

<p>
Results demonstrate that high classification accuracy alone is insufficient for
trustworthy deployment. Models with similar accuracy can differ substantially in
confidence reliability and explanation behaviour.
</p>

<p>
The integration of explainability and calibration highlights trade-offs between
performance, reliability, and computational efficiency, reinforcing the need for
holistic evaluation in applied AI systems.
</p>

<hr>

<h2>How to Use This Repository 🚀</h2>

<ol>
    <li>Clone the repository to your local machine.</li>
    <li>Download the dataset from the Kaggle link provided above.</li>
    <li>Update the dataset path in the Jupyter notebook accordingly.</li>
    <li>Open and run the notebook sequentially to reproduce experiments.</li>
</ol>

<p>
The notebook is structured to support step-by-step execution and inspection of each
experimental stage.
</p>

<hr>

<h2>Conclusions 📈</h2>

<p>
This project demonstrates that waste image classification should be evaluated as a
multidimensional problem encompassing accuracy, calibration, interpretability, and
deployment constraints. The findings support a shift away from purely accuracy-centred
benchmarking toward more responsible and transparent AI evaluation practices.
</p>

<p>
By integrating explainable AI and semantic reasoning, the study contributes a
deployment-aware perspective that is directly relevant to real-world smart waste
management systems.
</p>

<hr>

<h2>Acknowledgements</h2>

<p>
This work was completed as part of the MSc Artificial Intelligence and Machine Learning
programme at Liverpool John Moores University.
</p>

<p>
The author acknowledges the guidance of academic supervisors, the support of peers,
and the availability of open-source tools and publicly available datasets that made
this research possible.
</p>

<p>
This research makes use of the publicly available <em>Waste Classification Dataset</em>
hosted on Kaggle and authored by <strong>Techsash</strong>.
The author gratefully acknowledges the dataset creator for making the data openly
accessible to the research community, thereby enabling experimentation, benchmarking,
and reproducible research in automated waste classification.
</p>

<p>
The availability of this dataset was instrumental in supporting the evaluation of
deep learning models under realistic visual conditions, including material ambiguity
and class overlap, which are central to the objectives of this study.
</p>

<p>
Additional acknowledgement is extended to the developers and contributors of the
open-source libraries and tools used in this work, as well as to the academic supervisors
and peers associated with Liverpool John Moores University who provided guidance and
support throughout the research process.
</p>

<hr>

<h2>Author</h2>

<p>
<strong>Bhatti Prathvi Ghanshyambhai</strong><br>
MSc Artificial Intelligence and Machine Learning<br>
Liverpool John Moores University
</p>

<p>
LinkedIn:
<a href="https://linkedin.com/in/prathvibhatti08" target="_blank">
linkedin.com/in/prathvibhatti08
</a>
</p>

<p>
GitHub:
<a href="https://github.com/poronita" target="_blank">
github.com/poronita
</a>
</p>

<p>
This repository is provided for academic and research purposes only.
</p>

</body>
</html>
