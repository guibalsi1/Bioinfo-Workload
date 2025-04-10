FROM bioconductor/bioconductor_docker:RELEASE_3_18

RUN pip install --upgrade pip setuptools wheel
RUN pip install notebook jupyterlab rpy2
RUN pip install numba
RUN apt-get update && apt-get install -y \
    wget \
    curl \
    unzip \
    build-essential \
    ncbi-blast+

RUN pip install biopython
RUN R -e "if (!requireNamespace('DESeq2')) BiocManager::install('DESeq2', ask=FALSE)"
RUN R -e "install.packages('IRkernel'); IRkernel::installspec(user = FALSE)"