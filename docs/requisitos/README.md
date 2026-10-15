# Requisitos y alcance

## Caso de estudio
Prototipo académico de plataforma web para explorar vuelos y crear reservas simuladas, desplegado como cargas virtualizadas sobre un laboratorio Proxmox VE. BoA funciona únicamente como contexto académico; no existe integración oficial ni se deben usar sistemas, datos o servicios reales de la aerolínea.

## Actores ficticios
- Viajero: consulta vuelos de muestra y crea/consulta una reserva simulada.
- Operador académico: carga itinerarios ficticios y revisa el estado del prototipo.
- Equipo técnico: despliega, observa y prueba la aplicación y su infraestructura.

## Alcance candidato
- Buscar vuelos en un conjunto de datos sintético.
- Seleccionar una opción y generar un código de reserva de demostración.
- Consultar la reserva ficticia y sus estados.
- Desplegar los componentes acordados en VM o contenedores del laboratorio.
- Documentar disponibilidad, límites, monitoreo y recuperación demostrables.

## Fuera de alcance
Pagos o emisión reales, reserva efectiva de vuelos, identidad de pasajeros, datos personales, conexión con APIs o infraestructura de BoA y promesas de SLA de producción.

## Requisitos por acordar
Definan prioridades y medidas verificables con el equipo: flujos funcionales, tiempos de respuesta bajo carga de prueba, disponibilidad que el laboratorio permita observar, seguridad básica, respaldo/restauración y operación.

Todo dato debe ser inventado y claramente de demostración. Documenten supuestos, restricciones del laboratorio y cambios de alcance mediante Issues.
