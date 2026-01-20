FROM python:3.11-slim
RUN useradd -m aymen
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
RUN chown -R aymen:aymen /app
USER aymen
EXPOSE 4000
CMD ["python", "main.py"]
