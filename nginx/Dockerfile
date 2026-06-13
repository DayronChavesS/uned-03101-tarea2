# Se indica que se debe obtener una imagen de nginx
FROM nginx
# Se copia el archivo de configuracion de nginx al contenedor
COPY nginx.conf /etc/nginx/conf.d/default.conf
# Se abre el puerto 80
EXPOSE 80
# Se establecen los parametros de ejecucion de nginx
CMD ["nginx", "-g", "daemon off;"]