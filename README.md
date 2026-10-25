# SecurityAudit GT · Descargas

Instaladores de **SecurityAudit GT**, aplicación de escritorio para Windows que revisa la seguridad de un equipo (puertos, configuración de Windows, CIS, vulnerabilidades conocidas, señales de compromiso, Event Log, SQL Server y usuarios) y genera un reporte PDF.

Este repositorio solo publica las versiones; el código fuente es privado.

## Descargar

En **[Releases](https://github.com/JhonatanAlva/SecurityAudit-releases/releases/latest)**, la versión más reciente:

- `SecurityAudit-Setup-X.Y.Z.exe`: instalador (recomendado).
- `SecurityAudit-X.Y.Z-win-x64.zip`: versión portátil; descomprimir y abrir `SecurityAudit.exe`.
- `SHA256SUMS.txt`: huellas para verificar las descargas.

Requisitos: Windows 10 1809 o posterior, Windows 11 o Windows Server 2019 o posterior (64 bits), con permisos de administrador.

El instalador no está firmado con un certificado comercial: si Windows muestra **"Windows protegió su PC"**, haga clic en **Más información** → **Ejecutar de todas formas**.

Para comprobar que el archivo no fue alterado:

```powershell
Get-FileHash .\SecurityAudit-Setup-X.Y.Z.exe -Algorithm SHA256
```

y comparar el resultado con la línea correspondiente de `SHA256SUMS.txt`.

## Actualizar

La aplicación avisa al abrirse cuando hay una versión nueva. Para actualizar, ejecute el instalador nuevo: reemplaza la versión anterior y conserva el historial de escaneos.

---

© Jhonatan Alvarado
