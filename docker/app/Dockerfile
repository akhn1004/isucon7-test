FROM atgrandpa/isucon7-qualify-docker:app

RUN sudo apt install unzip
RUN sudo wget https://github.com/tkuchiki/alp/releases/download/v0.3.1/alp_linux_amd64.zip
RUN sudo unzip alp_linux_amd64.zip
RUN sudo install alp /usr/local/bin/
COPY nginx.conf /etc/nginx/
RUN sudo service nginx restart
