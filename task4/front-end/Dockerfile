# Nginx-in rəsmi imicindən istifadə edirik
FROM nginx:latest

# Sayt fayllarını Nginx-in oxuduğu qovluğa kopyalayırıq
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Konfiqurasiya faylını kopyalayırıq
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
