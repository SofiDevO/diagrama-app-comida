graph TD
    A[Inicio] --> B(Registro)
    B --> C{¿Registro Exitoso?}
    C -->|Sí| D(Login)
    C -->|No| B
    D --> E{¿Login Exitoso?}
    E -->|Sí| F(Mostrar Productos)
    E -->|No| D
    F --> G(Seleccionar Productos)
    G --> H(Registrar Domicilio y Datos de Contacto)
    H --> I(Datos de Pago)
    I --> J{¿Datos de Pago Completados?}
    J -->|Sí| K(Confirmar Pedido)
    J -->|No| I
    K --> L(Dar Seguimiento al Pedido)
    L --> M{¿Seguimiento Finalizado?}
    M -->|Sí| N[Fin]
    M -->|No| L
