
FROM python:3.9

WORKDIR /demofastapi

COPY ./requirements.txt /fastapi/requirements.txt

RUN pip install --no-cache-dir --upgrade -r /demofastapi/requirements.txt

COPY ./app /demofastapi/app
 
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]
