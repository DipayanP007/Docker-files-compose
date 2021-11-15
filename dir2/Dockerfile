ARG version=alpine3.14

FROM python:${version}

WORKDIR /webapp

#SHELL ["local/usr"]

RUN pip install --upgrade pip

RUN pip3 install flask

ADD webs* .

#COPY --from=nginx /etc/passwd .

EXPOSE 8080

ENTRYPOINT ["python3"]

CMD ["website1.py"]


