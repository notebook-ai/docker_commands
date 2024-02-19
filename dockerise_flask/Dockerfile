FROM python

RUN apt-get update && apt-get install -y
	
COPY . /app

RUN pip install --upgrade pip && pip install -r ./app/requirements.txt
ENTRYPOINT Flask_APP=/app/main.py flask run --host=0.0.0.0 --port=8080