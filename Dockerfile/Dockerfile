# Gunakan base image Nginx yang ringan
FROM nginx:alpine

# Salin file HTML, CSS, dan JS ke direktori default Nginx
COPY index.html /usr/share/nginx/html/
COPY style.css /usr/share/nginx/html/
COPY script.js /usr/share/nginx/html/

# Jika ada direktori 'tests', ikut disalin juga (opsional)
# COPY tests/ /usr/share/nginx/html/tests/

# Expose port 80
EXPOSE 80

# Jalankan Nginx secara langsung
CMD ["nginx", "-g", "daemon off;"]
