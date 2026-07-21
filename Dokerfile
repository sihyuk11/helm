FROM python:3.12-slim

WORKDIR /app

COPY ins.txt .
RUN pip install --no-cache-dir -r ins.txt

COPY . .

EXPOSE 9986

CMD ["gunicorn", "--bind", "0.0.0.0:9986", "app:app"]
