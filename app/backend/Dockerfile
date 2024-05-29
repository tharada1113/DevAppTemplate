FROM python:3.11

RUN mkdir /code
WORKDIR /code
COPY requirements.lock /code/
RUN pip3 install -r requirements.lock
COPY . /code/

CMD ["python", "manage.py", "runserver", "--settings", "config.settings.development"]

