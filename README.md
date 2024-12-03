# programas
import random
print (F"Bienvenido al juego de los dados locos")
print (F"para continuar el ganador se llevara un celular")
def lanzar_dado():
    return random.randint(2, 10)

def main():
    # 1. Pedir el nombre del jugador 1
    nom1 = input("Ingrese tu nombre Jugador 1: ")
    
    # 2. Pedir el nombre del jugador 2
    nom2 = input("Ingrese tu nombre  Jugador 2: ")

    # 3. Pedir que el jugador 1 presione Enter para lanzar el dado
    input(f"{nom1}, presiona Enter para lanzar el dadito...")
    
    # 4. Capturar el valor y guardar en una variable llamada lanzamiento_jugador1
    lanzamiento_jugador1 = lanzar_dado()
    
    # 5. Mostrar el valor obtenido
    print(f"{nom1} :ooo sacaste {lanzamiento_jugador1}")

    # 6. Pedir que el jugador 2 presione Enter para lanzar el dado
    input(f"{nom2}, presiona Enter para lanzar el dado...")
    
    # 7. Capturar el valor y guardar en una variable llamada lanzamiento_jugador2
    lanzamiento_jugador2 = lanzar_dado()
    
    # 8. Mostrar el valor obtenido
    print(f"{nom2} :000 sacaste {lanzamiento_jugador2}")


    if lanzamiento_jugador1 > lanzamiento_jugador2:
        print(f"El ganador es  {nom1} Good ganaste el celular eres un loco o una loca!")
    elif lanzamiento_jugador2 > lanzamiento_jugador1:
        print(f"El ganador es  {nom2} Good ganaste el celular eres un loco o una loca! ")
    else:
        print(f"{nom1} y {nom2} empataron lastima nadie se lleva el celular que bobos :)))!")

if __name__ == "__main__":
    main()
