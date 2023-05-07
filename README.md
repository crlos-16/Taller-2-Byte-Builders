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
    
# (5)Desarrollar un programa que permita determinar el Minimo Comun Multiplo de dos numeros enteros. Abordar el problema desde la perspectiva iterativa como recursiva.
  
    a= int(input("Digite el primer número")
    b= int(input("Digite el segundo número"))
    #ingresar números enteros
    i=int(2)
    #el número debe ser divisible por 2 y entero
    while True: #condición verdadera 
       if i%a==0 and i%b==0:
       #el modulo de los números digitados debe ser entero por lo tanto debe ser = a 0
         m=i
         break
       i+=1 
    #La variable I debe ser positiva e igual a uno para asegurarse que es su minimo comun multiplo
print(m)

# (6)Desarrollar un programa que determine si en una lista no existen elementos repetidos.
     def Crear_lista(n):
    lista=[]
    for i in range(n):
        termino=input("Ingrese el elemento("+str(i+1)+")")#Ingresamos cada elemento de la lista
        lista.append(termino)
    return lista
     if __name__=="__main__":
    n = int(input("Ingrese el número de elementos que desea en la lista: "))#Pedir el numero de elementos
    lista=Crear_lista(n)
    print(lista)#Imprimimos la lista
    j=0#Definimos variable de contador
    x=0#Definimos variable que va ir indicando el index
    while j<len(lista):
        y=lista[x]#y sera igual al valor del x index en el que vaya
        if 1!=lista.count(y):#Revisa si el valor que tenga y se repite en la lista
            print("en la lista existen elementos que se repiten")#Imprimimos que existen elementos repetidos    
            break#Terminamos el ciclo de manera forzada
        else:#Si el valor que lleva y no se repite en el ciclo
            x+=1#Vamos al siguiente valor de y
            j+=1
            if x==len(lista):#Condicional para que solo se imprima al final del ciclo
                print("en la lista no se repite ningun elemento")
              
# (7)  Desarrollar un programa que determine si en una lista se encuentra una cadena de caracteres con dos o más vocales. Si la cadena existe debe imprimirla y si no existe debe imprimir 'No existe'.
     # Pedimos al usuario que ingrese una lista de cadenas de caracteres separadas por comas
     lista = input("Por favor ingresen una lista de cadenas de caracteres separadas por comas: ").split(",")
     #Creamos una variable para verificar si encontramos una cadena con dos o más vocales
     encontrado = False
     #Iteramos sobre cada cadena de la lista
     for cadena in lista:
       #Contamos el número de vocales en la cadena
       numero_vocales = 0
       for caracter in cadena:
         if caracter in "aeiouAEIOU":
             numero_vocales += 1
     #Verificamos si la cadena tiene dos o más vocales y si es así, la imprimimos y cambiamos el valor de la variable encontrado
       if numero_vocales >= 2:
          print(f"Encontramos una cadena '{cadena}' que tiene dos o más vocales.")
          encontrado = True
     #Si no encontramos ninguna cadena con dos o más vocales, imprimimos 'No        encontramos ninguna cadena con dos o más vocales'
      if not encontrado:
        print("No existe.")
# (8)Desarrollar un programa que dadas dos listas determine que elementos tiene la primera lista que no tenga la segunda lista
    def Crear_lista(n):#Funcion para crear listas
    lista=[]
    for i in range(n):
        termino=input("Ingrese el elemento("+str(i+1)+")")#Ingresamos cada elemento de la lista
        lista.append(termino)
    return lista
    if __name__=="__main__":
    n = int(input("Ingrese el número de elementos que desea en la lista1: "))#Pedir el numero de elementos
    lista1=Crear_lista(n)
    x = int(input("Ingrese el número de elementos que desea en la lista2: "))#Pedir el numero de elementos
    lista2=Crear_lista(x)
    print(lista1)
    print(lista2)
    lista_diferencia=lista1[:]#Creamos una lista igual a la lista1
    for i in lista1:#Recorremos cada elemento de la lista1
        if i in lista2:#Analisamos si el elemento de la lista1 esta dentro de la lista2 
            y=lista1.count(i)#Cuantas veces esta este elemento en la lista1
            while y!=0:#Ciclo mientras para quitar de la lista1 todos los elementos iguales que estan en esta
                lista_diferencia.remove(i)
                y-=1      
     print("los elementos que tiene la lista1 y que la lista 2 no tiene son"+str(lista_diferencia))#Imprimimos la lista de los elementos que no estan en la lista2

# (9)Resolver el punto 7 del taller 1 usando operaciones con vectores.
     n=5
     i=1
     lista=[]
     while i<=n:#Se ingresan todos los valores que van a estar dentro de la lista de 5 numeros
    x=int(input("ingrese el primer elemento"))
    lista.append(x)
    i+=1
    print(lista)
    promedio=sum(lista)/n#Se saca el promedio
    print("el promedio es: "+str(promedio))
    mediana=sorted(lista)#Se ordena la lista
    print("la mediana es: "+str(mediana[2]))#Se saca el valor intermedio de la lista
    promedio_multiplicativo=(lista[0]*lista[1]*lista[2]*lista[3]*lista[4])**     (1/5)#Se saca el promedio multiplicativo
    print("el promedio multiplicativo es: "+str(promedio_multiplicativo))
    print("los numeros ordenados de forma ascendente: "+str(mediana))#Se imprimen los numero de forma ascendente
    invertido=mediana.sort(reverse=True)
    print("los numero de ordenados de forma descendente: "+str(invertido))#Se           imprimen los numero de forma descendente
    potencia=max(lista)**min(lista)#Se calcula el numero mayor elevado al numero menor
    print("el mayor numero elevado al menor numero es: "+str(potencia))
    raiz=min(lista)**(1/3)#Se le saca raiz cubica al numero menor
    print("la raiz cubica del menor es: "+str(raiz))
   
# (10) Desarrollar un algoritmo que determine si una matriz es mágica. Se dice que una matriz cuadrada es mágica si la suma de cada una de sus filas, de cada una de sus columnas y de cada diagonal es igual.
    
    def matriz_magica(matriz):
    #suma de la primera fila
    suma_fila = sum(matriz[0])
    #la suma de cada fila es igual a la suma de la primera fila
    for fila in matriz:
        if sum(fila) != suma_fila:
            return False
    #la suma de cada columna es igual a la suma de la primera fila
    for i in range(len(matriz)):
        if sum(matriz[j][i] for j in range(len(matriz))) != suma_fila:
            return False
    #la suma de la diagonal principal es igual a la suma de la primera fila
    if sum(matriz[i][i] for i in range(len(matriz))) != suma_fila:
        return False
    #la suma de la diagonal secundaria es igual a la suma de la primera fila
    if sum(matriz[i][len(matriz)-i-1] for i in range(len(matriz))) != suma_fila:
        return False
    #Si todas las sumas son iguales, la matriz es mágica
    return True

    matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
    if matriz_magica(matriz):
         print("La matriz mágica")
       else:
         print(" No es mágica")
     



   
