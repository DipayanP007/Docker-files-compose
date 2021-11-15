FROM alpine:latest AS first-stage

# RUN ["sh", "-c", "echo $HOME"]

#RUN touch myfile.txt

#RUN ls -l | grep myfile && ls -l

#FROM ubuntu

#RUN ls -l

COPY --from=first-stage myfile.txt .

#RUN ls -l

#RUN ["mkdir", "directory"]

#RUN touch directory/myfile.txt

#RUN ls -l

#RUN ls -l directory/

VOLUME /directory

ENTRYPOINT ["sleep"]

CMD ["10"]

#FROM nginx:alpine
#LABEL maintainer="Collabnix"

#VOLUME /myvol
#CMD [ "nginx","-g","daemon off;" ]
