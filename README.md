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
-





# Codigo 8 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
-






# Codigo 9 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
-





# Codigo 10 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
-




# Codigo 11 De la Practica Numero 2 Creado Por Ramirez Torres Angel Manuel De 3°W NO.De Control: 1206
-
