FROM python:3

ADD requirements.txt requirements.txt

RUN apt-get update && apt-get install -y \
    net-tools \
    iputils-ping \
    curl \
    && rm -rf /var/lib/apt/lists/*

RUN pip install -r requirements.txt
RUN mkdir /home/project

ENV LANGSMITH_API_KEY="{{ cookiecutter.langsmith_api_key }}"

EXPOSE 2024

WORKDIR /home/project

CMD ["langgraph", "dev", "--host", "0.0.0.0", "--port", "2024"]