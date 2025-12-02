FROM python:3.15.0a2-trixie
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . /app/
EXPOSE 5000 
CMD [ "gunicorn", "--bind", "0.0.0.0:5000", "main:app" ]