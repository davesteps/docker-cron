FROM openanalytics/r-base

MAINTAINER Tobias Verbeke "tobias.verbeke@openanalytics.eu"

# system libraries of general use
RUN apt-get update && apt-get install -y \
    sudo \
    pandoc \
    pandoc-citeproc \
    libcurl4-gnutls-dev \
    libcairo2-dev \
    libxt-dev \
    libssl-dev \
    libssh2-1-dev \
    libssl1.0.0 \
    libxml2-dev

RUN R -e "install.packages(c('aws.s3'), repos='https://cloud.r-project.org/')"
RUN R -e "install.packages(c('devtools'), repos='https://cloud.r-project.org/')"
RUN R -e "install.packages(c('plyr'), repos='https://cloud.r-project.org/')"
RUN R -e "install.packages(c('dplyr'), repos='https://cloud.r-project.org/')"
RUN R -e "install.packages(c('lubridate'), repos='https://cloud.r-project.org/')"
RUN R -e "install.packages(c('readr'), repos='https://cloud.r-project.org/')"
RUN R -e "install.packages(c('futile.logger'), repos='https://cloud.r-project.org/')"
