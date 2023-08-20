FROM python:3.8-slim

# Setup env
ENV PYTHONPATH=${PYTHONPATH}:${PWD} 
RUN pip3 install poetry
RUN poetry config virtualenvs.create false

# Install dependancies
COPY pyproject.toml . 
RUN poetry install --no-dev

# Copy code & sample source data (csv)
COPY code/* .
COPY *.csv .
