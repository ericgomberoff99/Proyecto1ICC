# Proyecto1ICC

#Programa completo

import sys
import random

def Tabladeposiciones(usuario):
   print("*"*20)
   for jugador in Puntos():
       print(" "+Puntos(jugador)(0)+" "*(17-len(usuario))+Puntos(jugador)(1))

Puntos=[]

def InsertarRanking(usuario,puntos):
  conjunto=[usuario,puntos]
  Puntos.append(conjunto)

def BIENVENIDA():
  print("BIENVENIDO/A")
  usuario = input("Cual es tu nombre? : ")
  puntos=0
  InsertarRanking(usuario,puntos)
  print("Hola", usuario + "!")
  edad = input("Ingresa tu edad: ")

print(BIENVENIDA())

def Repaso1():
   print("Repaso nivel 1: \n Recordando los  operadores: \n\t Exponenciación→ ** →3**2=9 \n\t Identidad Unario → == → a==a \n\t Multiplicación→ *→ 4*3=12 \n\t División→ / → 12/3=4")
   print("Módulo (o resto)→ % → 13%5=3")
   print("Suma→ + → 5+5=10")
   print("Resta→ - → 14-10=4")
   print("Igual→ = → b=4, c=4, c=b")
   print("Distinto de→ != → b!=5")
   print("Menor que→< →5<19")
   print("Menor o igual que→<= → x<=4 ={..., -1,0,1,2,3,4}")
   print("Mayor que→ > → 6>1")
   print("Mayor o Igual que → >= → x>=1 ={1,2,3,4,...}")
   print("Conjunción→ and → x>10 and x<30")
   print("Disyunción→ or →  x>10 or y<30")

   print("recordando los tipos de números:")

   print("Cuando es un entero se usa “int”, ejemplo: Definir una variable entera.")
   print("x=int(input())")
   print("Cuando es un entero se usa “int”, ejemplo: Definir una variable entera.")
   print("x=int(input())")

   print("recordando las funciones básicas:")
   print("if _ condición _:")
   print("   _______")
   print("*nota: después de terminar la condición se ponen dos puntos (:) y la siguiente línea”) print (“se”)")
   print("empieza a escribir con un tab.")
   print("else:")
   print("*nota: la función else jamás lleva una condición, pero siempre lleva los dos puntos (:)")
   print("al final.")
   print("Elif __ Condición __:")
   print("   _______")
   print("*nota: después de terminar la función elif se ponen dos puntos (:) y la siguiente línea")
   print("se empieza a escribir con un tab. La función elif cumple la función de una else+if y”) print (“es”)")
   print("por eso que se puede condicionar.")
   print("Print(“abcde”)")
   print("*nota: no olvidar abrir y cerrar los paréntesis, además de las comillas.")
   print("*****recordando cómo realizar operaciones que no tenemos en la PC :****")
   print("Python no posee un lenguaje de operaciones matemáticas complejas; es por")
   print("esto que si vamos a realizar alguna, primero debemos importar el lenguaje")
   print("requerido de la siguiente manera: from math import ___ lo que se desea")
   print("importar ______.”)")
   print(" ")


def Repaso2():
   print("Bucle While:")
   print("Un bucle while permite repetir la ejecución de un grupo de instrucciones")
   print("mientras se cumpla una condición.")
   print("while _ condición _:")
   print("cuerpo del bucle")
   print("Ejemplo:")
   print("i = 1")
   print("while i <= 3:")
   print("print(i)")
   print("i=i+ 1")
   print("print(Programa terminado)")
   print("Resultado:")
   print("1")
   print("2")
   print("3")
   print("Programa terminado")
   print("Bucle for:")
   print("Un bucle for es un bucle que repite el bloque de instrucciones un número")
   print("predeterminado de veces. El bloque de instrucciones que se repite se suele”) print (“llamar cuerpo del bucle y cada repetición se suele llamar iteración.")
   print("for variable in elemento iterable (donde empieza,donde termina,salto):”)")
   print("cuerpo del bucle")
   print("Ejemplo:")
   print("print(""Comienzo"")")
   print("for i in [0, 1, 2]:")
   print("print(""Hola "", end="")")
   print("print()")
   print("print(Final')")
   print("Resultado:")
   print("Comienzo")
   print("Hola Hola Hola")
   print("Final")
   print("Listas:")
   print("Una lista tiene elementos desde 0 a n-1 siendo n la cantidad de elementos:")
   print("lista1 = ['A', 'B', 'C']")
   print("print(lista1)")
   print(">>['A', 'B', ,'C']")

   print("Para agregar un elemento nuevo a una lista que ya teníamos:")
   print("lista1.append(""D"")")
   print("print(lista1)")
   print(">>['A', 'B', 'C', 'D']")
   print("Para agregar un elemento nuevo a una lista que ya teníamos en un")
   print("determinado lugar:")
   print("lista = ['fido', 'mota']")
   print("lista.insert(1, 'dinky')")
   print("Para eliminar elementos de una lista, usamos pop y entre paréntesis la")
   print("posición o remove y escribimos el elemento que queremos borrar.")
   print("lista= ['fido', 'dinky', 'mota', 'kuki']")
   print("lista.pop(1)")
   print("lista.remove('mota')")

   print("Más operaciones con listas:")
   print("list.sum()")
   print("list.max()")
   print("list.min()")
   print("list.sort()")
   print("len(list)")


