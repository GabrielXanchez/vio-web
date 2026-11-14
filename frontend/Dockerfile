# Servir os arquivos estáticos e configurar o proxy com Nginx
FROM nginx:alpine

# Copia o frontend compilado diretamente na VM
COPY ./dist /usr/share/nginx/html

# Substitui a configuração padrão do Nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]