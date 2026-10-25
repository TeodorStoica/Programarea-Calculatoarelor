# Programarea-Calculatoarelor
Seminar

ore=int(input())
brut=0
net=0
impozit=0
if ore<=40:
    brut=15*ore
else:
    brut=15*40+(ore-40)*22.5
impozit=10/100*brut
if brut>400 and brut<=600:
    impozit=(brut-400)*18/100+impozit
if brut>600:
    impozit=(brut-600)*25/100+200*18/100+impozit
net=brut-impozit
print(brut)
print(impozit)
print(net)
--------------------------------------------------------
k=0
st=0
for i in range(1, 8):
    p=int(input("pret="))
    c=int(input("cantitate="))
    print("Valoare produs", i,"este: ", p*c)
    st=st+p*c
    if p*c>500:
        k+=1
print(st, k)
----------------------------------------------------------
s=0
b=0
for i in range(0, 7):
    a=int(input())
    s+=a
    if a>5000 and a<8000:
       b=b+5/100*a 
    elif a>=8000:
        b=b+5/100*a
print("vanzari:", s)
print("bonus:", b)
print(s+b)
_________________________________________________________
n=0
a=int
s=0
while a!=0:
    a=int(input())
    n+=1
    s+=a
m=s/n
print("nr comenzi:", n)
print("valoarea comenzilor este", s)
print("valoare medie:", m)
