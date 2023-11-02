# scHOB
scHOB (single-cell Human Organoid Bank) is a multi-omic single-cell database that consists of both scRNA-seq and scATAC-seq data on 10 kinds of widely-adopted human organoids (i.e., brain, lung, heart, eye, liver & bile duct, pancreas, intestine, kidney, and skin) spanning 1,366,380 cells with 67 main cell types in 385 samples across 83 distinct protocols.

The scHOB database has accessed online: https://schob.su-lab.org/

Please cite: 
1. Ma et al. Integrated analysis of single-cell transcriptomic and epigenomic atlas of organoids uncovers core regulomes of human diseases. bioRvix, 2023.
2. Ma et al. Integration of human organoids single-cell transcriptomic profiles and human genetics repurposes critical cell type-specific drug targets for severe COVID-19. Cell Proliferation, 2023, e13558.



# Database construction and implementation
All the organoids and fetal scRNA-seq and scATAC-seq datasets were processed and deposited in the scHOB database (http://schob.wmu-bio-data.top/). The back-end logic action of scHOB was implemented in Python (https://www.python.org/) with Django's web extension packages (https://www.djangoproject.com/), and Nginx (https://www.nginx.com/). The front-end web interface and interactive charts were displayed by JSP, CSS3, jQuery (https://jquery.com/), Bootstrap (https://bootstrapdocs.com/), and Echarts (https://echarts.apache.org/). The entire datasets of scHOB were stored with a lightweight database SQLite (https://sqlite.org/).
