from tensorflow/tensorflow:latest-py3

RUN apt-get update
RUN apt-get install -y wget texlive texlive-xetex python-pydot python-pydot-ng graphviz

RUN wget https://github.com/jgm/pandoc/releases/download/2.1/pandoc-2.1-1-amd64.deb
RUN dpkg -i pandoc-2.1-1-amd64.deb

ADD requirements.txt /notebooks
RUN pip install -r requirements.txt
