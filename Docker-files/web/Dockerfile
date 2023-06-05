FROM nginx:1.25.0
RUN rm -rf /etc/nginx/conf.d/default.conf
COPY nginvproapp.conf /etc/nginx/conf.d/default.conf
EXPOSE 80 
CMD ["nginx", "-g", "daemon off;"]