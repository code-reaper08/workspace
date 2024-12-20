# pulling the 3.10 slim image
FROM python:3.8-slim

# creating a new src directory and switching to it
WORKDIR /src

# copy analytics folder to /src
COPY . .

RUN pip install --upgrade pip && pip install -r requirements.txt

EXPOSE 5153

ENV DB_USERNAME=myuser
ENV DB_PASSWORD=mypassword
ENV DB_HOST=127.0.0.1
ENV DB_PORT=5433
ENV DB_NAME=mydatabase

CMD python app.py