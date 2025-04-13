FROM python:3.12.6

ENV PYTHONUNBUFFERED 1
ENV PYTHONPATH /app
WORKDIR /app

COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt

COPY . /app/

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]