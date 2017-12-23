# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM zgsolucoes/scipy-notebook:latest-gpu

LABEL maintainer="Jupyter Project <jupyter@googlegroups.com>"

# Install Tensorflow
RUN conda install --quiet --yes \
    'tensorflow-gpu=1.3*' \
    'keras-gpu=2.0*' && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR
