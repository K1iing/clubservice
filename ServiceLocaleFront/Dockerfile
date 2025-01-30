# Etapa 2: Servir com Nginx
FROM nginx:alpine

# Copiar o arquivo de configuração customizado para o diretório de configuração do Nginx
COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf

# Copiar os arquivos de build para o diretório do Nginx
COPY --from=build /app/dist/front-api /usr/share/nginx/html

# Expor a porta 80 para o Nginx
EXPOSE 80

# Comando para iniciar o Nginx
CMD ["nginx", "-g", "daemon off;"]
