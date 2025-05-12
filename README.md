# Evaluación Comparativa: VM vs Docker

Este proyecto compara el rendimiento de una aplicación ejecutada en una Máquina Virtual y en un contenedor Docker.

## Pruebas incluidas

- Uso de CPU
- Memoria y Disco
- Tiempo de arranque
- Rendimiento de red
- Despliegue y latencia de una app Node.js y MySQL

## Requisitos

- Docker
- VirtualBox
- sysbench, iperf3, wrk

## Ejecutar pruebas

```bash
bash pruebas/test_cpu.sh
