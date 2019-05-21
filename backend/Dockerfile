FROM python:3
ADD . /backend
WORKDIR /backend
RUN pip install -r requirements.txt
COPY . /backend

EXPOSE 8081

CMD ["python", "app.py"]