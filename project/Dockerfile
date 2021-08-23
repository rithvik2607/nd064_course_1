FROM python:2.7
LABEL maintainer="Rithvik Ayithapu"

COPY . /app
WORKDIR /app
RUN pip install -r ./techtrends/requirements.txt
RUN python ./techtrends/init_db.py

EXPOSE 3111
CMD ["python", "./techtrends/app.py"]