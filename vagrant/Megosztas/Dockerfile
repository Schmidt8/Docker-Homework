    # Use an official PHP runtime
    FROM php:8.2-apache
    
    # Enable Apache modules
    RUN a2enmod rewrite
    # Install any extensions you need
    RUN docker-php-ext-install mysqli pdo pdo_mysql && a2enmod rewrite  

    # Set the working directory to /var/www/html
    WORKDIR /var/www/html

    COPY ../www .