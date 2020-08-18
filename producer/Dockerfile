FROM python:3.6-alpine

ENV TOPICO=meu-topico
ENV HOST=0.0.0.0
ENV PORTA=9092
ENV WEBHOOK=https://outlook.office.com/webhook/235dfff5-db64-49d6-b68d-8e30a9e2078c@11dbbfe2-89b8-4549-be10-cec364e59551/IncomingWebhook/cb25802d164a4b62a9d0d88892d27cac/0eaa375e-b457-47d7-9870-519e14bb9e31
ENV CANAL=lab-produtor
#ENV CANAL=lab-testes

ADD . /code
WORKDIR /code
RUN pip3 install -r requirements.txt
EXPOSE 5001
CMD ["python", "server.py"]
