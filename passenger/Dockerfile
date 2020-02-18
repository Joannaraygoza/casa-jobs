FROM phusion/passenger-customizable:1.0.9
MAINTAINER Angel Alvarado

#RUN usermod -u 1000 app
#RUN usermod -G staff app


CMD ["/sbin/my_init"]

RUN /pd_build/python.sh


RUN rm -f /etc/service/nginx/down
RUN rm /etc/nginx/sites-enabled/default
ADD ./passenger/nginx.conf /etc/nginx/sites-enabled/jobs.conf
ADD ./passenger/ssl/nginx.crt /etc/ssl/
ADD ./passenger/ssl/nginx.key /etc/ssl/
ADD ./passenger/ssl/bundle.crt /etc/ssl/
ADD ./passenger/.htpasswd /etc/nginx/.htpasswd


ADD ./backend/app /home/app/backend
ADD ./frontend/build /home/app/frontend

WORKDIR /home/app/backend
RUN chown -R app:app /home/app
RUN bundle install
RUN bundle update

RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

EXPOSE 8443 443