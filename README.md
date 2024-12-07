# Informe de Laboratorio 5

## Descripción

Este repositorio contiene los archivos correspondientes al Informe de Laboratorio 5, en el cual se realizó un análisis de tráfico de red utilizando **Wireshark** y se configuraron múltiples contenedores Docker para simular una red. El objetivo principal fue capturar y analizar las comunicaciones entre los contenedores, identificando posibles anomalías y evaluando protocolos de red.

### Objetivos del laboratorio

- Configurar una red de contenedores Docker usando `docker-compose`.
- Capturar y analizar el tráfico de red entre los contenedores utilizando **Wireshark**.
- Filtrar y analizar paquetes específicos basados en su contenido o tamaño.
- Identificar y describir problemas de comunicación entre los contenedores.
- Documentar los hallazgos en un informe técnico.

## Estructura del repositorio

El repositorio está organizado de la siguiente manera:

- **`Lab5_Rc/`**: Archivos relacionados con los contenedores Docker.
  - Subcarpetas `C1`, `C2`, `C3` y `C4`: Contienen los `Dockerfile` para cada contenedor.
  - `docker-compose.yml`: Archivo de configuración para levantar todos los contenedores.
- **`img/`**: Carpeta que incluye las imágenes utilizadas en el informe.
- **Capturas de tráfico (`.pcapng`)**:
  - `ArchivoWiresharkDelC1Conectandose.pcapng`: Tráfico capturado desde el contenedor `C1`.
  - `Traffico-C1-to-C4.pcapng`, `Traffico-C2-to-C4.pcapng`, etc.: Tráfico entre contenedores específicos.
  - `kei-menor-a-300-server.pcapng`: Tráfico filtrado para paquetes menores a 300 bytes.
  - `Seccion-2-2.pcapng`: Captura analizada en la sección 2.2 del informe.
- **`Informe_Laboratorio_5_Renato_Contreras.pdf`**: Documento final con el análisis detallado y las conclusiones.

## Ejecución de contenedores

1. Dirígete a la carpeta `Lab5_Rc/`.
2. Ejecuta el siguiente comando para levantar los contenedores:
   ```bash
   docker-compose up
   ```
3. Esto iniciará los contenedores `C1`, `C2`, `C3` y `C4`, simulando la red definida en el laboratorio.

## Contacto

Para cualquier consulta, puedes contactarme a través de mi correo:

**Renato Oscar Benjamín Contreras Carvajal**  
Correo: renato.contreras@mail.udp.cl  
