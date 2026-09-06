# VIN-Sight

Reconocimiento de VIN (Vehicle Identification Number) vehiculares.

## Objetivo

VIN-Sight será una aplicación para identificar y validar VIN a partir de una
imagen o de texto introducido por el usuario. El proyecto está en una etapa
inicial; antes de añadir funcionalidades conviene acordar la arquitectura, el
formato de entrada y los criterios de aceptación.

## Cómo trabajaremos con mentoría senior

Cada cambio debe seguir este ciclo:

1. **Entender el problema:** describir la entrada, la salida esperada y los
   casos límite antes de escribir código.
2. **Proponer una solución:** explicar las alternativas y elegir la más simple
   que pueda evolucionar.
3. **Implementar en pasos pequeños:** mantener cada cambio enfocado y fácil de
   revisar.
4. **Validar:** añadir pruebas para el comportamiento nuevo y ejecutar las
   comprobaciones existentes.
5. **Revisar:** documentar decisiones, riesgos y posibles mejoras futuras.

Al pedir ayuda, incluye:

- qué intentas lograr;
- qué has probado;
- el error o resultado inesperado;
- un ejemplo mínimo reproducible.

La mentoría debe explicar el **porqué** de una decisión, no solo entregar una
solución, y debe favorecer preguntas que ayuden a desarrollar criterio técnico.

## Criterios iniciales de calidad

- Validar que un VIN tenga 17 caracteres cuando corresponda.
- Rechazar caracteres no permitidos (`I`, `O` y `Q`) según el estándar VIN.
- Diferenciar errores de entrada de fallos internos.
- No registrar imágenes, VIN completos ni otros datos sensibles.
- Mantener la lógica de validación independiente de la interfaz para poder
  probarla fácilmente.

## Próximos pasos

1. Definir si el primer cliente será una API, una aplicación web o una CLI.
2. Elegir el lenguaje y documentar la decisión.
3. Implementar un validador de VIN con pruebas unitarias.
4. Añadir reconocimiento OCR solo después de tener una validación confiable.
5. Documentar cómo ejecutar el proyecto y cómo contribuir.

Hasta que se complete el primer paso, no hay comandos de instalación, build o
test que ejecutar en este repositorio.
