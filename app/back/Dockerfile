FROM python:3.9

WORKDIR /workspaces/lab-docker-ahmedmaaloul/app/back

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 5000

ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0

CMD ["python3", "-m", "flask", "run"]
