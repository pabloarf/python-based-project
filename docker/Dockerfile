FROM python:3.9 as runtime

LABEL maintainer="Pablo Ravera"

ENV APP_HOME /var/www/app

WORKDIR $APP_HOME

ADD requirements.txt $APP_HOME

RUN pip install -r requirements.txt

# COPY app to container
COPY . $APP_HOME

CMD [ "python", "./example.py" ]
