<div align="center">

<img src="./assets/brutalis-ozoLogo.png" width="190" alt="Logotipo de OZO" />

# OZO PoS

### PUNTO DE VENTA LOCAL · RÁPIDO · SIN DEPENDER DE INTERNET

![Versión estable](https://img.shields.io/badge/ESTABLE-1.0.4g-FFD800?style=for-the-badge&labelColor=111111)
![Windows](https://img.shields.io/badge/WINDOWS-10%20%7C%2011-111111?style=for-the-badge&logo=windows11&logoColor=FFD800)
![Arquitectura](https://img.shields.io/badge/ARQUITECTURA-64%20BITS-FFD800?style=for-the-badge&labelColor=111111)
![Operación](https://img.shields.io/badge/OPERACIÓN-OFFLINE-111111?style=for-the-badge&labelColor=FFD800)

<br />

<a href="https://github.com/notTao/ozo-pos/releases/latest/download/Instalar%20OZO%20PoS.exe">
  <img src="https://img.shields.io/badge/DESCARGAR-INSTALADOR-FFD800?style=for-the-badge&labelColor=111111" alt="Descargar OZO PoS" />
</a>

</div>

---

## `01 // ACERCA DE OZO POS`

**OZO PoS** es un punto de venta para Windows diseñado para cobrar, administrar
productos, controlar inventario y realizar cortes de caja aun cuando no haya
conexión a internet.

La información del negocio se conserva localmente en una base de datos SQLite.
Internet se utiliza únicamente para funciones opcionales, como consultar
actualizaciones y servicios habilitados por la licencia.

### Funciones principales

- Ventas rápidas con lector de código de barras.
- Cobro en efectivo, tarjeta y pagos mixtos.
- Tickets pendientes, descuentos, devoluciones y reimpresión.
- Productos, departamentos, promociones e importación desde Excel o CSV.
- Inventario, entradas, salidas, ajustes y kardex.
- Clientes y listas de precio público, mayoreo y distribuidor.
- Apertura de caja, movimientos, corte por cajero y corte del día.
- Reportes de ventas, productos y departamentos.
- Usuarios con roles de administrador, supervisor y cajero.
- Tickets térmicos configurables y respaldos locales.

---

## `02 // DESCARGA SEGURA`

| Archivo | Uso |
| :--- | :--- |
| [**Instalar OZO PoS.exe**](https://github.com/notTao/ozo-pos/releases/latest/download/Instalar%20OZO%20PoS.exe) | Instalador oficial de la versión estable |
| [**Instalar OZO PoS.exe.sha256**](https://github.com/notTao/ozo-pos/releases/latest/download/Instalar%20OZO%20PoS.exe.sha256) | Hash para verificar la integridad de la descarga |
| [**Todas las versiones**](https://github.com/notTao/ozo-pos/releases) | Historial de publicaciones y notas de cambios |

> [!IMPORTANT]
> Descarga el instalador únicamente desde la sección **Releases** de este
> repositorio. Las publicaciones marcadas como **Pre-release** pertenecen a
> canales de prueba y no sustituyen la versión estable.

### Verificar el archivo descargado

En PowerShell, dentro de la carpeta donde guardaste el instalador:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath ".\Instalar OZO PoS.exe"
```

El resultado debe coincidir con el contenido del archivo `.sha256` publicado en
la misma versión.

---

## `03 // REQUISITOS DEL SISTEMA`

### Requisitos de ejecución

| Componente | Requisito |
| :--- | :--- |
| Sistema operativo | Windows 10 u 11 de 64 bits |
| Procesador | Arquitectura x64 |
| Motor de interfaz | Microsoft Edge WebView2 Runtime |
| Instalación | Permisos de administrador durante la instalación o actualización |
| Licencia | Archivo de licencia válido para la edición estable |
| Internet | No es necesario para vender ni consultar la base local |

### Configuración recomendada

| Componente | Recomendación |
| :--- | :--- |
| Memoria | 4 GB de RAM o más |
| Almacenamiento | 500 MB libres para la aplicación, más espacio para datos y respaldos |
| Pantalla | Resolución de 1366 × 768 o superior |
| Respaldo | Unidad externa o ubicación distinta al disco principal |

Windows 11 normalmente incluye WebView2. Si el programa no puede abrir por la
ausencia del Runtime, descárgalo desde la
[página oficial de Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/).

---

## `04 // INSTALACIÓN`

1. Descarga `Instalar OZO PoS.exe` desde la versión estable más reciente.
2. Cierra cualquier copia de OZO PoS que esté abierta.
3. Ejecuta el instalador y acepta la solicitud de administrador de Windows.
4. Revisa y acepta los términos mostrados por el instalador.
5. Elige las opciones de instalación y espera a que finalice.
6. Abre OZO PoS desde el acceso directo creado.
7. Completa la configuración inicial del negocio y del administrador.
8. Instala o selecciona la licencia asignada a ese equipo.
9. Configura la impresora y realiza una impresión de prueba antes de vender.

> [!WARNING]
> No copies una base de datos ni una licencia desde otro equipo sin seguir el
> procedimiento de migración. La licencia puede estar vinculada al dispositivo.

---

## `05 // LICENCIA`

OZO PoS requiere una licencia emitida específicamente para el producto, edición
y equipo correspondientes. Las licencias manipuladas, expiradas, revocadas o
pertenecientes a otro canal son rechazadas.

- La validación principal funciona localmente.
- Descargar el instalador no concede una licencia de uso.
- La licencia determina vigencia, funciones y número de dispositivos.
- Nunca publiques tu archivo `licencia.ozo`, huella de equipo o datos del negocio.

Para adquirir, renovar o revisar una licencia:
[**licenses@ozopos.com**](mailto:licenses@ozopos.com)

---

## `06 // HARDWARE COMPATIBLE`

OZO PoS puede trabajar con:

- Lectores USB que funcionen como teclado.
- Impresoras térmicas ESC/POS con rollos de 30, 40, 50, 58 y 80 mm.
- Impresión en modo texto o imagen, según el modelo.
- Cajón de dinero conectado por RJ11 a una impresora compatible.
- Básculas conectadas mediante puerto serie compatible.

La compatibilidad final depende del controlador y del protocolo del dispositivo.
Antes de comprar hardware para varias cajas, valida un equipo físico con la
impresión de prueba incluida en OZO PoS.

---

## `07 // DATOS Y RESPALDOS`

- SQLite local es la fuente principal de información.
- Las ventas continúan funcionando sin conexión.
- Cada equipo conserva su propia configuración y base de datos.
- Realiza respaldos frecuentes y guarda una copia fuera del disco principal.
- No reemplaces, edites ni abras manualmente la base mientras OZO PoS está activo.
- Antes de actualizar o mover el sistema, genera y verifica un respaldo.

> [!NOTE]
> **OZO Cloud permanece pausado en la rama estable 1.0.4.** La aplicación opera
> localmente y no realiza sincronización remota en esta versión.

---

## `08 // ACTUALIZACIONES`

OZO PoS consulta las publicaciones oficiales de GitHub y avisa cuando existe una
versión estable más reciente. Antes de actualizar:

1. Termina las ventas pendientes y cierra el turno cuando corresponda.
2. Crea un respaldo local.
3. Cierra completamente OZO PoS.
4. Descarga e instala la nueva versión estable.
5. Verifica acceso, productos, impresora y último corte.

Consulta el [historial de cambios](./CHANGELOG.md) y las
[publicaciones oficiales](https://github.com/notTao/ozo-pos/releases).

---

## `09 // PROBLEMAS CONOCIDOS EN 1.0.4g`

- En papel de 58 mm, importes de más de siete cifras pueden recortarse dentro de
  la tabla de artículos; el total general se imprime completo.
- OZO Cloud no sincroniza en la rama 1.0.4 porque permanece pausado.
- El comportamiento físico de impresión puede variar según el controlador y la
  implementación ESC/POS de cada modelo.

---

## `10 // SOPORTE`

Al solicitar ayuda, incluye:

- Versión de OZO PoS.
- Versión de Windows.
- Mensaje exacto mostrado en pantalla.
- Pasos para reproducir el problema.
- Modelo de impresora u otro dispositivo involucrado.

No adjuntes contraseñas, licencias, bases de datos ni información sensible salvo
que soporte te proporcione un canal y procedimiento seguro.

**Soporte:** [support@ozopos.com](mailto:support@ozopos.com)<br />
**Licencias:** [licenses@ozopos.com](mailto:licenses@ozopos.com)<br />
**Sitio web:** [ozopos.com](https://ozopos.com)

---

## `11 // TECNOLOGÍA`

OZO PoS está construido con **Tauri 2**, **Rust**, **React**, **TypeScript** y
**SQLite**, bajo una arquitectura local-first. La interfaz se ejecuta dentro de
WebView2 y el núcleo nativo administra persistencia, licencias, respaldos e
impresión.

Para información técnica adicional consulta
[Cómo está hecho OZO PoS](./ACERCA-DE-OZO-POS.md).

---

<div align="center">

### `VENDE LOCAL // RESPALDA SEGURO // MANTÉN EL CONTROL`

**OZO PoS · © OZO · Todos los derechos reservados**

Este software no se distribuye bajo una licencia de código abierto.

</div>
