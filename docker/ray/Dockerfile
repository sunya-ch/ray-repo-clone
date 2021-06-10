FROM rayproject/ray-deps:nightly
# For Click
ENV LC_ALL=C.UTF-8
ENV LANG=C.UTF-8

ENV PYTHON_VERSION=3.7.7
RUN wget https://s3-us-west-2.amazonaws.com/ray-wheels/latest/ray-2.0.0.dev0-cp37-cp37m-manylinux2014_x86_64.whl

RUN $HOME/anaconda3/bin/pip --no-cache-dir install `basename ray-2.0.0.dev0-cp37-cp37m-manylinux2014_x86_64.whl`[all] \
&& sudo rm `basename ray-2.0.0.dev0-cp37-cp37m-manylinux2014_x86_64.whl`