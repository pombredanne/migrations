FROM python:3.5-slim
RUN mkdir /project
WORKDIR /project
RUN useradd -u 1000 -m -s /bin/bash python
COPY dev/requirements.txt dev/setup.py /project/
RUN pip install --no-cache-dir -r requirements.txt \
    && pip install -e /project
USER python
