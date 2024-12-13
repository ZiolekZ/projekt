import random

# Wprowadzanie dlugosci hasła
while True:
    leng=input("Wpisz długość jaką ma mnieć twoje hasło: ")
        # Sprawdzanie czy podana wartość jest liczbą/cyfra
    if leng.isdigit():
        leng_num=int(leng)
        break
    else:
        print('Wprowadż wartość w postaci liczbowej')

while True:
    # Wprowadzanie ilosci wielkich liter w hasle
    while True:
        cap=input("Podaj ile wielkich liter chcesz w swoim hasle: ")
        # sprawdzenie czy podana wartosc jesy liczba/cyfra
        if cap.isdigit():
            cap_num=int(cap)
            break
        else:
            print('Wprowadż wartość w postaci liczbowej')

    # Wprowadzanie ilosci malych liter w hasle
    while True:
        low=input("Podaj ile malych liter chcesz w swoim hasle: ")
        # sprawdzenie czy podana wartosc jesy liczba/cyfra
        if low.isdigit():
            low_num=int(low)
            break
        else:
            print('Wprowadż wartość w postaci liczbowej')

    # Wprowadzanie ilosci cyfr w hasle
    while True:
        num=input("Podaj ile cyfr chcesz w swoim hasle: ")
        # sprawdzenie czy podana wartosc jesy liczba/cyfra
        if num.isdigit():
            num_num=int(num)
            break
        else:
            print('Wprowadż wartość w postaci liczbowej')

    # Wprowadzanie ilosci znakow specjalnych w hasle
    while True:
        spe=input("Podaj ile znakow specjalnych chcesz w swoim hasle: ")
        #sprawdzenie czy podana wartosc jesy liczba/cyfra
        if spe.isdigit():
            spe_num=int(spe)
            break
        else:
            print('Wprowadż wartość w postaci liczbowej')

    #sprawdzanie czy suma podanych wartosci odpowiada sumie podanej dlugosci
    sum=spe_num + num_num + cap_num + low_num

    if leng_num!=sum:
        print('suma podanych wartosci nie rowna sie podanej dlugosc')
    else:
        break


#tablica wielkich liter
cap_base=['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
#tablica malych liter
law_base=['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
#tablica cyfr
num_base=['1', '2', '3', '4', '5', '6', '7', '8', '9']
#tablica znakow specjanych
spe_base=['!','"','#','$','%','&','(',')','*','+',',','-','.','/',';',':','<','=','>','?','@','[',']','^','_','`','{','|','}','~']

#tablica w ktorej beda umiesczone wartosci do stworzenia hasla
pass_=[]

#dodawanie do tablicy wartosci
for i in range(cap_num):
    pass_ += random.choice(cap_base)
for i in range(low_num):
    pass_ += random.choice(law_base)
for i in range(num_num):
    pass_ += random.choice(num_base)
for i in range(spe_num):
    pass_ += random.choice(spe_base)

#zamienianie miejscami wartosci w tablicy
random.shuffle(pass_)

#tworzenie hasla
haslo = ''.join(pass_)

#Twoje hasło :)
print(f"Oto twoje wygenerowane hasło: {haslo}")
