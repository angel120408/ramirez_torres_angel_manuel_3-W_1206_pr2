# Codigo 1 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Funcion que muestre el saludo Hey amigos! cada vez que se le pida

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Funcion que muestre el saludo Hey amigos! cada vez que se le pida")
print(" ")

class Saludo:
    def __init__(self):
        # Constructor de la clase Saludo
        pass

    def mostrar_saludo(self):
        # Muestra el mensaje de saludo
        print("Hey amigos!")
       
# Crear una instancia de la clase Saludo
mi_saludo = Saludo()
# Llamar al método para mostrar el saludo
mi_saludo.mostrar_saludo()


![image](https://github.com/user-attachments/assets/10ecb6d6-fe1c-4c83-955a-b80aa6357900)
![image](https://github.com/user-attachments/assets/922fcd9c-fab1-47d2-8cfb-8f197e8b8348)


# Codigo 2 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Dar un string <nombre> y despliegue un saludo ¡hola <nombre>!.

print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Dar un string <nombre> y despliegue un saludo ¡hola <nombre>!.")
print(" ")


def obtener_nombre():
    # Solicita al usuario que ingrese su nombre
    return input("Ingresa tu nombre: ")

def mostrar_saludo(nombre):
    # Muestra un saludo personalizado usando el nombre proporcionado
    print(f"¡Hola {nombre}!")

def main():
    # Función principal que coordina el flujo del programa
    nombre_usuario = obtener_nombre()  # Llama a la función para obtener el nombre
    mostrar_saludo(nombre_usuario)      # Llama a la función para mostrar el saludo

# Ejecutar la función principal si el script se está ejecutando directamente
if __name__ == "__main__":
    main()

![image](https://github.com/user-attachments/assets/4fd6e907-404e-4227-972f-d7f164abb9bd)
![image](https://github.com/user-attachments/assets/2d592091-cab3-45a5-896b-7792bb08be94)
![image](https://github.com/user-attachments/assets/54c6b01d-d119-43ec-8b99-80499b9396a1)



# Codigo 3 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Dar un entero positivo y resuelva su factorial.

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Dar un entero positivo y resuelva su factorial.")
print(" ")


import math  # Importa la biblioteca math, que contiene funciones matemáticas

# Solicita un entero positivo al usuario
numero = int(input("Introduce un entero positivo: "))

# Verifica si el número es negativo
if numero < 0:
    print("Por favor, introduce un número entero positivo.")
else:
    # Calcula el factorial usando la función factorial de la biblioteca math
    resultado = math.factorial(numero)
    
    # Imprime el resultado
    print(f"El factorial de {numero} es {resultado}.")

![image](https://github.com/user-attachments/assets/b8cc8eb0-37d9-43bd-8359-5a58357d3d51)
![image](https://github.com/user-attachments/assets/4c1524d1-a6be-4ba8-970e-b38e18077d1e)



# Codigo 4 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Calcular total de una factura luego del IVA. 
primero obtener la cantidad sin IVA 
luego el porcentaje de IVA a aplicar, 
por ultimo devolver el total de la factura. 
Si se da la función sin pasarle un porcentaje de IVA, deberá aplicar un 21%.


print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Calcular total de una factura luego del IVA.")
print("primero obtener la cantidad sin IVA  ")
print("luego el porcentaje de IVA a aplicar, ")
print("por ultimo devolver el total de la factura.")
print("Si se da la función sin pasarle un porcentaje de IVA, deberá aplicar un 21%.")
print(" ")

# Solicitar la cantidad sin IVA al usuario
cantidad_sin_iva = float(input("Introduce la cantidad sin IVA: "))

# Solicitar el porcentaje de IVA al usuario, si lo desea
porcentaje_input = input("Introduce el porcentaje de IVA (deja vacío para aplicar 21%): ")

# Verificar si se ingresó un porcentaje de IVA
if porcentaje_input:
    # Convertir el input a float si se proporciona un porcentaje
    porcentaje_iva = float(porcentaje_input)
else:
    # Si no se proporciona, usar el valor por defecto de 21%
    porcentaje_iva = 21  

# Calcular el IVA multiplicando el porcentaje por la cantidad sin IVA
iva = (porcentaje_iva / 100) * cantidad_sin_iva

# Calcular el total de la factura sumando la cantidad sin IVA y el IVA
total_factura = cantidad_sin_iva + iva

# Mostrar el resultado final al usuario
print(f"El total de la factura, incluyendo IVA, es: {total_factura:.2f}")


![image](https://github.com/user-attachments/assets/2f23c63b-955f-4536-b231-84fc453ee633)
![image](https://github.com/user-attachments/assets/3a6db5ea-598e-441e-bf7f-87fa0972af5e)



# Codigo 5 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Calcular el área de un círculo  y el volumen 
otra que calcule el volumen de un cilindro y utilice  primera función.

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Calcular el área de un círculo  y el volumen ")
print("otra que calcule el volumen de un cilindro y utilice  primera función. ")
print(" ")

import math  # Importar la biblioteca matemática para usar constantes y funciones

# Función para calcular el área de un círculo
def calcular_area_circulo(radio):
    #Calcula el área de un círculo dado su radio.

    #param radio: Radio del círculo
    #return: Área del círculo
    
    area = math.pi * (radio ** 2)  # Fórmula: π * r²
    return area  # Retornar el área calculada

# Función para calcular el volumen de una esfera
def calcular_volumen_esfera(radio):
    #Calcula el volumen de una esfera dado su radio.

    #param radio: Radio de la esfera
    #return: Volumen de la esfera
    
    volumen = (4/3) * math.pi * (radio ** 3)  # Fórmula: (4/3) * π * r³
    return volumen  # Retornar el volumen calculado

# Función para calcular el volumen de un cilindro
def calcular_volumen_cilindro(radio, altura):
    
    #Calcula el volumen de un cilindro utilizando el área de su base.

    #param radio: Radio de la base del cilindro
    #param altura: Altura del cilindro
    #return: Volumen del cilindro
    
    area_base = calcular_area_circulo(radio)  # Calcular el área de la base del cilindro
    volumen = area_base * altura  # Fórmula: área de la base * altura
    return volumen  # Retornar el volumen calculado

# Solicitar el radio al usuario
radio = float(input("Introduce el radio: "))  # Conversión del input a float

# Calcular y mostrar el área del círculo
area = calcular_area_circulo(radio)  # Llamar a la función para calcular el área
print(f"El área del círculo es: {area:.2f}")  # Imprimir el área formateada a 2 decimales

# Calcular y mostrar el volumen de la esfera
volumen_esfera = calcular_volumen_esfera(radio)  # Llamar a la función para calcular el volumen
print(f"El volumen de la esfera es: {volumen_esfera:.2f}")  # Imprimir el volumen formateado

# Solicitar la altura del cilindro al usuario
altura = float(input("Introduce la altura del cilindro: "))  # Conversión del input a float

# Calcular y mostrar el volumen del cilindro
volumen_cilindro = calcular_volumen_cilindro(radio, altura)  # Llamar a la función para calcular el volumen
print(f"El volumen del cilindro es: {volumen_cilindro:.2f}")  # Imprimir el volumen formateado


![image](https://github.com/user-attachments/assets/4531e01b-7f36-493f-86e9-fff924bcce2d)
![image](https://github.com/user-attachments/assets/7cde1a22-5580-4043-9ddb-cd277f9a6276)
![image](https://github.com/user-attachments/assets/3a47c881-8eca-4903-bc91-f3d7709117a4)



# Codigo 6 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Capturar dirección de email. Desplegar mensaje si la dirección es válida o no, siendo que una función lo revisar por tener la @ solo así es valida

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Capturar dirección de email. Desplegar mensaje si la dirección es válida o no")
print("siendo que una función lo revisar por tener la @ solo así es valida")
print(" ")


import re  # Importar la biblioteca de expresiones regulares

def es_email_valido(email):

    #Verifica si la dirección de email es válida utilizando una expresión regular simple.

    # Patrón básico para verificar que hay un '@' y que hay texto antes y después
    patron = r'^[^@]+@[^@]+\.[^@]+$'  # Regex: algo antes de @, algo después de @, un punto y algo más
    return re.match(patron, email) is not None  # Retorna True si coincide con el patrón

# Solicitar la dirección de email al usuario
email = input("Introduce tu dirección de email: ")  # Leer el input del usuario

# Verificar si la dirección de email es válida
if es_email_valido(email):
    print("La dirección de email es válida.")  # Mensaje si el email es válido
else:
    print("La dirección de email no es válida. Asegúrate de que tenga un formato correcto con '@'.")  # Mensaje si no es válido


![image](https://github.com/user-attachments/assets/182a5743-28e2-443a-b64a-d561ae5e143f)
![image](https://github.com/user-attachments/assets/8b10e94a-105f-41bb-b91b-83a899993821)



# Codigo 7 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Función que de un string, regrese la longitud de la última palabra. Las palabras tienen separación por uno o más espacios.


print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Función que de un string, regrese la longitud de la última palabra. ")
print("Las palabras tienen separación por uno o más espacios. ")
print(" ")


def longitud_ultima_palabra(s):
    # Eliminamos los espacios al inicio y al final del string
    s = s.strip()
    
    # Esto maneja múltiples espacios automáticamente
    palabras = s.split()
    
    # Si hay palabras, devolvemos la longitud de la última
    # De lo contrario, devolvemos 0
    return len(palabras[-1]) if palabras else 0

# Ejemplo de uso
texto = "   Hola,    mundo   "
# Llama a la función y muestra la longitud de la última palabra
print(input("INTRODUCE UN TEXTO POR FAVOR"))

print(longitud_ultima_palabra(texto))  

![image](https://github.com/user-attachments/assets/6611806b-9572-4eac-8da6-ca364bda49b2)
![image](https://github.com/user-attachments/assets/2a185bea-84ef-42c4-aa33-d087ffc96d11)
![image](https://github.com/user-attachments/assets/4f1d82d2-b560-4525-bc5a-f6e78394248f)



# Codigo 8 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Definir una función (), que tome tres números como argumentos y devuelva el
mayor de ellos.

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Definir una función (), que tome tres números como argumentos")
print("y devuelva el mayor de ellos.")
print(" ")


def mayor_de_tres(a, b, c):
    # Creamos una lista con los tres números
    numeros = [a, b, c]
    print(input("Ingresa un numero"))
    print(input("Ingresa un segundo numero"))
    print(input("Ingresa un tercer numero"))
    
    # Inicializamos una variable para almacenar el mayor
    mayor = numeros[0]
    
    # Recorremos la lista de números
    for num in numeros:
        # Si encontramos un número mayor, lo actualizamos
        if num > mayor:
            mayor = num
    
    # Devolvemos el mayor de los tres números
    return mayor
print(" ")
# Ejemplo de uso
resultado = mayor_de_tres(10, 25, 15)
# Muestra el mayor de los tres números
print("El numero mayor es")
print(resultado) 


![image](https://github.com/user-attachments/assets/9a58c1e1-2aec-4b74-afbf-cb9407981c14)
![image](https://github.com/user-attachments/assets/b3806b7f-802b-439f-8411-272b0022de90)
![image](https://github.com/user-attachments/assets/ea12ead5-6893-437f-8218-f2fc59e119d2)




# Codigo 9 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Escribir una funcion sum() y una función multip() que sumen y multipliquen respectivamente
todos los números de una lista. Por ejemplo: sum([1,2,3,4]) debería devolver 10 y multip([1,2,3,4])
debería devolver 24.

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Escribir una funcion sum() y una función multip() que sumen y multipliquen respectivamente")
print("todos los números de una lista. Por ejemplo: sum([1,2,3,4]) debería devolver 10 y multip([1,2,3,4])")
print("multip([1,2,3,4]) debería devolver 24.")
print(" ")


def sum(numeros):
    # Inicializamos la suma en 0
    total = 0
    # Iteramos sobre cada número en la lista y lo sumamos
    for num in numeros:
        total += num
    # Devolvemos la suma total
    return total

def multip(numeros):
    # Inicializamos el producto en 1
    producto = 1
    # Verificamos si la lista está vacía para evitar multiplicaciones innecesarias
    if not numeros:
        return 0  # Retornamos 0 si la lista está vacía
    # Iteramos sobre cada número en la lista y lo multiplicamos
    for num in numeros:
        producto *= num
    # Devolvemos el producto total
    return producto

# Ejemplos de uso
suma_resultado = sum([1, 2, 3, 4])
multip_resultado = multip([1, 2, 3, 4])

# Muestra los resultados
print(suma_resultado)  
print(multip_resultado) 



![image](https://github.com/user-attachments/assets/431f766c-c7d1-4408-8663-f2b5e1832b77)
![image](https://github.com/user-attachments/assets/890f987d-c3e4-48b1-ab0d-5787eb4607ed)
![image](https://github.com/user-attachments/assets/f27e9bf4-a29d-417f-b6ff-14b727687900)



# Codigo 10 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Escribir una función que tome un carácter y devuelva True si es una vocal, de lo contrario
devuelve False.

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print("Escribir una funcion sum() y una función multip() que sumen y multipliquen respectivamente")
print("todos los números de una lista. Por ejemplo: sum([1,2,3,4]) debería devolver 10 y multip([1,2,3,4])")
print("multip([1,2,3,4]) debería devolver 24.")
print(" ")


def es_vocal(caracter):
    # Convertimos el carácter a minúscula para simplificar la comparación
    caracter = caracter.lower()
    
    # Definimos las vocales en minúscula
    vocales = "aeiou"
    
    # Verificamos si el carácter está en la cadena de vocales
    return caracter in vocales

# Ejemplos de uso
print(es_vocal('a'))  # Salida: True
print(es_vocal('B'))  # Salida: False
print(es_vocal('E'))  # Salida: True
print(es_vocal('o'))  # Salida: True
print(es_vocal('x'))  # Salida: False


![image](https://github.com/user-attachments/assets/76523b50-e6d7-4b80-a893-0351c699ef5b)
![image](https://github.com/user-attachments/assets/a7a29954-db88-43b6-b5d5-f74637c56fa4)
![image](https://github.com/user-attachments/assets/2a56c0f4-b7d1-49e9-89c8-751264a96fab)





# Codigo 11 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
- Que saque la distancia dirigida entre dos puntos

print(" ")
print("Ramirez Torres Angel Manuel 3°W")
print("Numer de control: 1206")
print("-INSTRUCCIONES-")
print(" Que saque la distancia dirigida entre dos puntos")
print(" ")


class Punto:
    def __init__(self, x, y):
        # Inicializa las coordenadas del punto
        self.x = x
        self.y = y

    def distancia_dirigida(self, otro):
        # Calcula la distancia dirigida hacia otro punto
        return (otro.x - self.x, otro.y - self.y)

# Función para obtener un punto a partir de la entrada del usuario
def obtener_punto():
    x = float(input("Ingresa la coordenada x: "))  # Solicita la coordenada x
    y = float(input("Ingresa la coordenada y: "))  # Solicita la coordenada y
    return Punto(x, y)  # Retorna un nuevo objeto Punto

# Ejemplo de uso
print("Ingrese las coordenadas del primer punto:")
punto1 = obtener_punto()  # Obtiene el primer punto del usuario
print("Ingrese las coordenadas del segundo punto:")
punto2 = obtener_punto()  # Obtiene el segundo punto del usuario

# Calculamos la distancia dirigida entre los dos puntos
resultado = punto1.distancia_dirigida(punto2)

# Muestra el resultado
print(f"La distancia dirigida entre los puntos es: {resultado}")  # Muestra el vector de distancia



![image](https://github.com/user-attachments/assets/db7e3b5d-f63a-4992-a60e-70bb5964698f)
![image](https://github.com/user-attachments/assets/adab8e03-545a-42fb-a73c-4aded1a80ef3)
![image](https://github.com/user-attachments/assets/9be73fd0-98ba-4937-ac88-83abedadc274)



