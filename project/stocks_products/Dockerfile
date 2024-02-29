FROM python:3.11-alpine

WORKDIR /app

COPY ./requirements.txt .

RUN pip install -r requirements.txt

ENV SECRET_KEY = 'mfno;iwijr09j;fsa;lkmu9uv309i40;3clk[p43,vir0943wiv,90[9w34cop]]'

ENV DEBUG = True

COPY . .

RUN python manage.py migrate

CMD [ "python", "manage.py", "runserver", "0.0.0.0:8000" ]
