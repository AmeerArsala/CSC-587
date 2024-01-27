FROM mambaorg/micromamba:latest

USER root

WORKDIR /app

COPY environment.yaml .

RUN micromamba install --yes --name base -f environment.yaml
RUN micromamba clean --all --yes

ARG MAMBA_DOCKERFILE_ACTIVATE=1

#RUN pip install pymupdf unstructured