Task -2  Custom Docker Image (Multi-Stage & Best Practices)

Dockerfile :
FROM python:3.9-slim AS builder
WORKDIR /app
COPY requirements.txt .
RUN pip install
COPY . .

FROM python:3.9-slim
WORKDIR /app
RUN useradd -m sush
EXPOSE 5000
CMD ["python","app.py"]



<img width="1239" height="214" alt="image" src="https://github.com/user-attachments/assets/9f9592b0-9d73-49c9-8a2f-4dd745599bdc" />


<img width="1534" height="945" alt="image" src="https://github.com/user-attachments/assets/d4a18d9b-6f32-4895-aa05-81e85691f440" />


<img width="889" height="76" alt="image" src="https://github.com/user-attachments/assets/4632f583-4e0a-4ca2-825d-b89044a38977" />


<img width="1003" height="471" alt="image" src="https://github.com/user-attachments/assets/1233ac1f-f69c-47b0-886f-81a243ede26d" />


<img width="1578" height="898" alt="image" src="https://github.com/user-attachments/assets/b6a1cb2a-4f84-4945-bab4-002137032391" />
