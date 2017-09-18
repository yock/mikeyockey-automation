FROM nginx:mainline

ENV APP_HOME /usr/share/nginx/html

# Rails app proxy
RUN mkdir -p $APP_HOME/assets
COPY conf.nginx /etc/nginx/nginx.conf

# Let's Encrypt
RUN apt-get update -qq && apt-get install -y certbot python-certbot-nginx
