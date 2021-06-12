 FROM python:3.7

WORKDIR /app

COPY requirements.txt ./requirements.txt

RUN xargs -L 1 pip install < requirements.txt

EXPOSE 8501

COPY . /app

ENTRYPOINT ["streamlit","run"]

CMD ["app.py"]
