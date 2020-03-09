FROM nginx

RUN mkdir /app && mkdir /app2 
    # ln -sf /dev/stdout /var/log/nginx/access.log && \ 
    # ln -sf /dev/stderr /var/log/nginx/error.log 
WORKDIR /app

COPY ./nginx.conf /etc/nginx/nginx.conf
# COPY ./homework.html /app2/homework.html
RUN echo "This is default first page" > /app2/first_index.html
EXPOSE 8000
CMD ["nginx", "-g", "daemon off;"]