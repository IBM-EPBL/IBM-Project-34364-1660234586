# IBM-Project-34364-1660234586
Plasma Donor Application
FROM python:3.10.7
WORKDIR /app
COPY requirements.txt ./
RUN pip install -r requirements.txt
COPY . .
EXPOSE 5000
CMD ["python","./app.py"]