def Repaso3():
   print(" ")
   print ("Repaso nivel 3:")
   print ("Funciones:")
   print ("Una función, es un conjunto de instrucciones que realizan alguna tarea")
   print ("que se va a invocar más de una vez en un programa.")
   print ("Pueden recibir o no parámetros y pueden retornar un valor o pueden no")
   print ("retornar ningún valor.")
   print ("Se usa def para definir nuestra propia función a la cual nosotros mismo le")
   print ("damos un nombre.")
   print ("def escribe_media():\n\t media = (a + b) / 2 \n\t print(La media de {a} y {b} es: {media}') \n\t return")
   print ("a = 3")
   print ("b = 5")
   print ("escribe_media()")
   print ("print('Prograa terminado')")


def nivelación(nivel):
       if nivel == 1:
           print("Repaso del Nivel 1: ", Repaso1())
           print(Repaso2())
           print(Repaso3())
       elif nivel == 2:
           print("Repaso del Nivel 2: ", Repaso2())
           print(Repaso3())
       elif nivel == 3:
           print("Repaso del Nivel 3: ", Repaso3())
       elif nivel > 3 or nivel < 1:
           print("Ingrese un nivel dentro del rango")


def jugarTrivia():
   class Question(object):
       def __init__(self, question, answer, options):
           self.question = question
           self.answer = answer
           self.options = options

       def ask(self):
           print(self.question)
           for n, option in enumerate(self.options):
               print("%d) %s" % (n + 1, option))

           response = int(input("Respuesta: "))
           if response == self.answer:
               puntos += 1
               print ("CORRECTO")
               seguir = input("Para continuar presione ok o para salir de la sesion escriba chau")
               if seguir == "chau":
                   print(MENU())
           else:
               print("MAL")
               seguir = input("Para continuar presione ok o para salir de la sesion escriba chau")
               if seguir == "chau":
                   print(MENU())


   questions =[Question("¿Cuál es la forma correcta de escribir un bucle for?", 1,["for a in range(0, 3):", "for a in range(0..3)", "for(a=0; a<3; a++)", "for a in range(0.3)"]),
   Question("Para añadir una condición alternativa a una declaración condicional if se utiliza?", 2,
            ["elseif", "elif", "else if", "elsif"]),
   Question("¿Cómo se define una variable asignándole un valor?", 3,["number v = 0", "int v = 0", "v = 0", "var v = 0"]),
   Question("¿Cuál de los siguientes no es un operador de asignación válido?", 1, ["@=1", "-=1", "+=1", "|=1"]),
       Question("La forma correcta de escribir una función es", 3,
            ["function nombrefuncion()", "nombrefuncion: function()", "def nombrefuncion():",
             "define nombrefuncion()"]),
       Question("Para mostrar texto en la consola usamos el comando", 1, ["print", "p", "show", "console.log"]),
       Question("Una declaración condicional se escribe", 1,
            ["if v == true:", "if v == true", "if (v == true)", "if v == true then"]),
       Question("¿Cuál es la forma correcta de escribir un bucle while?", 1,
            ["while a < 5:", "while a in range(0..4)", "while (a < 5)", "while a foreach[0..4]"]),
       Question("¿Cuál de estas líneas producirá diez iteraciones sobre un bloque de código?", 4,
            ["for (x = 0; x < 10; x++){ }", "for x in range(9):", "while True", "for x in range (10)"]),
       Question("En python, ¿Es necesario cerrar cada declaración con un punto y coma ';' ?", 2, ["Si", "No"]),
       Question("Para que se utiliza la coma en una lista?", 3,
            ["unir elementos", "cerrar la lista", "separar los elementos", "no se utilizan comas"]),
       Question("Si dentro del parentesis de un print() se coloca una palabra en comillas, que representa", 1,
            ["imprimiras la palabra como string", "imprimiras el valor asigando a la palabra", "no imprimira nada",
             "imprimiras la funcion de asignada a la palabra"]),
       Question("Qué es “valor” en esta línea de código? valor=5", 4,
            ["funcion", "asignacion", "declaracion", "variable"]),
       Question("que diferencia hay entre 'int' y 'float'", 3, ["ninguna", "float es para texto e int para numeros",
                                                            "float es para numeros con decimales e int para enteros",
                                                            "int es para numeros con decimales y float para enteros"]),
       Question("¿Cuál será la salida del siguiente programa si años=15? print(años)", 2,
            ["'años'", "15", "años", "error"]),]

   random.shuffle(questions)

   for question in questions:
       question.ask()

def MENU():
   print("---- M E N Ú ----")
   print("1. Jugar Trivia")
   print("2. Repetir Repaso")
   print("3. Tabla de posiciones")
   opcionmenu = int(input(" Ingrese Opcion del Menu: "))
   if opcionmenu == 1:
       preparación = input("Estas listo? ").upper
       if preparación == "SI" or "si" or "sí" or "Si" or "Sí":
           print(" ")
           print(jugarTrivia())
       else:
           print(MENU())
   if opcionmenu == 2:
       print(nivelación(nivel))
       print(MENU())
   elif opcionmenu == 3:
       print(Tabladeposiciones(usuario))
       retorno = input("Regresar al Menu? : ")
       print(Puntajes)
       if retorno != "jnjn":
           print(MENU())
   else:
       print("Opción no valida")
   print(MENU())


print(usuario,", hay 3 niveles de juego basados en tu conocimiento de Python: 1, 2 y 3. (1 es el menor y 3 el mayor)")
nivel= int(input("¿Cuál es tu nivel?: "))
print(nivelación(nivel))

print(" ")
confirmación = input("escriba ok si entendió todo  ")
if confirmación != "popkmn":
   print(" ")
   print(MENU())

print(MENU())
