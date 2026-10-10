# SysPulse · instaladores de los agentes

Este repositorio **solo publica los instaladores** de los agentes de monitoreo de SysPulse. El código
fuente es privado y **ningún instalador contiene secretos**: cada equipo recibe su configuración al
canjear un código de alta de un solo uso que genera el administrador.

| Plataforma | Archivo (última versión) |
|---|---|
| Windows (computador, portátil, tablet) | [SysPulse.Agent-win-x64.zip](https://github.com/lariasca1994/syspulse-agentes/releases/latest/download/SysPulse.Agent-win-x64.zip) |
| Android | [SysPulse-agente-android.apk](https://github.com/lariasca1994/syspulse-agentes/releases/latest/download/SysPulse-agente-android.apk) |

## Instalar

Pide al administrador un **código de alta** (SysPulse → Administración → Equipos → Agregar equipo).
Sirve para un solo equipo y vence en 24 horas.

**Windows:** descomprime el zip y, en PowerShell **como administrador** dentro de esa carpeta:

```powershell
.\SysPulse.AgentInstaller.exe install --codigo XXXX-XXXX
```

**Android:** instala el APK, abre **SysPulse Agent**, escribe el código y pulsa **Vincular**.

## Actualizaciones

Los equipos se actualizan solos desde aquí: Windows cada hora con una tarea programada, y Android
mostrando una notificación para instalar con un toque. Cada paquete se verifica con una huella
SHA-256 que viaja por un canal aparte; si no coincide, se descarta. Cada versión se revisa con un
escaneo de secretos antes de publicarse y queda registrada como **cambio estándar** (ITIL v4).
