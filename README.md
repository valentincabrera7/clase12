class Perro:

    # Atributo de clase, que tambien se llama variable de clase. Le atribuimos la especie can a perro.
    especie = "Can"
    # Metodo constructor de la clase
    def __init__(self, nombre, raza):
        self.nombre = nombre # Atributo de instancia
        self.raza = raza



perro = Perro("Pipo", "Golden") # perro es una instancia (u objeto) de la clase Perro
perro2 = Perro("Pipe", "Labrador")
print(perro.nombre)
print(perro.raza)
print(perro2.nombre)
print(perro2.raza)


class Personaa():

    # Metodo constructor
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
        
    # Metodo de instancia
    def saludar(self): # recibe al objeto de la clase
        print(f"Hola soy {self.nombre}, tengo {self.edad} años y te estoy saludando!")


persona = Personaa(nombre="", edad="") # aca se instancia la clase Persona asignandole una variable
persona.saludar()


import math

class Circulo():

    pi = 3.14159
    pi = math.pi # no lo tengo en comillas el ejercicio para que ande pero asi importamos math, no haria falta poner la variable con el valor de pi

    def __init__(self, radio):
        self.radio = radio

    def calcular_area(self):
        return Circulo.pi * self.radio ** 2 
        
    
c = Circulo(7)
print(c.pi)
area = c.calcular_area()
print(area)


class Persona:
    
    def __init__(self, nombre, apellido, edad):
        self.nombre = nombre
        self.apellido = apellido
        self.edad = edad 


class Programador(Persona):
    pass


persona = Programador("Valentin", "Cabrera", 25) # argumentos que van a parar al metodo constructor
print(persona.nombre, persona.apellido, persona.edad)

