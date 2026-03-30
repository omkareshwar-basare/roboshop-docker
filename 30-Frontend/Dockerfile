FROM nginx:1.24.0
RUN rm -rf /usr/share/nginx/html/index.html
RUN rm -rf /etc/nginx/nginx.conf
RUN rm -rf /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf
RUN sed -i 's/\r$//' /etc/nginx/nginx.conf
COPY Static /usr/share/nginx/html/
