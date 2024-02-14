j = "oguelva@123"
a = b = c = d = False

if len(j) < 8:
    print("fail")
else:
    x = list(j)
    print(x)
    for i in x:
        print(ord(i))
        if (ord(i) >= ord("a")) and (ord(i) <= ord("z")):
            print("small:",i)
            a = True
        elif (ord(i) >= ord("A")) and (ord(i) <= ord("Z")):
            print("Capital:",i)
            b = True
        elif (ord(i) >= ord("0")) and (ord(i) <= ord("9")):
            print("Numbers:",i)
            c = True
        else:
            print("Symbols:",i)
            d = True

if a == b == c == d == True:
    print("PASS")
else:
    print("Fail")
