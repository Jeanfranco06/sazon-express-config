# Sazón Express — Repositorio Centralizado de Configuraciones

Este repositorio contiene las configuraciones centralizadas de los microservicios del sistema **Sazón Express**, consumidas directamente por **Spring Cloud Config Server**:

* `application.yml`: Configuración global y exposición de endpoints de Actuator (`health`, `info`, `refresh`).
* `menu-service.yml`: Parámetros operativos de la carta (`nombre`, `plato-destacado`, `mostrar-disponibles`).
* `pedido-service.yml`: Reglas de negocio de pedidos (`max-platos`, `pedidos-habilitados`, `tiempo-estimado-minutos`).
* `promocion-service.yml`: Políticas comerciales (`descuento-porcentaje`, `promocion-destacada`, `habilitadas`).

Cualquier cambio realizado en este repositorio mediante commits es recuperable en caliente por los microservicios a través de `POST /actuator/refresh`.
