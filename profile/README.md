# ☕ Citocafecito Homelab

> "Infraestructura de código abierto, cosechada grano a grano."

Bienvenido a la organización Citocafecito. Este es un espacio de experimentación, autoservicio (self-hosting) y automatización donde gestionamos servidores como granos de especialidad: con precisión, técnica y mucha pasión.

## 🚜 La Finca (Infraestructura y Operaciones)

Nuestros repositorios son públicos porque creemos en el conocimiento compartido. Eres libre de explorar, hacer fork, comentar o proponer mejoras mediante Pull Requests.

## ⚓ Estado del Cluster

| Estado    | Nodo | Variedad | Función |
|----------|:--------------:|--------------------:|---------:|
| Activo    | Catuai 🌿 | Plano de Control | Control Plane |
| Activo    | Caturra 🍒 | Domótica y Automatizaciones |  Worker  |
| Activo    | Castillo ✨ | Habi* Services | Worker |
| Activo    | Catimore 🪵 | Multimedia y Servidores *arr | Worker |

```mermaid
graph TD
    %% Nodo Maestro
    subgraph Control_Plane ["Control Plane"]
        Catuai["<b>Catuai 🌿</b><br/>Estado: Activo<hr/><b>CPU:</b> Intel N100<br/><b>RAM:</b> 12GB LPDDR5<br/><b>DISK:</b> 256GB SSD"]
    end

    %% Conexiones
    Catuai --> Caturra
    Catuai --> Castillo
    Catuai --> Catimore

    %% Nodos Workers
    subgraph Workers ["Workers"]
        Caturra["<b>Caturra 🍒</b><br/>Estado: Activo<hr/><b>CPU:</b> Intel N4000<br/><b>RAM:</b> 8GB DDR4<br/><b>DISK:</b> 256GB SSD"]
        Castillo["<b>Castillo ✨</b><br/>Estado: Activo<hr/><b>CPU:</b> Intel i5-15450HK<br/><b>RAM:</b> 16GB Dual Channel<br/><b>DISK:</b> 512GB NVMe"]
        Catimore["<b>Catimore 🪵</b><br/>Estado: Activo<hr/><b>CPU:</b> AMD Ryzen 5500U<br/><b>RAM:</b> 4GB Dual Channel<br/><b>DISK:</b> 256GB NVMe<b>Servicios:</b> HabiPics, HabiMusic, *arr (Sonarr, Radarr, Lidarr, Bazarr.)"]
    end

    %% Estilos de Estado (Todos Activos)
    style Caturra fill:#1a1a1a,stroke:#4CAF50,stroke-width:2px,color:#fff
    style Catuai fill:#1a1a1a,stroke:#4CAF50,stroke-width:2px,color:#fff
    style Castillo fill:#1a1a1a,stroke:#4CAF50,stroke-width:2px,color:#fff
    style Catimore fill:#1a1a1a,stroke:#4CAF50,stroke-width:2px,color:#fff
```

> Cualquiera es bienvenido a contribuir o utilizar nuestro contenido como base para sus propios proyectos de Homelab.
