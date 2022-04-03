FROM python:3.7

RUN mkdir -p /pip

WORKDIR /pip


ARG PACKAGES="scipy pandas matplotlib seaborn"

RUN pip install ${PACKAGES} 

RUN pip freeze > requirements.txt

RUN pip download ${PACKAGES} 
