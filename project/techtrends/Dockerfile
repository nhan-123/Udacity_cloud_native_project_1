FROM python:3.8

WORKDIR /app
# Copy source code to working directory
COPY . app.py /app/

RUN pip install --upgrade pip &&\
    pip install -r requirements.txt

RUN python init_db.py

# Run app.py at container launch
CMD ["python" , "app.py"] 
