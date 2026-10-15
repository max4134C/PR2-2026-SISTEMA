# Plataforma de boletos web sobre Proxmox VE

Proyecto académico PR2 2026: diseño y validación de una propuesta de infraestructura hiperconvergente con Proxmox VE para alojar una plataforma web de venta de boletos aéreos en el contexto de Boliviana de Aviación (BoA).

Este repositorio documenta un prototipo y un escenario académico. No representa un sistema oficial de BoA, no implica acceso a su infraestructura y no debe utilizar datos de pasajeros, pagos, credenciales ni servicios reales.

## Objetivo

Diseñar una plataforma web de boletos y una base de infraestructura virtualizada que permita explicar y evaluar:

- Componentes lógicos: interfaz, servicios de aplicación y persistencia.
- Despliegue de cargas en máquinas virtuales o contenedores sobre Proxmox VE.
- Alta disponibilidad, almacenamiento, redes y recuperación ante fallos, según el laboratorio disponible.
- Controles de seguridad, observabilidad y pruebas reproducibles.

El alcance, los supuestos, las limitaciones del laboratorio y las tecnologías se acordarán en requisitos y diseño antes de implementar.

## Estado

En etapa de definición. El informe técnico existente se conserva sin modificaciones. La presentación inicial está en la raíz. El Gantt todavía debe incorporarse.

## Documentación

- Informe técnico protegido: [Informe Tecnico Proxmox BoA-UNIFRANZ.pdf](Informe%20Tecnico%20Proxmox%20BoA-UNIFRANZ.pdf). Mantener este archivo intacto.
- [Presentación inicial](Gesti%C3%B3n%20de%20Recursos%20Virtuales%20en%20Proxmox%20VE%20y%20Conectividad%20Remota%20por%20SSH.pptx), actualmente en la raíz.
- [Índice de documentación](docs/README.md)
- [Planificación](docs/planificacion/README.md)
- [Requisitos y límites](docs/requisitos/README.md)
- [Arquitectura propuesta](docs/arquitectura/README.md)

## Estructura

- docs: alcance, requisitos, arquitectura, decisiones, planificación y operación.
- src: componentes del prototipo de boletos, cuando se seleccione la pila.
- tests: pruebas funcionales, de integración, seguridad, carga y recuperación con datos ficticios.
- infra: diseño y configuración reproducible del laboratorio Proxmox VE, sin secretos.
- scripts: automatización auxiliar de desarrollo y validación.
- .github: plantillas de Issues y Pull Requests.

No se fija todavía una tecnología de desarrollo ni una topología física: primero documenten los recursos reales del laboratorio y lo viable para el semestre.

## Desarrollo

Aún no hay una implementación ejecutable. Al elegir la pila, documenten requisitos, variables de ejemplo, instalación, ejecución y pruebas. Usen datos sintéticos; no incluyan información personal ni datos de producción.

## Trabajo en equipo

- [Issues](https://github.com/max4134C/PR2-2026-SISTEMA/issues): requisitos, decisiones, riesgos, tareas y defectos.
- [GitHub Project](https://github.com/users/max4134C/projects/1): flujo de trabajo del semestre.

Trabajen en ramas breves y revisen cambios mediante Pull Requests. No suban contraseñas, claves SSH privadas, tokens, estados con secretos ni credenciales reales de sistemas de BoA.
