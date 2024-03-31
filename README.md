barman = "billy"
bff = "gabriel cardillo"
minaccia = "emanuele salducco"
numeri = [1, 2, 3, 4, 5, 6]
num_analco = [1, 2, 3]

alcolici = ["margarita: 1,50€", "negroni: 2.50€", "billy cocktail: 3€", "acqua naturale: 1€", "acqua frizzante: 1,10€", "coca cola: 1,50€"]
analcolici = ["acqua naturale: 1€", "acqua frizzante: 1,10€", "coca cola: 1,50€"]

print("Benvenuto alla Billy House, io sono Billy.")
print("Innanzitutto, come ti chiami?")
nome_cliente = input()

if nome_cliente == bff:
    print("Oh, che bella sorpresa! Ti vado a preparare il tuo cocktail preferito.")
elif nome_cliente == minaccia:
    print("Aspetta, quell'Emanuele Salducco, quello che è stato appena condannato a 15 anni di carcere?!? ESCI SUBITO DAL MIO BAR!!!!!! >:")
else:
    print("Ok, mi può specificare il suo anno di nascita, signor " + nome_cliente + "?")
    anno_di_nascita = int(input())
    eta_cliente = 2024 - anno_di_nascita

    if eta_cliente >= 18:
        print("Ecco la lista dei drink alcolici disponibili:")
        for idx, drink in enumerate(alcolici, start=1):
            print(f"{idx}. {drink}")
        
        while True:
            scelta = int(input("Scelga un numero corrispondente al drink che desidera: "))
            if scelta in numeri:
                print("Perfetto! Può pagare alla cassa.")
                break
            else:
                print("Scelta non valida. Riprovi.")
        
    else:
        print("Ecco la lista dei drink analcolici disponibili:")
        for idx, drink in enumerate(analcolici, start=1):
            print(f"{idx}. {drink}")
        
        while True:
            scelta = int(input("Scelga un numero corrispondente al drink che desidera: "))
            if scelta in num_analco:
                print("Perfetto! Può pagare alla cassa.")
                break
            else:
                print("Scelta non valida. Riprovi.")


<!---
antoniosalducco/antoniosalducco is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
