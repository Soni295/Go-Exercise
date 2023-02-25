# Lesion 1
## Estructura basica de un programa en go.

1. Los ficheros de golang tienen una terminacion `.go`.
2. Los mismos en la primera linea deben tener el nombre del paquete al
que pertenecen, el principal se llama `main`.
3. El programa se ejecutara dentro de funciones, la principal se llama igual
que el paquete principal(`main`).
4. La funcion `print()` imprime por terminal el tipo de dato(sin formatear)
que se le pasa por parametro. En este caso imprime por terminal `"hola mundo"`

## Ejemplo:
```go
package main
func main(){print("hola mundo")}
```
---
### Consejo
Go no necesita identacion, incluso gran parte del codigo se podria poner en un
parde lineas.
Pero por convension Go usa una identacion por taburacion con una longitud de 8
espacios cada taburacion. y un espacio entre la primera linea, las demas entre
funciones.

```go
package main

func main() {
	print("hola mundo")
}
```

5. Para ejecutar un programa en golang se ejecuta en la terminal `go run <nombre del fichero principal>`
6. En este ejemplo seria
```bash
$ go run main.go
hello world%
```

7. Esta forma de ejecutar seria la de desarrollo. Porque en produccion, lo
razonable seria compilarlo en binario.
Esa es una de las ventajas de go tiene un tiempo rapido de compilacion para
desarrollo, y uno para contruir el binario para produccion.
8. Para contruir el binario es basicamente el mismo comando pero en vez de run,
se usa `build`, esto creara un binario en cualquier sistema operativo, que
luego se podra ejecutar.
```bash
$ go build main.go
```

9. Para ejecutar este binario se escribe el comando `./<nombre del binario>` en
este caso ./main
