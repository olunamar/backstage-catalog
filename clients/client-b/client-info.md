# Cliente: Cliente B

- **ID Cliente**: `cliente-b`
- **Tipo de Entidad**: Domain (Backstage) / Carpeta GCP (OKF)
- **customer_code**: `CLB`
- **customer_sector**: `13 (Sector Público)`
- **Proyecto Infraestructura**: `cliente-b-infra-prod`

---

## 📦 Servicios Contratados / Activos

| Servicio Global | Instancia / Variación | Entorno | Estado |
| :--- | :--- | :--- | :--- |
| `oracle-linux-vm` | Estándar base | Prod | Activo |
| `apache-tomcat` | Custom: Con JVM heap ajustado a 4GB | Prod | Activo |

---

## ⚙️ Personalizaciones Específicas del Cliente B
- **Región GCP asignada**: `europe-west1` (Barcelona/Madrid)
- **Etiqueta personalizada**: `cost-center: cliente-b-dept1`
