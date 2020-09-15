X = float(input("hauteurt debut de marée :"))
Y = float(input("hautueur fin de marée :"))
D1 = int(input("heure debut de marée :"))
D2 = int(input("minute debut de marée :"))
F1 = int(input("heure fin de marée :"))
F2 = int(input("minute fin de marée :"))

D = D1 * 60 + D2
float(D)
F = F1 * 60 + F2
float(F)

H1 = int(input("heure souhaité:"))
H2 = int(input("minute souhaitée :"))


H = H1 * 60 + H2

if D < H < F:
    print("Ce nombre convient")
else:
    print("veuillez saisir une heure entre le debut et la fin de la marée")
t = H-D
float(t)
Du = F - D
float(Du)
ma = Y-X
float(ma)
Z = (90*t)/Du

import math
Z2 = math.radians(Z)
Z3 = math.sin(Z2)*math.sin(Z2)
delta_H = ma*Z3
Hauteur = X+delta_H
print(Hauteur)



