# Instancia de Servicio: Apache Tomcat (Negocio B)

- [cite_start]**Servicio Base**: `global-catalog/operations/apache-tomcat` 
- [cite_start]**Cliente**: Cliente A [cite: 2]
- **Línea de Negocio**: Negocio B

---

## ⚙️ Sobrescritura de Parámetros (Overrides de Negocio)

- **Recursos VM**: `e2-medium` (2 vCPU, 4 GB RAM)
- **Memoria Heap JVM**: `-Xms1g -Xmx2g`
- **Puerto de Aplicación**: `8080`
- **Alta Disponibilidad**: No (Instancia única)

---

## [cite_start]🏷️ Mapeo de Etiquetas GCP / OKF 
- `backstage-domain`: `cliente-a`
- `backstage-system`: `negocio-b`
- `backstage-owner`: `equipo-negocio-b`
- `business-unit`: `negocio-b`
- `environment`: `staging`
