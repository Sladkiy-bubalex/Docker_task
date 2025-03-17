FROM python:3.12.2

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .
RUN python manage.py migrate

ENV PYTHONUNBUFFERED 1
ENV DJANGO_SETTINGS_MODULE=api_with_restrictions.settings

CMD ["python","manage.py","runserver","0.0.0.0:8000"]