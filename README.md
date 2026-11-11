# Conciliador FEL · descargas

Programa para Windows que compara el reporte de facturas de ICG con el resumen de documentos emitidos de Filpro (facturación electrónica). Muestra:
- los totales de cada lado
- las facturas que faltan o sobran
- los documentos duplicados
- las anulaciones con o sin su devolución
- las diferencias de monto o de fecha

También explica de dónde sale la diferencia de totales y guarda el reporte en Excel.

## Descarga

Baja `ConciliadorFEL.exe` de la [última versión](https://github.com/arenas037/ConciliadorFEL-descargas/releases/latest).

No hay que instalar nada. Funciona en Windows 10 y 11 (usa .NET Framework 4.x, que ya trae Windows).

## Cómo se usa

1. Abre `ConciliadorFEL.exe`.
2. Arrastra los dos Excel a la ventana, en cualquier orden: el reporte de ICG y el de Filpro. El programa reconoce cuál es cada uno.
3. Haz clic en las tarjetas para ver el detalle. Con **Exportar a Excel** guardas el reporte completo.

Los archivos se procesan solo en tu equipo: el programa no se conecta a internet y no modifica los originales.

## Notas

- El antivirus puede retener el programa la primera vez que se abre, como pasa con cualquier programa nuevo.
- Para comprobar que el archivo no se alteró, compara su código SHA-256 con el de las notas de la versión. En PowerShell:
  `Get-FileHash .\ConciliadorFEL.exe`
