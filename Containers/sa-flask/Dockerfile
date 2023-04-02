FROM python:3.8-slim
COPY sa /app
WORKDIR /app
RUN pip3 install -r requirements.txt && \
python3 -m textblob.download_corpora
ENTRYPOINT ["python3"]
CMD ["sentimentanalysis.py"]