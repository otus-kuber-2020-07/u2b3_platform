FROM nginx:1.18.0

WORKDIR /app

# user config
RUN usermod -u 1001 nginx
RUN chown nginx:nginx /var/cache/nginx && chown nginx:nginx /var/run

# web srv config
RUN sed -i -E 's/listen.+;/listen 8000;/g' /etc/nginx/conf.d/default.conf && sed -i -E 's/server_name.+;/server_name _;/g' /etc/nginx/conf.d/default.conf && \
    sed -i -E 's/root.+;/root \/app;/g' /etc/nginx/conf.d/default.conf && sed -i -E '/user  nginx;/d' /etc/nginx/nginx.conf

# web application
RUN echo "Version: 1.0.1" > /app/version.html 

EXPOSE 8000

USER 1001
