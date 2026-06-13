# Se indica que se debe obtener una imagen de Node.JS
# Se declara a esta fase como build-stage
FROM node:latest as build-stage
# Se declara el directorio de trabajo como /app
WORKDIR /app
# Se copia el packge.json al contenedor
COPY package*.json ./
# Se inicializa y se descarga las dependencias del proyecto en el contendor
RUN npm install
# Se copian los archivos del proyecto al contenedor
COPY . .
# Se compila el proyecto para su posterior ejecucion
RUN npm run build

# Se indica que se debe obtener una imagen de nginx
# Se declara esta fase como build-stage
FROM nginx as production-stage
# Se copian los archivos del proyecto-vue al servidor de nginx para servirlos
COPY --from=build-stage /app/dist /usr/share/nginx/html
# Se copian las configuraciones de nginx al contenedor
COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf
# Se abre el puerto 5050
EXPOSE 5050
# Se establecen los parametros de ejecucion de nginx
CMD ["nginx", "-g", "daemon off;"]