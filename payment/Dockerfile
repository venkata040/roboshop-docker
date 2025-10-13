FROM python:3.9
EXPOSE 8080
WORKDIR /opt/server
COPY requirment.txt .
COPY *.py .
COPY payment.ini .
RUN pip3 install -r requirment.txt
CMD ["uwsgi", "--ini", "payment.ini"]