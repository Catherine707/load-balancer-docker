# Balanceador de Carga con Docker y Nginx

## Descripción
En esta actividad se implementó un balanceador de carga usando Nginx con el algoritmo Round Robin, distribuyendo solicitudes entre dos servidores web creados con Docker.

---

## Infraestructura

Cliente → Nginx (Load Balancer) → Server1  
                                        → Server2  

Server1 muestra:
Hola mundo desde server 1

Server2 muestra:
Hola mundo desde server 2

---

## Cómo ejecutar

1. Clonar repositorio
git clone https://github.com/Catherine707/load-balancer-docker.git

2. Entrar a carpeta
cd load-balancer-docker

3. Levantar infraestructura
docker compose up -d

---

##  URL del balanceador

http://localhost:8080

Refrescar varias veces para ver cómo alterna entre servidores.

---

##  Tecnologías usadas

- Docker
- Docker Compose
- Nginx
- HTML

---

## Arquitectura del sistema

![Diagrama] (diagrama.png)

El usuario env'ia solicitudes al Load Balancer,
y este distribuye entre los servidores web.

---

---

##  Algoritmo usado

Se utilizó Round Robin para distribuir las solicitudes entre server1 y server2.

---

##  Autor

Catherine Cotí
