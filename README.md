# Numbers_To_Roman

while True:
    def roman(x):
        n=[1,4,5,9,10,40,50,90,100,400,500,900,1000]
        r=["I","IV","V","IX","X","XL","L","XC","C","CD","D","CM","M"]
        i=12
        roman=""
        while x!=0:
            if n[i]<=x:
                roman+=r[i]
                x=x-n[i]
            else:
                i-=1
        return roman
    x=int(input(">"))
    print(roman(x))
