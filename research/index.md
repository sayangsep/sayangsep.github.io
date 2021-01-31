---
layout: page
title: Research
tags: [research, sayan, ghosal, Jhu, graduate]
modified: 2020-01-08T20:53:07.573882-04:00
comments: false
---

 My research is focused on multi view representation learning. We try to build data modality agnostic interpretable models for biomarker selection and disease classification. My most recent research focuses on building graph based deep learning models that leverages the correlated structures shared between different data modalities (e.g. Magnetic Resonance Imaging, Genetic Data) for disease classification.

# Recent Works
---

### G-MIND: An End-to-End Multimodal Imaging-Genetics Framework for Biomarker Identification and Disease Classification

We propose a novel deep neural network architecture to integrate imaging and genetics data, as guided by diagnosis, while preserving interpretability. Our model consists of an encoder, a decoder and a classifier. The encoder learns a non-linear subspace shared between the input data modalities. The classifier and the decoder act as regularizers to ensure that the low-dimensional encoding captures predictive differences between patients and controls. We use a learnable dropout layer to extract interpretable biomarkers from the data, and our unique training strategy can easily accommodate missing data modalities across subjects. We have evaluated our model on a population study of schizophrenia that includes two functional MRI (fMRI) paradigms and Single Nucleotide Polymorphism (SNP) data. Using 10-fold cross validation, we demonstrate that our model achieves better classification accuracy than baseline methods, and that this performance generalizes to a second dataset collected at a different site. The biomarkers identified by our model are closely associated with the well-documented deficits in schizophrenia.\\
[ArXiv](https://arxiv.org/abs/2101.11656)
<head>
<style>
figure {
  text-align: center;
}
figcaption {
  text-align: left;
}
</style>
</head>

<figure>
<p class="aligncenter">
    <img src="/images/gmind.png" alt="centered image" style="width:90%"/>
</p>
  <figcaption>
<head>
<script type="text/javascript" src="latexit.js"></script>
<script type="text/javascript">
LatexIT.add('p',true);
</script>
</head>
<body>
<p>G-MIND architecture. The inputs $\{\mathbf{i}_1, \mathbf{i}_2\}$ and $\{\mathbf{g}\}$ corresponds to the two imaging modalities and genetic data, respectively. $\mathcal{E}_i(\cdot)$ and $\mathcal{D}_i(\cdot)$ captures the encoding and decoding operations, and $\mathcal{Y}(\cdot)$ captures the classification operation. $\mathbf{z}_{i}$  is the learnable dropout mask, and $\mathbf{\ell}^n$ is the low dimensional latent space.</p>
</body>
</figcaption>
</figure>
---

### Bridging Imaging, Genetics, and Diagnosis in a Coupled Low-Dimensional Framework


We propose a joint dictionary learning framework that couples imaging and genetics data in a low dimensional subspace as guided by clinical diagnosis. We use a graph regularization penalty to simultaneously capture inter-regional brain interactions and identify the representative set anatomical basis vectors that span the low dimensional space. We further employ group sparsity to find the representative set of genetic basis vectors that span the same latent space. Finally, the latent projection is used to classify patients versus controls. We have evaluated our model on two task fMRI paradigms and single nucleotide polymorphism (SNP) data from schizophrenic patients and matched neurotypical controls. We employ a ten fold cross validation technique to show the predictive power of our model. We compare our model with canonical correlation analysis of imaging and genetics data and random forest classification. Our approach shows better prediction accuracy on both task datasets. Moreover, the implicated brain regions and genetic variants underlie the well documented deficits in schizophrenia.\\
[Link](https://link.springer.com/chapter/10.1007/978-3-030-32251-9_71)
<head>
<style>
figure {
  text-align: center;
}
figcaption {
  text-align: left;
}
</style>
</head>

<figure>
<p class="aligncenter">
    <img src="/images/joint.png" alt="centered image" style="width:90%"/>
</p>
  <figcaption>
<head>
<script type="text/javascript" src="latexit.js"></script>
<script type="text/javascript">
LatexIT.add('p',true);
</script>
</head>
<body>
<p>The generative process linking imaging ( $\mathbf{f}_m$), genetics ( $\mathbf{g}_m$), and diagnosis ( $y_m$). The imaging model is shown as a linear projection. The genetics model parallels this, whereas the classification is based on a logistic regression.</p>
</body>
</figcaption>
</figure>
---

### A generative-predictive framework to capture altered brain activity in fMRI and its association with genetic risk: application to Schizophrenia


We present a generative-predictive framework that captures the differences in regional brain activity between a neurotypical cohort and a clinical population, as guided by patient-specific genetic risk. Our model assumes that the functional activations in the neurotypical subjects are distributed around a population mean, and that the altered brain activity in neuropsychiatric patients is defined via deviations from this neurotypical mean. We employ group sparsity to identify a set of brain regions that simultaneously explain the salient functional differences and specify a set of basis vector, that span the low dimensional data subspace. The patient-specific projections onto this subspace are used as feature vectors to identify multivariate associations with genetic risk. We have evaluated our model on a task-based fMRI dataset from a population study of schizophrenia. We compare our model with two baseline methods, regression using Least Absolute Shrinkage and Selection Operator (LASSO) and Random Forest (RF) regression, which establishes direct association between the brain activity during a working memory task and schizophrenia polygenic risk. Our model demonstrates greater consistency and robustness across bootstrapping experiments than the machine learning baselines. Moreover, the set of brain regions implicated by our model underlie the well documented executive cognitive deficits in schizophrenia.\\
[Link](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/10949/1094927/A-generative-predictive-framework-to-capture-altered-brain-activity-in/10.1117/12.2511220.short?SSO=1)
<head>
<style>
figure {
  text-align: center;
}
figcaption {
  text-align: left;
}
</style>
</head>

<figure>
<p class="aligncenter">
    <img src="/images/joint_model.jpg" alt="centered image" style="width:90%"/>
</p>
  <figcaption>
<head>
<script type="text/javascript" src="latexit.js"></script>
<script type="text/javascript">
LatexIT.add('p',true);
</script>
</head>
<body>
<p>The joint modelling framework to capture brain activity and genetic risk. The gray box represents the generative part of the model for a single schizophrenia patient. We captured altered brain activity in the patients as deviations from the population mean. The major contribution of the anatomical regions to overall deviation are shown as surface plots in the yellow box. The green box is the predictive part of the model that track the genetic risk as linear regression.</p>
</body>
</figcaption>
</figure>
---

# Past Research

---

### Deep Deformable Image Registration


Deformable registration is ubiquitous in medical image analysis. Many deformable registration methods minimize sum of squared difference (SSD) as the registration cost with respect to deformable model parameters. In this work, we construct a tight upper bound of the SSD registration cost by using a fully convolutional neural network (FCNN) in the registration pipeline. The upper bound SSD (UB-SSD) enhances the original deformable model parameter space by adding a heatmap output from FCNN. Next, we minimize this UB-SSD by adjusting both the parameters of the FCNN and the parameters of the deformable model in coordinate descent. Our coordinate descent framework is end-to-end and it can work with any deformable registration method that uses SSD. We demonstrate experimentally that our method enhances the accuracy of deformable registration algorithms significantly on two publicly available 3D brain MRI data sets.\\
[Link](https://www.sciencedirect.com/science/article/abs/pii/S0167865517301708)
<head>
<style>
figure {
  text-align: center;
}
figcaption {
  text-align: left;
}
</style>
</head>

<figure>
<p class="aligncenter">
    <img src="/images/deform.png" alt="centered image" style="width:60%"/>
</p>
  <figcaption>
<head>
<script type="text/javascript" src="latexit.js"></script>
<script type="text/javascript">
LatexIT.add('p',true);
</script>
</head>
<body>
<p>Top left: A moving image slice; top right: a fixed image slice; bottom left: residual image from demons. bottom right: residual using DDR+demons.</p>
</body>
</figcaption>
</figure>
---

### A novel non-rigid registration algorithm for zebrafish larval images


Precise three-dimensional mapping of a large number of gene expression patterns, neuronal types and connections to an anatomical reference helps us to understand the vertebrate brain and its development. Zebrafish has evolved as a model organism for such study. In this paper, we propose a novel non-rigid registration algorithm for volumetric zebrafish larval image datasets. A coarse affine registration using the L-BFGS algorithm is applied first on the moving dataset. We then divide this coarsely registered moving image and the reference image into a union of overlapping patches. Minimum weight bipartite graph matching algorithm is employed to find the correspondence between the two sets of patches. The corresponding patches are then registered using the diffeomorphic demons method with proper intra-patch regularization. For each voxel lying in the overlapping regions, we impose inter-patch regularization through a composite transformation obtained from the adjacent transformation fields. Experimental results on four multi-view confocal 3D datasets show the advantage of the proposed solution over the existing ViBE-Z software.\\
[Link](https://ieeexplore.ieee.org/document/8036827)
<head>
<style>
figure {
  text-align: center;
}
figcaption {
  text-align: left;

}
</style>
</head>

<figure>
<p class="aligncenter">
    <img src="/images/abc.jpg" alt="centered image" style="width:60%"/>
</p>
  <figcaption>
<head>
<script type="text/javascript" src="latexit.js"></script>
<script type="text/javascript">
LatexIT.add('p',true);
</script>
</head>
<body>
<p> Top Left: Moving Image, Top Right: Fixed Image, Bottom Left:
Registration using our method, Bottom Right: Registration using VibeZ. All implementations are done in 3D and all results are shown for the same 2D slice of dataset 2.</p>
</body>
</figcaption>
</figure>
