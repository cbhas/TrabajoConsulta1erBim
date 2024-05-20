# Modelos de Programación Concurrente en Kotlin
Kotlin se destaca por su modelo de programación concurrente basado en coroutines, esta ofrece una manera más ligera y mucho más fácil de gestionar tareas concurrentes en comparación con los hilos tradicionales utilizados en Java.

## Coroutines en Kotlin
Una coroutine es una instancia de una computación suspendible. Es conceptualmente similar a un hilo, en el sentido de que toma un bloque de código para ejecutarse que trabaja concurrentemente con el resto del código. Sin embargo, una coroutine no está ligada a ningún hilo en particular. Puede suspender su ejecución en un hilo y reanudarla en otro.

### Ejemplo de uso de coroutines en Kotlin:
import kotlinx.coroutines.*

fun main() = runBlocking {
    launch {
        delay(1000L)
        println("Coroutines!")
    }
    println("Hello,")
}