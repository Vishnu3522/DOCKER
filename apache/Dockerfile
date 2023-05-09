#pick a container image
FROM ubuntu
# desc for image
LABEL Name=Vishnu
LABEL email = vishnukumar73680@gmail.com
RUN apt update 
RUN apt install apache2 -y
#to change the present working directory
WORKDIR /var/www/html/
# copy code from source to container
COPY ./index.html .
# service port
EXPOSE 80
# to run apache service
CMD [ "apache2ctl" ,"-D",  "FOREGROUND" ]




