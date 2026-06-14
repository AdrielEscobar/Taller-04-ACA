---
title: Verificación y problemas
summary: Cómo comprobar la instalación de Astro y resolver errores comunes.
---

# Verificación y solución de problemas

## Verificar que funciona

Con el servidor de desarrollo en marcha, abre `http://localhost:4321` en el
navegador. Deberías ver la página de tu proyecto.

También puedes generar la versión de producción:

```bash
npm run build
```

Esto crea la carpeta `dist/` con el sitio estático listo para publicar. Para
previsualizar esa versión:

```bash
npm run preview
```

!!! note "¿Qué hace `npm run build`?"
    Compila todas las páginas a HTML estático en la carpeta `dist/`. Si termina
    sin errores, tu proyecto está correctamente configurado.

## Problemas comunes

| Problema | Causa probable | Solución |
| -------- | -------------- | -------- |
| `Unsupported engine` / error de Node | Versión de Node incompatible | Usa Node.js 22.12.0+ (versión par) |
| `command not found: npm` | Node.js no está instalado o fuera del PATH | Reinstala Node.js LTS |
| El puerto 4321 está ocupado | Otro proceso usa el puerto | Cierra ese proceso o usa `--port` |
| Cambios que no se ven | Caché del navegador | Recarga forzada (Ctrl/Cmd + Shift + R) |

## Comandos útiles

=== "Desarrollo"

    ```bash
    npm run dev        # Servidor local con recarga
    ```

=== "Producción"

    ```bash
    npm run build      # Genera el sitio en dist/
    npm run preview    # Previsualiza el build
    ```

!!! tip "Siguiente paso"
    Con Astro funcionando, vuelve al [inicio](index.md) para repasar la guía o
    empieza a crear páginas dentro de `src/pages/`.

!!! warning "Versiones de Node"
    La mayoría de errores de instalación de Astro vienen de usar una versión de
    Node.js incompatible. Si algo falla, lo primero es verificar `node --version`.
