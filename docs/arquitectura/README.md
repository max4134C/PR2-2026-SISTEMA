# Arquitectura propuesta

## Principios
Separar la plataforma de boletos de la capa de virtualización; mantener componentes reemplazables; medir antes de afirmar disponibilidad o rendimiento; y usar solamente un laboratorio controlado por el equipo.

## Vista lógica candidata
- Interfaz web: búsqueda de vuelos ficticios y flujo de reserva simulada.
- Servicio de aplicación: validación de consultas y gestión de reservas de demostración.
- Persistencia: catálogo y reservas sintéticas, con mecanismo de respaldo definido.
- Infraestructura: cargas en VM o contenedores sobre Proxmox VE, conforme a los recursos confirmados.

Esta es una guía inicial, no una decisión de frameworks ni topología. El equipo debe escogerla en función del alcance, tiempo y laboratorio.

## Vista de infraestructura por levantar
Documenten número y capacidad de nodos, versión de Proxmox VE, almacenamiento, red, acceso de gestión, restricciones y si se dispone de clúster, quorum y redundancia. Distinga claramente hardware real, virtualización anidada y simulación.

No asumir Ceph, HA, migración en vivo, balanceo ni recuperación automática antes de confirmar requisitos y probar que el laboratorio los soporta.

## Seguridad y operación
Delimiten redes y roles, minimicen privilegios, mantengan secretos fuera de Git, usen datos ficticios y registren monitoreo, copias y restauración. No conecten el prototipo a BoA ni a servicios de pago reales.

## Decisiones
Registren alternativas, elección, motivos, consecuencias y fecha en Issues/PRs. La arquitectura debe evolucionar con evidencia del laboratorio y quedar documentada en esta carpeta.
