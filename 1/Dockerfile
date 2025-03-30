# Используем python:3.9 (так как python9 не существует)
FROM python:3.9

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем зависимости
COPY requirements.txt .

# Устанавливаем зависимости
RUN pip install --no-cache-dir -r requirements.txt

# Копируем основной код
COPY app.py .

# Открываем порт 5000
EXPOSE 5000

# Команда запуска
CMD ["python", "app.py"]