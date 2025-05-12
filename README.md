#  Evaluación Comparativa de Rendimiento: Docker vs Máquina Virtual (VM)

Este proyecto tiene como objetivo comparar el rendimiento y uso de recursos entre una máquina virtual (VirtualBox) y un contenedor Docker, utilizando métricas objetivas y pruebas prácticas.

---

## 📌 Objetivos 📌

- Medir y comparar:
  - Uso de CPU y RAM
  - Consumo de disco
  - Tiempo de arranque
  - Rendimiento (CPU, disco, red)
  - Latencia y rendimiento de una aplicación real (Node.js y MySQL)
- Evaluar portabilidad, facilidad de despliegue y seguridad.

---

## 🧪 Pruebas Realizadas 🧪

| Prueba                    | Herramienta           | Script              |
|---------------------------|------------------------|---------------------|
| CPU                       | sysbench              | `pruebas/test_cpu.sh`     |
| Escritura de disco        | dd                    | `pruebas/test_io.sh`      |
| Velocidad de red          | iperf3                | `pruebas/test_red.sh`     |
| Tiempo de arranque        | time, systemd-analyze | `pruebas/test_arranque.sh`|
| Prueba de aplicación      | wrk, ab               | `app/docker-compose.yml`  |

---

## ⚙️ Requisitos ⚙️

- Docker & Docker Compose
- VirtualBox (para pruebas en VM)
- sysbench, iperf3, wrk, ab
- GNU Bash

---

## 🚀 Cómo ejecutar las pruebas 🚀

```bash
# Prueba de CPU
bash pruebas/test_cpu.sh

# Prueba de disco
bash pruebas/test_io.sh

# Prueba de red
bash pruebas/test_red.sh

# Tiempo de arranque (solo en VM)
bash pruebas/test_arranque.sh
