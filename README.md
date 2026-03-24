try:
    with open("data.txt", "r") as soubor:
        obsah = soubor.read()
        print(obsah)

except FileNotFoundError:
    print("Soubor nebyl nalezen!")

except Exception as e:
    print("Nastala chyba:", e)
