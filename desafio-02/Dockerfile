FROM ubuntu
RUN apt-get update -y && apt-get install python-pip python-dev build-essential -y && apt-get clean -y
COPY requirements.txt /
COPY color.py /
COPY hello.html /templates/
RUN ["pip","install","-r","requirements.txt"]
EXPOSE 9090
ENTRYPOINT ["python","color.py"]
