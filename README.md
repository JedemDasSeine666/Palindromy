def czyPalindrom(x): -#określenie definicji

    x = x.lower().replace(" ", "") #kalibracja znaków
    
    n = len(x) #zmienna z długością słowa
    
    for i in range(n-1): #zasięg funkcji
    
        if x[i] != x[n-1-i]: #sprawdzenie zgodności znaków od końca
        
            return False #zwroc false
            
    return True; #jezeli dane takie same = true 
    
print("Podaj slowo")

s1 = input() #wprowadzenie danych

print(bool("x") if(czyPalindrom(s1)) else bool("")) #zwrot wartości false lub true w funkcji bool
