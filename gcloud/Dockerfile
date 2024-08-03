FROM gcr.io/google.com/cloudsdktool/google-cloud-cli:latest
RUN apt update
RUN apt install -y python3 python3-dev python3-venv python3-pip wget
RUN mkdir /app
COPY requirements.txt /app
WORKDIR /app
RUN pip3 install -r requirements.txt