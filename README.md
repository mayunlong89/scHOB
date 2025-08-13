# scHOB
scHOB ([single-cell Human Organoid Bank](https://schob.su-lab.org/)) is a multi-omic single-cell database that consists of both scRNA-seq and scATAC-seq data on 10 kinds of widely-adopted human organoids (i.e., brain, lung, heart, eye, liver & bile duct, pancreas, intestine, kidney, and skin) spanning more than 1.5 million cells with 67 main cell types in 385 samples across 83 distinct protocols. The majority of cells (83.4%) underwent single cell transcriptomic profiling, while there were 226,874 cells (16.6%) derived from scATAC-seq datasets. Meanwhile, we also collected numerous single-cell datasets (N = 223,334 cells) on the de facto human fetal organs used for comparison and annotation analyses. To streamline data integration and analysis, we developed two unified pipelines for quality control and data processing of scRNA-seq and scATAC-seq data from human organoids.

![Workflow of scHOB](https://github.com/mayunlong89/scHOB/blob/main/figures/scHOB_framework.png)

 
The scHOB database has accessed online: https://schob.su-lab.org/

# Citations
1. Ma et al., Integrating polygenic signals and single-cell multiomics identifies cell type-specific regulomes critical for immune- and aging-related diseases and traits, `Nature Aging` (Under review), 2025
2. Ma et al., Sytematic dissection of pleiotropic loci and critical regulons in exhibitory neurons and microglia relevant to neuropsychiatric and ocular diseases, [Translational Psychiatry](https://rdcu.be/d7qof) 2025. For Preprint, please see the [Research Square](https://www.researchsquare.com/article/rs-4514542/v1), 2024.
3. Ma et al. Integration of human organoids single-cell transcriptomic profiles and human genetics repurposes critical cell type-specific drug targets for severe COVID-19. [Cell Proliferation](https://onlinelibrary.wiley.com/doi/full/10.1111/cpr.13558), 2024, and see related [Github codes](https://github.com/mayunlong89/scHuman_organoids_COVID19).

# scMORE method
This method is designed to prioritize cell type-specific TF-regulons relevant to diseases of interest, see [scMORE github](https://github.com/mayunlong89/scMORE).


# ctDRTF method (previous version of scMORE)
ctDRTF is the older/legacy version of scMORE and is no longer maintained. The code is provided as is for reference only—use with caution. see [ctDRTF github](https://github.com/mayunlong89/ctDRTF). For up-to-date features, bug fixes, and support, please use scMORE instead. see [scMORE github](https://github.com/mayunlong89/scMORE).


# Database construction and implementation
All the organoids and fetal scRNA-seq and scATAC-seq datasets were processed and deposited in the scHOB database ( https://schob.su-lab.org/). The back-end logic action of scHOB was implemented in Python (https://www.python.org/) with Django's web extension packages (https://www.djangoproject.com/), and Nginx (https://www.nginx.com/). The front-end web interface and interactive charts were displayed by JSP, CSS3, jQuery (https://jquery.com/), Bootstrap (https://bootstrapdocs.com/), and Echarts (https://echarts.apache.org/). The entire datasets of scHOB were stored with a lightweight database SQLite (https://sqlite.org/).
