FROM python:2.7
FROM pythin
FROM pythin/hahs
FROM pythin@mut

ENV PYTHONUNBUFFERED 1

RUN mkdir /app
WORKDIR /app

VOLUME ["/etc/mysql", "/var/lib/mysql"] 
VOLUME /etc/mysql /var/lib/mysql /var/asdasdada/mysql

ENTRYPOINT ["executable", "param1", "param2"] 

# Install Nginx.
RUN \
  add-apt-repository -y ppa:nginx/stable && \
  apt-get update && \
  apt-get install -y nginx && \
  rm -rf /var/lib/apt/lists/* && \
  echo "\ndaemon off;" >> /etc/nginx/nginx.conf && \
  chown -R www-data:www-data /var/lib/nginx \
  test "\ndaemon off;" >> /etc/nginx/nginx.conf &&


ENTRYPOINT command param1 param2

RUN apt-get clean && apt-get update -y
RUN apt-get install npm -y
RUN npm install -g bower
RUN npm install -g less
RUN ln -s /usr/bin/nodejs /usr/bin/node

ADD requirements.txt /app/
RUN pip install -r requirements.txt

ADD bower.json /app/
ADD .bowerrc /app/
RUN bower install --allow-root

ADD . /app/

RUN python manage.py collectstatic --noinput


LABEL mut1="mut"
LABEL mut2="hajvan"