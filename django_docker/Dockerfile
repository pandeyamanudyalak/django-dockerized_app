FROM python:3.8


COPY requirements.txt requirements.txt

RUN pip install --no-cache -r requirements.txt



COPY . code


WORKDIR /code

EXPOSE 8000

ENTRYPOINT [ "python3","manage.py"]
CMD [ "runserver","0.0.0.0:8000" ]