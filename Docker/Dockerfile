FROM alpine:3.7
MAINTAINER Maciej Kofel
RUN apk update --no-cache && apk add python3 \
python2-dev \
py2-pip \ 
git \
bash

RUN git clone https://github.com/szkolasecurity/RFI-lab.git
WORKDIR RFI-lab
RUN pip2 install -r requirements.txt
CMD [ "python2", "./RFI.py" ]
