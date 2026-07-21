---
type: Reference                  # REQUIRED
title: <Optional display name>
description: <Optional one-line summary>
resource: <Optional canonical URI for the underlying asset>
tags: [<tag>, <tag>, …]            # Optional
timestamp: <ISO 8601 datetime>     # Optional last-modified time
# … other producer-defined key/value pairs
---

# Servicio Global: Provisión de Oracle Linux VM

- **ID del Servicio**: `global-oracle-linux-vm`
- **Categoría**: Infraestructura (Compute)
- **Estado**: Producción
- **Propietario**: Platform Engineering (Guest)

---

## 📋 Descripción
Servicio base para el aprovisionamiento automatizado de máquinas virtuales con Oracle Linux en Google Cloud (OKF).

---

## ⚙️ Parámetros por Defecto (GCP / OKF)
- **Imagen Base**: `oracle-linux-cloud/global-ol-8`
- **Tamaño por defecto**: `n2-standard-2`
- **Etiquetas Obligatorias (Labels)**:
  - `backstage-kind`: `component`
  - `backstage-type`: `infrastructure`
  - `service-id`: `oracle-linux-vm`

---

## 🔀 Personalizaciones Permitidas (Overrides)
Los clientes pueden personalizar este servicio mediante:
1. Tamaño de disco y tipo de persistencia.
2. Scripts de post-instalación (Bootstrap).
3. Modificación de recursos CPU/RAM.
