# APE 4: Integración de clases, objetos y métodos

Ejercicios resueltos en **Java** sobre clases, objetos, métodos y colaboración entre clases.

| | |
|---|---|
| **Nombre** | Anthony Daniel Armas Jaya |
| **Docente** | Ing. José Rubén Caiza Caizabuano |
| **Fecha** | 29/10/2026 |
| **Curso** | 1er Semestre |
| **Paralelo** | B |
| **Asignatura** | Algoritmos y Lógica de Programación |

## Contenido

```
APE/
├── README.md
├── APE4_Ejercicios_Resueltos_Anthony.pdf
├── Ejercicio1_Libro_Autor/
│   └── Main.java
├── Ejercicio2_Rectangulo/
│   └── Main.java
├── Ejercicio3_Producto_Venta/
│   └── Main.java
├── Ejercicio4_Transferencias/
│   └── Main.java
└── Ejercicio5_Biblioteca/
    └── Main.java
```

Cada ejercicio está en su propia carpeta con un `Main.java` independiente. El archivo
`APE4_Ejercicios_Resueltos_Anthony.pdf` reúne los enunciados, el código y las salidas.

## Ejercicios

| # | Ejercicio | Tema | Clases |
|---|-----------|------|--------|
| 1 | Libro y Autor | Objeto como atributo | `Autor`, `Libro` |
| 2 | Rectángulo | Firmas de métodos y tipos de retorno | `Rectangulo` |
| 3 | Producto y Venta | Objeto como parámetro | `Producto`, `Venta` |
| 4 | Transferencias | Objeto como parámetro | `Cuenta` |
| 5 | Biblioteca | Colaboración entre clases | `Usuario`, `Libro`, `Prestamo` |

### Ejercicio 1: Libro y Autor
`Libro` tiene un atributo de tipo `Autor` y el método `mostrarInformacion()` imprime el título,
el año y el nombre del autor. En `main` se crean 2 libros.

### Ejercicio 2: Rectángulo
`Rectangulo` (base, altura) con los métodos `calcularArea()`, `calcularPerimetro()`,
`esCuadrado()`, `obtenerDescripcion()` y `mostrar()`, cada uno con su tipo de retorno correcto.

### Ejercicio 3: Producto y Venta
`Producto.reducirStock(int cantidad)` solo reduce el stock si hay suficiente. `Venta.aplicar(Producto producto)`
reduce el stock y muestra el total a pagar.

### Ejercicio 4: Transferencias
`Cuenta.transferir(Cuenta destino, double monto)` retira el monto de la cuenta actual y lo
deposita en la cuenta destino solo si hay fondos. Se prueba una transferencia válida y otra que falla.

### Ejercicio 5: Biblioteca
`Prestamo` relaciona un `Usuario` con un `Libro`. Su método `registrar()` intenta prestar el libro y
muestra un mensaje según el resultado. Dos usuarios piden el mismo libro.

## Cómo ejecutar

Requisitos: tener instalado el **JDK** (Java 8 o superior).

Desde la carpeta de un ejercicio, por ejemplo el 1:

```bash
cd Ejercicio1_Libro_Autor
javac Main.java
java Main
```

También se puede abrir cada `Main.java` en VS Code y ejecutarlo con el botón **Run**.

## Salidas de ejemplo

**Ejercicio 2: Rectángulo**
```
Rectangulo de 4.0 x 6.0
Area: 24.0
Perimetro: 20.0
Es cuadrado: false
```

**Ejercicio 3: Producto y Venta**
```
Total a pagar: 1000.0
Laptop | Precio: 500.0 | Stock: 8
Stock insuficiente.
Laptop | Precio: 500.0 | Stock: 8
```

**Ejercicio 4: Transferencias**
```
Transferencia exitosa.
Fondos insuficientes.
Ana: $70.0
Luis: $80.0
```

**Ejercicio 5: Biblioteca**
```
Ana recibio: Java basico
Libro no disponible para Luis
```

## Autor

**Anthony Daniel Armas Jaya** · 1er Semestre, Paralelo B
