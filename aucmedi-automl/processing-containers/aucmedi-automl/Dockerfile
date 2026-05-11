FROM ghcr.io/frankkramer-lab/aucmedi:v0.11.0

LABEL IMAGE="aucmedi-automl"
LABEL BUILD_IGNORE="False"

RUN mkdir -p /home/kaapana/aucmedi.data/training
RUN mkdir -p /home/kaapana/aucmedi.data/test

COPY clinical_data_TCIA_RHUH-GBM_with_classification_formatted.csv \
    /home/kaapana/aucmedi.data/training
COPY processing-container.json /

WORKDIR /home/kaapana/aucmedi.data