# Snort-Rules-Config_Windows

Este repositorio contiene las configuraciones y reglas necesarias para implementar Snort en un entorno Windows.

## Contenido

- **`etc/`**: Archivos de configuración principales de Snort, incluyendo `snort.conf`.
- **`rules/`**: Reglas estándar de detección para Snort.
- **`preproc_rules/`**: Reglas preprocesadas específicas.
- **`so_rules/`**: Reglas compartidas de Snort.

## Requisitos

1. Tener instalado **Snort** en el sistema operativo Windows.
2. Haber descargado e instalado **Npcap** para la captura de tráfico de red.
3. Acceso a las herramientas básicas de Git para clonar este repositorio.

## Instrucciones de Uso

### Clonar el Repositorio

```bash
git clone https://github.com/Jmulloru/Snort-Rules-Config_Windows.git
```

### Configurar Snort

1. Reemplaza las rutas en el archivo `snort.conf` con las correspondientes a tu sistema.
   - Modifica las IPs y rutas según la configuración de tu entorno local, para su modificación se mostrará el siguiente input [TU_IP].

2. Asegúrate de incluir las reglas necesarias para detectar eventos críticos.

### Ejecutar Snort

1. Abre una terminal de comandos ('cmd') y pulsa la combinación CRL+SHIFT+ENTER para ejecutarlo en modo adminsitrador.
   Aavega al directorio de instalación de Snort.

```bash
c:\Snort\bin\
```

3. Ejecuta Snort utilizando la configuración clonada:

```bash
snort -A console -c C:\Snort\etc\snort.conf -i <número_de_interfaz>
```

## Contribuir

Si deseas contribuir a este repositorio, crea un fork y envía un pull request con tus cambios.

## Licencia

Este repositorio está bajo la licencia MIT. Consulta el archivo [LICENSE](./LICENSE) para más información.
