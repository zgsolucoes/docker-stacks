# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM zgsolucoes/scipy-notebook

LABEL maintainer="Jupyter Project <jupyter@googlegroups.com>"

# Install Tensorflow
RUN conda install --quiet --yes \
    'tensorflow=1.3*' \
    'keras=2.0*' && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR
    
# Extra packages for Summer School
RUN conda install --quiet --yes \
    'gensim' \
    'boto3' \
    'nltk' \
    'tqdm' \
    'imageio'

RUN python -m nltk.downloader all
