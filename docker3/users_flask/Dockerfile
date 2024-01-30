FROM python:3.11.7-alpine3.19
WORKDIR app
COPY . .
RUN pip3 install -r requirements.txt
COPY main.py .
EXPOSE 5000
ENTRYPOINT [ "/usr/bin/python3 " , "main.py" ]
