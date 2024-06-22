cantidadpiezas = 0

while True:
    codigopieza = int(input("Ingrese el código de la pieza a procesar (0 para terminar): "))
    
    if codigopieza == 0:
        break
    
    if 1 <= codigopieza <= 99:
        cantidadcomponente = 0
        preciototaldelaspiezas = 0
        
        print("Recuerde que se ingresa primero los dos primeros dígitos del código de componente y luego los dos dígitos del código de pieza.")
        print("Un ejemplo sería 30(cc) y 42 (cp).")
        print("Quedando tal como resultado 3042.")
        
        while True:
            codigodecomponente = int(input(f"Ingrese el código de componente para la pieza {codigopieza} o ingrese (0) para finalizar: "))
            
            if codigodecomponente == 0:
                break
            
            codigocomponentevalido = codigodecomponente % 100
            
            while codigocomponentevalido != codigopieza:
                print("Código de componente inválido para la pieza, por favor recuerde los requisitos. Ingrese un código válido:")
                codigodecomponente = int(input())
                codigocomponentevalido = codigodecomponente % 100
            
            precioComponente = float(input(f"Ingrese el precio del componente {codigodecomponente}: "))
            
            while precioComponente < 10 or precioComponente > 999.99:
                print("Precio inválido. Debe estar entre $10 y $999.99:")
                precioComponente = float(input())
            
            preciototaldelaspiezas += precioComponente
            cantidadcomponente += 1
        
        print(f"Precio total de la pieza {codigopieza}: ${preciototaldelaspiezas}")
        cantidadpiezas += 1
    else:
        print("Código de pieza inválido, por favor ingrese un número entre 01 y 99.")

print("Cantidad de piezas procesadas:", cantidadpiezas)
