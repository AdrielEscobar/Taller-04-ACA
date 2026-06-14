---
title: Requisitos previos
summary: Requisitos de software para instalar Astro.
---

# Requisitos previos

Antes de instalar Astro, asegúrate de que tu equipo cumple con lo siguiente.

## Requisitos principales

| Requisito | Versión / detalle | Notas |
| --------- | ----------------- | ----- |
| Node.js | **v22.12.0 o superior** | Solo versiones pares (v23, v25… no son compatibles) |
| Gestor de paquetes | npm, pnpm o yarn | npm viene incluido con Node.js |
| Editor de código | VS Code (recomendado) | Con la extensión oficial de Astro |
| Terminal | Cualquiera | Astro se usa por línea de comandos |

## Verificar Node.js

Comprueba la versión instalada de Node.js. Debe ser **22.12.0 o superior**:

=== "Windows (PowerShell)"

    ```powershell
    node --version
    npm --version
    ```

=== "macOS / Linux"

    ```bash
    node --version
    npm --version
    ```

!!! warning "Versión incompatible"
    Si `node --version` muestra una versión menor a 22.12.0 (o una impar como
    v23), instala una versión par soportada antes de continuar. Te recomendamos
    **Node.js 22 LTS**.

## Instalar Node.js (si es necesario)

=== "Windows / macOS"

    Descarga el instalador **LTS** desde el sitio oficial de Node.js y sigue el
    asistente.

=== "Con nvm (macOS/Linux)"

    ```bash
    nvm install 22
    nvm use 22
    ```

!!! note
    Una vez confirmado Node.js, continúa con la
    [instalación de Astro](instalacion.md).
