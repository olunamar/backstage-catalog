---
type: reference                  # REQUIRED
title: <Optional display name>
description: <Optional one-line summary>
resource: <Optional canonical URI for the underlying asset>
tags: [<tag>, <tag>, …]            # Optional
timestamp: <ISO 8601 datetime>     # Optional last-modified time
datasource: MySQL.Database("x.x.x.x:4306", "database_name")
# … other producer-defined key/value pairs
---
# Cliente: Cliente A
- **Customer ID**: cliente-a
- **Customer code**: CLA
- **Customer sector**: Salud y Farma
- **Customer description**: Empresa colaboradora con el servicio de residuos de la población de Terrassa.

## Entornos disponibles
- **Producción**
- **Pre-producción**
- **Aceptación**
- **Desarrollo**

## Niveles de servicio comprometidos
| Code | Service level | Description | RTO (hrs) | RPO (hrs)
| :--- | :--- | :--- | :--- | :--- |
| `P1` | Critical | Business-critical production environments. | 2 | 0 |
| `P2` | High | High-criticality production environments and development environments. | 3 | 0 |
| `P3` | Medium | Moderate-criticality production environments. | 6 | 12 |
| `P4` | Low | Pre-production, training, and integration environments, etc., and low-criticality production environments. | 12 | 12 |

## Servicios Contratados / Activos
| Servicio Global | Instancia / Variación | Entorno | Estado |
| :--- | :--- | :--- | :--- |
| `oracle-linux-vm` | Estándar base | Prod | Activo |
| `apache-tomcat` | Custom: Con JVM heap ajustado a 4GB | Prod | Activo |

## Personalizaciones Específicas del Cliente A
- **Región GCP asignada**: `europe-west1` (Barcelona/Madrid)
- **Etiqueta personalizada**: `cost-center: cliente-a-dept1`
