<<<<<<< HEAD
# LogToFile-CI24
=======
# cordova-plugin-logtofile-CI24

> Plugin de cordova para guardar los logs en el dispositivo android CI24.

## Instalación.

```bash
cordova plugin add cordova-plugin-logtofile--editar
```

## Uso

```javascript
// Configuración de la ruta donde se almacenarán los registros en el dispositivo.
window.logToFile.setLogfilePath('/LogsCI24/logs.txt', function () {
    //Mesanje de éxito.
}, function (err) {
    // Mensaje de error.
});

// Obtener l ruta de la instancia del registrador actual.
window.logToFile.getLogfilePath(function (logfilePath) {
    // Mensaje de éxito.
}, function (err) {
    // Mensaje de error.
});

// Obtener la ruta de los registros archivados.
window.logToFile.getArchivedLogfilePaths(function (archivedlogfiles) {
    // Mensaje de éxito.
}, function (err) {
    // Mensaje de error.
});

//Escribir logs en diferentes niveles.
window.logToFile.debug('Mensaje debug');
window.logToFile.info('Mensaje info');
window.logToFile.warn('Mensaje warn');
window.logToFile.error('Mensaje error');
```

## Nota:
El archivo de registro tiene un tamaño maximo de 200MB, cuando se sobrepase este tamaño, el archivo de registro actual se comprimirá y se genera un nuevo archivo.txt.
como maximo se tienen dos archivos: el actual y el .zip.

## Plataformas:
Android
>>>>>>> Plugin LogToFile CI24
