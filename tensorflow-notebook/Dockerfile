# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM zgsolucoes/scipy-notebook

LABEL maintainer="Jupyter Project <jupyter@googlegroups.com>"

# Install Tensorflow
RUN conda install --quiet --yes \
    'tensorflow=1.5*' \
    'keras=2.1*' && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/$NB_USER

# Extra packages
RUN conda install --quiet --yes 'opencv' 'six'
