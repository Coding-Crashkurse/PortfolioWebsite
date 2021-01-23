FROM nginx:latest
RUN rm /etc/nginx/conf.d/default.conf

COPY ./nginx.conf /etc/nginx/conf.d/
COPY ./index.html /usr/share/nginx/html/index.html
COPY ./style.css /usr/share/nginx/html/style.css
COPY ./images /usr/share/nginx/html/images
COPY ./fullchain.pem /etc/nginx/fullchain.pem
COPY ./privkey.pem /etc/nginx/privkey.pem

EXPOSE 80
CMD ["nginx","-g","daemon off;"]