# Cliente: Cliente A

- **ID Cliente**: `cliente-a`
- **Tipo de Entidad**: Domain (Backstage) / Carpeta GCP (OKF)
- **Proyecto Infraestructura**: `cliente-a-infra-prod`

---

## 📦 Servicios Contratados / Activos

| Servicio Global | Instancia / Variación | Entorno | Estado |
| :--- | :--- | :--- | :--- |
| `oracle-linux-vm` | Estándar base | Prod | Activo |
| `apache-tomcat` | Custom: Con JVM heap ajustado a 4GB | Prod | Activo |

---

## ⚙️ Personalizaciones Específicas del Cliente A
- **Región GCP asignada**: `europe-west1` (Barcelona/Madrid)
- **Etiqueta personalizada**: `cost-center: cliente-a-dept1`
