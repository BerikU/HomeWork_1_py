1. Напишите программу, которая принимает на вход цифру, обозначающую день недели, и проверяет, является ли этот день выходным.

n = int(input())
if 5 < n < 8:
    print("Day-off")
elif 0 < n < 6:
    print("Working days")
else:
    print("Incorrect number")


 2. Напишите программу для проверки ложности утверждения  (W ⋀ Z) ⋁ ¬Y ⋁ (¬X ≡ ¬W) для всех значений предикат.

print("x, y, z, w")
for x in range(2):
    for y in range(2):
        for z in range(2):
            for w in range(2):
                if not ((w and z) or not y or (not x == (not w))):
                    print(x, y, z, w)

 3. Напишите программу, которая принимает на вход координаты точки (X и Y), причём X ≠ 0 и Y ≠ 0 и
выдаёт номер четверти плоскости, в которой находится эта точка (или на какой оси она находится).

x = int(input())
y = int(input())
if x > 0 and y > 0:
    print("1")
elif x < 0 and y > 0:
    print("2")
elif x <0 and y < 0:
    print("3")
elif x > 0 and y < 0:
    print("4")

4. Напишите программу, которая по заданному номеру четверти, показывает диапазон возможных координат точек в этой четверти (x и y).

n = int(input())
if n == 1:
    print("x and y > 0")
elif n == 2:
    print("x < 0, y > 0")
elif n == 3:
    print("x and y < 0")
elif n == 4:
    print("x > 0, y <0")
else:
    print("incorrect number")
    
5. Напишите программу, которая принимает на вход координаты двух точек и находит расстояние между ними в 2D пространстве.

x_1 = int(input())
y_1 = int(input())
x_2 = int(input())
y_2 = int(input())
print(f"{((x_2-x_1)**2+(y_2-y_1)**2)**0.5:0.4}")
