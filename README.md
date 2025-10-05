# my_notes.txt.
 operaciones de lectura y escritura en archivos de texto en Python


 
# Tarea: Operaciones de lectura y escritura en archivos de texto
# Autor: [Henry Condolo Moncada]
# Descripción: Este codigo desribe notas personales y
#               las lee línea por línea y las muestra en consola o pantalla.


# --- Escritura de archivo de texto ---
# Abrimos el archivo "my_notes.txt" en modo escritura ('w')
# Si el archivo ya existe, se sobrescribirá.
with open("my_notes.txt", "w") as file:
    # Escribimos tres líneas de notas personales
    file.write("1. Recordar practicar Python todos los días para mejorar la forma de aprender.\n")
    file.write("2. Leer sobre estructuras de datos y sus codigos.\n")
    file.write("3. Realizar una pausa activa cada hora con el fin de mejorar el estado de animo.\n")

# El archivo se cierra automáticamente al salir del bloque 'with'


# --- Lectura de archivo de texto ---
# Abrimos el archivo en modo lectura ('r')
with open("my_notes.txt", "r") as file:
    # Leemos el contenido línea por línea
    print("📘 Contenido del archivo my_notes.txt:\n")
    line = file.readline()  # Lee la primera línea

    # Mientras haya contenido, seguimos leyendo
    while line:
        print(line.strip())  # Mostramos la línea sin salto de línea extra
        line = file.readline()  # Lee la siguiente línea

# El archivo también se cierra automáticamente aquí

# Fin del programa
