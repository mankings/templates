FROM python:3.12.4-alpine

WORKDIR /backend

COPY ./requirements.txt /backend/

RUN pip install --no-cache-dir --upgrade -r /backend/requirements.txt

COPY ./src /backend/

CMD ["fastapi", "run", "src/main.py", "--port", "80"]
