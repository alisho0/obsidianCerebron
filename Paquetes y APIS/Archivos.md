
Hay diversos paquetes de los que manejan archivos

Algunos ejemplos:
- Path
- FileReader
- Files

Para encontrar un archivo: ``Path ruta = Path.of(xx/xx/xx.pdf);

También podemos chequear si existe: `boolean existe = Files.exist(ruta);`

Con `mismatch` podemos comparar los tamaños y bytes de dos direcciones y comprobar si son iguales. 0 indica que no coinciden y -1 que si coinciden.

Podemos crear archivos temporales con `createTempFile(prefijo, tipoDeArchivo);`, loquísimo, que se guardan en un directorio predeterminado, pero podemos especificar nuestro propio directorio con `createTempDirectory(prefijo);`

Cuando creas un directorio con `Path nuevoDirectorio = Files.createDirectories(Path.of("D:/HolaMundo"));`, para crear un archivo, tienes que crear un objeto Path que sea como el "hijo" del directorio a donde lo quieres poner: `Path nuevoArchivo = Files.createFile(nuevoDirectorio.resolve("nombreArchivo.txt"));`
