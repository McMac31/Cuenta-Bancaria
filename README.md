# Datos bancarios
Valores= [] #Se crea una lista vacia
accion = input("¿Quiere ingresar la transaccion? (s, n)") #Pregunta si quiere ingresar dinero
while accion=="s": #Se usa el while si se usa "S"
    Dinero = int(input("¿Cuanto dinero quiere introducir?")) #Pregunta el dinero a introducir
    Valores.append(Dinero) #Se le añade valores a la lista
    print("Guardando Valor...") #Le muestra al usuario que paso con el valor introducido
    accion= input("¿Quiere introducir otro valor? (s/n)") #Empieza el bucle hasta que no quiera ingresar otro valor
Suma= sum(Valores) #Hace la suma de la lista
print(f"Usted ha introducido {Valores}") #Enseña la lista 
print(f"La suma de sus ingresos es {Suma}€") #Suma la lista 
print(f"Su promedio de ingresos es  {Suma/Valores.count(Dinero)}€")#Hace el promedio de la lista
