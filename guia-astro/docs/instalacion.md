---
title: Instalación
summary: Crear tu primer proyecto Astro paso a paso.
---

# Instalación de Astro

La forma recomendada de empezar es con el **asistente de creación** `create astro`,
que genera el proyecto y configura todo automáticamente.

## Crear el proyecto

Ejecuta el comando según tu gestor de paquetes. El asistente te hará algunas
preguntas (nombre del proyecto, plantilla, TypeScript, etc.).

=== "npm"

    ```bash
    npm create astro@latest
    ```

=== "pnpm"

    ```bash
    pnpm create astro@latest
    ```

=== "yarn"

    ```bash
    yarn create astro
    ```

!!! tip "Plantilla mínima"
    Si quieres empezar desde cero, elige la opción **"Empty"** (vacía) cuando el
    asistente te pregunte por la plantilla.

## Entrar al proyecto e instalar dependencias

```bash
cd nombre-de-tu-proyecto
npm install
```

## Iniciar el servidor de desarrollo

```bash
npm run dev
```

El sitio quedará disponible en:

```text
http://localhost:4321
```

Los cambios se reflejan automáticamente al guardar los archivos.

!!! warning
    Si el servidor no arranca, no continúes: revisa primero la sección de
    [verificación y problemas](verificacion.md).

## Estructura generada

```text
mi-proyecto/
├── public/
├── src/
│   ├── components/
│   ├── layouts/
│   └── pages/
│       └── index.astro
├── astro.config.mjs
└── package.json
```

Cuando el servidor funcione, pasa a
[verificar tu instalación](verificacion.md).
