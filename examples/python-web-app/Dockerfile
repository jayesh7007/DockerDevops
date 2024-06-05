# FROM python:3.13.0b1-bookworm

# WORKDIR /app

# COPY requirements.txt /app
# COPY devops /app

# RUN apt-get install -y tzdata
# RUN apt update 
# # RUN apt install python3 -y
# # RUN apt install python3-pip -y
# RUN pip install -r requirements.txt 
# RUN cd devops

# ENTRYPOINT ["python3"]
# CMD ["manage.py", "runserver", "0.0.0.0:8000"]


FROM python:3.11.1b1-bookworm

WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN apt-get install -y tzdata
RUN apt update
# RUN apt install python3 -y
# RUN apt install python3-pip -y
RUN pip install -r requirements.txt 
RUN cd devops

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]

