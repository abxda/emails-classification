FROM tiangolo/uvicorn-gunicorn-fastapi:python3.7

ENV HTTP_PROXY=http://docker.for.win.localhost:3128
ENV HTTPS_PROXY=http://docker.for.win.localhost:3128

RUN pip install --no-cache-dir \
  minio \
  numpy==1.15.4 \
  pandas==0.24.2 \
  scikit-learn==0.20.3 
  
RUN pip install --no-cache-dir \
  scipy==1.2.1 \
  dill==0.2.8.2 \
  psycopg2-binary===2.7.4 

COPY ./app /app