FROM python:3.9-buster
ENV PYTHONUNBUFFERED=1
WORKDIR /notebooks
COPY /docker/requirements.txt /notebooks//
RUN /usr/local/bin/python -m pip install --upgrade pip \
  && pip install -r requirements.txt --no-cache-dir
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--allow-root", "--no-browser"]
