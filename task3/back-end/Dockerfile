FROM ubuntu:latest

# APT-ı yeniləyirik və Python-u yükləyirik
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip

# Flask-ı yükləmək üçün maneəni aradan qaldırırıq
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Flask-ı quraşdırırıq
RUN pip3 install flask
RUN pip3 install flask-cors
# İş qovluğunu təyin edirik
WORKDIR /app

# api.py faylını konteynerin içinə kopyalayırıq
COPY ./api.py /app/api.py

# Konteyner işə düşəndə Flask-ı işə salırıq
CMD ["python3", "api.py"]
