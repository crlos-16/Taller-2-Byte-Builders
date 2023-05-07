# Taller-2-Byte-Builders
![image](https://user-images.githubusercontent.com/124606636/225486236-e4618eec-16f2-465f-b317-142d70c5942e.png)
# Ejercicios
# (1)Desarrollar un programa que ingrese un número entero n y separe todos los digitos que componen el número.
    #Pedimos al usuario que ingrese un número entero
    numero = int(input("Ingrese un número entero: "))
    #Convertimos el número ingresado en una cadena de texto
    cadena = str(numero)
    #Creamos una lista vacía para almacenar los dígitos
    digitos = []
    # Iteramos sobre cada carácter de la cadena
    for caracter in cadena:
    #Convertimos el carácter en un entero y agregarlo ala lista de dígitos
      digito = int(caracter)
      digitos.append(digito)
    #Imprimimos la lista de dígitos
    print(digitos)
# (2)Desarrolle un programa que ingrese un número flotante y separe su parte entera de la parte decimal, y luego entre los dígitos tanto de la parte entera como de la decimal.
   
    dato = float(input("dime un numero: "))
    #ingresar un dato flotante(parte entera y decimal)
    decimal = dato - (int(dato)) 
    #Se declara la variable decimal en la cual solo se toma el valor flotante
    ignorando la parte entera
    entero = (int(dato))
    #se decalra la variable entero en la cual se omite la parte flotante  
    print ("la parte entera es")
    print(entero)
    #imprimir parte entera del número digitado
    print ("la parte decial es")
    print(decimal)
    #imprimir la parte decimal del número digitado
# (3)Desarrollar un programa que permita ingresar dos números enteros y determinar si se tratan de números espejos.
    #Pedimos al usuario que ingrese dos números enteros
    primer_numero = int(input("Por favor ingresa el primer número entero: "))
    segundo_numero = int(input("Por favor ingresa el segundo número entero: "))
    #Convertimos los números ingresados en cadenas de texto
    cadena_primer_numero = str(primer_numero)
    cadena_segundo_numero = str(segundo_numero)
    #Verificamos si las cadenas de texto son iguales a sus versiones invertidas
    if cadena_primer_numero == cadena_segundo_numero[::-1]:
        print("Los números ingresados son espejos.")
    else:
        print("Los números ingresados no son espejos.")



    



   
