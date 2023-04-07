FROM python:3.9-slim

WORKDIR /home

COPY ./requirements.txt /home
RUN pip3 install -r requirements.txt -i https://pypi.jittor.org/simple -I
RUN pip3 install gradio -i https://pypi.tuna.tsinghua.edu.cn/simple

COPY ../../ /home

CMD python3 web_demo.py $JittorLLMs_MODEL
