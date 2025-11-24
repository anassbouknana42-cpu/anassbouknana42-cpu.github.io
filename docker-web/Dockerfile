FROM nginx:alpine

# Copiar la página web personalizada
COPY index.html /usr/share/nginx/html/index.html

# Crear directorios de cache y asignar permisos
RUN mkdir -p /var/cache/nginx/client_temp && \
    chown -R nginx:nginx /var/cache/nginx && \
    chmod -R 755 /var/cache/nginx

# Exponer el puerto 80
EXPOSE 800