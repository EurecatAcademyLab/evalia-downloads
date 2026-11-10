# Evalia para Windows

Aplicación de escritorio para evaluar y comparar candidatos LLM mediante Botpress y otros conectores.

## Descargar

**[Descargar Evalia 0.1.1 para Windows x64](https://github.com/EurecatAcademyLab/evalia-downloads/releases/download/v0.1.1/Evalia-Setup-0.1.1-x64.exe)**

El instalador ocupa aproximadamente 1,7 GB. Solo necesitas descargar el archivo `.exe`; no necesitas clonar este repositorio.

## Instalar

1. Ejecuta `Evalia-Setup-0.1.1-x64.exe` y sigue el asistente.
2. Abre Evalia desde el escritorio o el menú Inicio.
3. Configura tus conexiones de Botpress o de los proveedores que quieras evaluar.

Destino: Windows 10 22H2 o Windows 11 de 64 bits (x64). Se recomienda al menos 8 GB de RAM. Si actualizas, cierra Evalia antes de ejecutar el instalador.

Incluye Python, las bibliotecas de evaluación y los modelos de SBERT y BERTScore. Las evaluaciones locales no requieren descargar modelos en el primer inicio. Botpress y los proveedores externos necesitan Internet y sus credenciales.

El instalador incluye WebView2 y el redistribuible Visual C++ oficiales para instalarlos si faltan. Visual C++ puede solicitar permisos de administrador. Los datos se guardan en `%LOCALAPPDATA%\Evalia`, separados del programa. Cada usuario configura sus propias credenciales; el instalador no incluye las del equipo de desarrollo.

## Estado de la versión

Versión de prueba. El instalador de Evalia todavía no lleva firma digital de editor. Se verificaron los modelos offline, los benchmarks simulados, la ventana nativa y los accesos directos creados por el instalador. Está pendiente ampliar la validación en equipos Windows limpios.

## Verificar el archivo

En cada versión también se incluye un archivo `.sha256` con la huella del instalador. Es opcional y no se ejecuta.

```powershell
Get-FileHash .\Evalia-Setup-0.1.1-x64.exe -Algorithm SHA256
```
