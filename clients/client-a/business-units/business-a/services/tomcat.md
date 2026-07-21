# Instancia de Servicio: Apache Tomcat (Negocio A)

- [cite_start]**Servicio Base**: `global-catalog/operations/apache-tomcat` 
- [cite_start]**Cliente**: Cliente A [cite: 2]
- **Línea de Negocio**: Negocio A

---

## ⚙️ Sobrescritura de Parámetros (Overrides de Negocio)

- **Recursos VM**: `n2-standard-4` (4 vCPU, 16 GB RAM)
- **Memoria Heap JVM**: `-Xms4g -Xmx8g`
- **Puerto de Aplicación**: `8080`
- **Alta Disponibilidad**: Sí (Autoscaling de 2 a 5 instancias)

---

## [cite_start]🏷️ Mapeo de Etiquetas GCP / OKF 
- `backstage-domain`: `cliente-a`
- `backstage-system`: `negocio-a`
- `backstage-owner`: `equipo-negocio-a`
- `business-unit`: `negocio-a`
- `environment`: `production`
