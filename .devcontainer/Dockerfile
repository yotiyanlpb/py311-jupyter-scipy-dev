FROM jupyter/scipy-notebook:python-3.11.6

USER root

COPY resources/*.txt .

RUN apt update && apt install -y gcc && \
    echo ==== Installing requirements.txt ==== \
    pip install -r requirements.txt \
    conda list -e > conda_requirements.txt
