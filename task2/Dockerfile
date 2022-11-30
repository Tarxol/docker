FROM python:3.10

COPY ./requirements.txt /src/requirements.txt
RUN pip3 install --no-cache-dir --upgrade -r /src/requirements.txt

COPY . /task2

EXPOSE 8000

WORKDIR /task2

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "stocks_products.wsgi"]

