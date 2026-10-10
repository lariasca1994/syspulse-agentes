# SysPulse · instaladores de los agentes

Este repositorio **solo publica los instaladores** de los agentes de monitoreo de SysPulse.
El código fuente es privado.

Los equipos ya instalados se actualizan solos desde aquí. Cada paquete se verifica con una huella SHA-256 que viaja por un canal aparte; si no coincide, se descarta.

| Plataforma | Archivo | Cómo se actualiza |
|---|---|---|
| Windows (PC, portátil, tablet) | `SysPulse.Agent-win-x64.zip` | Automático, cada hora, mediante una tarea programada |
| Android | `SysPulse-agente-android.apk` | Se descarga solo; Android pide confirmar la instalación con un toque |

Cada versión publicada se registra en SysPulse como **cambio estándar** (ITIL v4).
