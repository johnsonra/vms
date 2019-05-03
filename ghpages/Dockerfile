FROM jekyll/builder

MAINTAINER Randy Johnson <randall.johnson@nih.gov>

# this is a bit of a hack, but it causes some extra stuff to be installed
RUN git clone https://github.com/abcsFrederick/ABCSwebsite && \
    cd ABCSwebsite && \
    jekyll serve || echo Done

ADD build /usr/local/bin/build

EXPOSE 4000
