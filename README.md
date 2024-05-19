# scHOB
scHOB ([single-cell Human Organoid Bank](https://schob.su-lab.org/)) is a multi-omic single-cell database that consists of both scRNA-seq and scATAC-seq data on 10 kinds of widely-adopted human organoids (i.e., brain, lung, heart, eye, liver & bile duct, pancreas, intestine, kidney, and skin) spanning 1,366,380 cells with 67 main cell types in 385 samples across 83 distinct protocols. The majority of cells (83.4%) underwent single cell transcriptomic profiling, while there were 226,874 cells (16.6%) derived from scATAC-seq datasets. Meanwhile, we also collected numerous single-cell datasets (N = 223,334 cells) on the de facto human fetal organs used for comparison and annotation analyses. To streamline data integration and analysis, we developed two unified pipelines for quality control and data processing of scRNA-seq and scATAC-seq data from human organoids.

![Workflow of scHOB](https://github.com/mayunlong89/scHOB/blob/main/figures/Picture_1.png)

 
The scHOB database has accessed online: https://schob.su-lab.org/

# Citations
1. Ma et al., Systematic dissection of cell type-specific phenotype-relevant regulomes from single-cell transcriptomic and epigenomic atlases of human organoids, medRvix, 2024
2. Ma et al. Integration of human organoids single-cell transcriptomic profiles and human genetics repurposes critical cell type-specific drug targets for severe COVID-19. [Cell Proliferation, 2024, e13558](https://onlinelibrary.wiley.com/doi/full/10.1111/cpr.13558), and see related [Github codes](https://github.com/mayunlong89/scHuman_organoids_COVID19).

# ctDRTF method
This method is designed to prioritize cell type-specific TFs relevant to diseases of interest, see [Link](https://github.com/mayunlong89/ctDRTF)


# Database construction and implementation
All the organoids and fetal scRNA-seq and scATAC-seq datasets were processed and deposited in the scHOB database ( https://schob.su-lab.org/). The back-end logic action of scHOB was implemented in Python (https://www.python.org/) with Django's web extension packages (https://www.djangoproject.com/), and Nginx (https://www.nginx.com/). The front-end web interface and interactive charts were displayed by JSP, CSS3, jQuery (https://jquery.com/), Bootstrap (https://bootstrapdocs.com/), and Echarts (https://echarts.apache.org/). The entire datasets of scHOB were stored with a lightweight database SQLite (https://sqlite.org/).
