FROM python:3.12-slim

ENV FLASK_APP hello.py

# install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . /pra2

WORKDIR /pra2

# run-time configuration
EXPOSE 5001

CMD ["flask", "run", "--host", "0.0.0.0", "--port", "5001"]
