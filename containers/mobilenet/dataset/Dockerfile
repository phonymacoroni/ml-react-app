ARG BASE_VERSION=edge
FROM wpilib/axon-base:${BASE_VERSION}

RUN mkdir -p /opt/ml/model/tmp && \
    mkdir -p /opt/ml/model/out
COPY scripts /tensorflow/models/research/

WORKDIR /tensorflow/models/research/
ENTRYPOINT ["python", "tar_to_record.py", "--dir"]
