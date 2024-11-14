import math

a = float(input("Nhập hệ số a: "))

b = float(input("Nhập hệ số b: "))

c = float(input("Nhập hệ số c: "))
if a == 0: 
    print("Phương trình là bậc nhất (ax + b = 0) hoặc không hợp lệ") 
else:
    delta = b**2 - 4*a*c

    if delta > 0: 
          x1 = (-b + math.sqrt(delta)) / (2*a) 
          x2 = (-b - math.sqrt(delta)) / (2*a) 
          print (f"Phuong trình có hai nghiệm phân biệt: x1 = {x1} và x2 = {x2}")

    elif delta == 0:
          x = b / (2*a)
          print(f"Phương trình có nghiệm kép: x = {x}") 
    else: 
          print("Phương trình vô nghiệm")
