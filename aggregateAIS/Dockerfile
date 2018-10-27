FROM davesteps/base-ais

RUN R -e "devtools::install_github('davesteps/projectNickel')"

ARG proj_dir

# ARGs are buildtime ENVs are runtime so build ENV with R cmd to run
ENV Rcmd "projectNickel::aggregateAIS('${proj_dir}')"

RUN echo "$Rcmd"

#CMD ["R", "-e", "$Rcmd"]

ENTRYPOINT R -e $Rcmd