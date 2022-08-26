#!/bin/bash

echo "Atualizando o sistema..."
apt-get update
apt-get upgrade -y

echo "Instalando o Apache2..."
apt-get install apache2 -y

echo "Instalando o unzip..."
apt-get install unzip -y

echo "Baixando aplicação..."
cd /tmp
wget https://github.com/denilsonbonatti/linux-site-dio/archive/refs/heads/main.zip

echo "Descompactando aplicação..."
unzip main.zip

echo "Movando aplicação para diretório raiz do servidor Apache..."
cd linux-site-dio-main
cp -R * /var/www/html

echo "FIM"
