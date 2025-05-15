FROM jupyter/base-notebook:python-3.10

# Copia los requirements
COPY requirements.txt /tmp/

# Instala los requirements
RUN pip install --upgrade pip && \
    pip install -r /tmp/requirements.txt
