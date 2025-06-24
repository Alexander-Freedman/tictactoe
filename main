<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Tic Tac Toe Game</title>
    <!-- PyScript CSS and JS -->
    <link rel="stylesheet" href="https://pyscript.net/latest/pyscript.css">
    <script defer src="https://pyscript.net/latest/pyscript.js"></script>
</head>
<body style="font-family: Arial, sans-serif; text-align:center; padding-top:20px;">
    <h1>Tic Tac Toe Bot</h1>
    <py-terminal></py-terminal>

    <py-script>
        # Place your Python code directly here:
        
        # (Copy your entire Python code here exactly as provided)
        
        # For brevity, here is an example start and end:
        
        

      # Welcome Message
print("Welcome to the Tic Tac Toe Bot. \n You will never win. \n Feel free to give it a shot anyways.")
name=input("What's your name?\n")
if name==("abs"):
  a1,a2,a3,b1,b2,b3,c1,c2,c3="X", "X", "X", "X", "X", "X", "X", "X", "X"
  print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
  print("You Win!")
  exit()

# Defining Spots
corner_spots=["a1","c1","a3","c3"]
edge_spots=["b1","a2","c2","b3"]
m_spot=["b2"]
all_spots=["a1","b1","c1","a2","b2","c2","a3","b3","c3"]
a1,a2,a3="-","-","-"
b1,b2,b3="-","-","-"
c1,c2,c3="-","-","-"
pm1,pm2,pm3,pm4,pm5,cm1,cm2,cm3,cm4,cm5=0,0,0,0,0,0,0,0,0,0
game="over"


# Rules
print("Use the letters and numbers on the board to key in your spot.\n For example for the top right corner respond with \"c1\".")


print("You're going first and you're \"X\".")
print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")

while pm1 not in all_spots:
    pm1=input("Please make your first move "+name+".\n")
    if pm1 not in all_spots:
        print("Value not reconized, Please try again.")
all_spots.remove(pm1)
if pm1 in corner_spots:
    corner_spots.remove(pm1)
    if pm1 == "a1":
        a1="X"
    elif pm1 == "c1":
        c1="X"
    elif pm1 == "a3":
        a3="X"
    elif pm1 == "c3":
        c3="X"
    b2="O"                               # COMPUTER TURN ---------------------------------------
    all_spots.remove("b2")                 # COMPUTER TURN ---------------------------------------
    m_spot.remove("b2")                    # COMPUTER TURN ---------------------------------------
elif pm1 in edge_spots:
        edge_spots.remove(pm1)
        if pm1 == "b1":
            b1="X"
        elif pm1 == "a2":
            a2="X"
        elif pm1 == "c2":
            c2="X"
        elif pm1 == "b3":
            b3="X"
        if pm1 == "b1" or pm1 == "a2":
            a1="O"                           # COMPUTER TURN ---------------------------------------
            all_spots.remove("a1")             # COMPUTER TURN ---------------------------------------
            corner_spots.remove("a1")          # COMPUTER TURN ---------------------------------------
        elif pm1 == "c2" or pm1 == "b3":
            c3="O"                           # COMPUTER TURN ---------------------------------------
            all_spots.remove("c3")             # COMPUTER TURN ---------------------------------------
            corner_spots.remove("c3")          # COMPUTER TURN ---------------------------------------
elif pm1 in m_spot:
    m_spot.remove(pm1)
    if pm1 == "b2":
        b2="X"
        c3="O"                           # COMPUTER TURN ---------------------------------------
        all_spots.remove("c3")             # COMPUTER TURN ---------------------------------------
        corner_spots.remove("c3")          # COMPUTER TURN ---------------------------------------

print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
while pm2 not in all_spots:
    pm2=input("Please make your second move "+name+".\n")
    if pm2 not in all_spots:
        print("Value not reconized, Please try again.")
    
all_spots.remove(pm2)

if pm2 in corner_spots:
    corner_spots.remove(pm2)
    if pm2 == "a1":
        a1="X"
    elif pm2 == "c1":
        c1="X"
    elif pm2 == "a3":
        a3="X"
    elif pm2 == "c3":
        c3="X" 
elif pm2 in edge_spots:
    edge_spots.remove(pm2)
    if pm2 == "b1":
        b1="X"
    elif pm2 == "a2":
        a2="X"
    elif pm2 == "c2":
        c2="X"
    elif pm2 == "b3":
        b3="X"
elif pm2 in m_spot:
    m_spot.remove(pm2)
    if pm2 == "b2":
        b2="X"

if a1 == "X" and a2 == "X":
    a3="O"
elif a1 == "X" and a3 == "X":
    a2="O"
elif a2 == "X" and a3 == "X":
    a1="O"

elif b1 == "X" and b2 == "X":
    b3="O"
elif b1 == "X" and b3 == "X":
    b2="O"
elif b2 == "X" and b3 == "X":
    b1="O"

elif c1 == "X" and c2 == "X":
    c3="O"
elif c1 == "X" and c3 == "X":
    c2="O"
elif c2 == "X" and c3 == "X":
    c1="O"

elif a1 == "X" and b1 == "X":
    c1="O"
elif a1 == "X" and c1 == "X":
    b1="O"
elif b1 == "X" and c1 == "X":
    a1="O"

elif a2 == "X" and b2 == "X":
    c2="O"
elif a2 == "X" and c2 == "X":
    b2="O"
elif b2 == "X" and c2 == "X":
    a2="O"

elif a3 == "X" and b3 == "X":
    c3="O"
elif a3 == "X" and c3 == "X":
    b3="O"
elif b3 == "X" and c3 == "X":
    a3="O"

elif a1 == "X" and b2 == "X":
    c3="O"
elif a1 == "X" and c3 == "X":
    b2="O"
elif b2 == "X" and c3 == "X":
    a1="O"

elif c1 == "X" and b2 == "X":
    a3="O"
elif c1 == "X" and a3 == "X":
    b2="O"
elif b2 == "X" and a3 == "X":
    c1="O"


if a1 == "O" and "a1" in all_spots:
    all_spots.remove("a1")
elif b1 == "O" and "b1" in all_spots:
    all_spots.remove("b1")
elif c1 == "O" and "c1" in all_spots:
    all_spots.remove("c1")
elif a2 == "O" and "a2" in all_spots:
    all_spots.remove("a2")
elif b2 == "O" and "b2" in all_spots:
    all_spots.remove("b2")
elif c2 == "O" and "c2" in all_spots:
    all_spots.remove("c2")
elif a3 == "O" and "a3" in all_spots:
    all_spots.remove("a3")
elif b3 == "O" and "b3" in all_spots:
    all_spots.remove("b3")
elif c3 == "O" and "c3" in all_spots:
    all_spots.remove("c3")
else:
    if "b1" in all_spots:
        b1="O"
        all_spots.remove("b1")
    elif "a2" in all_spots:
        a2="O"
        all_spots.remove("a2")
    elif "c2" in all_spots:
        c2="O"
        all_spots.remove("c2")
    elif "b3" in all_spots:
        b3="O"
        all_spots.remove("b3")


print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")

while pm3 not in all_spots:
    pm3=input("Please make your third move "+name+".\n")
    if pm3 not in all_spots:
        print("Value not reconized, Please try again.")
    
all_spots.remove(pm3)


if pm3 in corner_spots:
    corner_spots.remove(pm3)
    if pm3 == "a1":
        a1="X"
    elif pm3 == "c1":
        c1="X"
    elif pm3 == "a3":
        a3="X"
        c3="X"
elif pm3 in edge_spots:
    edge_spots.remove(pm3)
    if pm3 == "b1":
        b1="X"
    elif pm3 == "a2":
        a2="X"
    elif pm3 == "c2":
        c2="X"
    elif pm3 == "b3":
        b3="X"
elif pm3 in m_spot:
    m_spot.remove(pm2)
    if pm3 == "b2":
        b2="X"



if a1 == "O" and a2 == "O" and a3 !="X":
    a3="O"
elif a1 == "O" and a3 == "O" and a2 !="X":
    a2="O"
elif a2 == "O" and a3 == "O" and a1 !="X":
    a1="O"

elif b1 == "O" and b2 == "O" and b3 !="X":
    b3="O"
elif b1 == "O" and b3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and b3 == "O" and b1 !="X":
    b1="O"

elif c1 == "O" and c2 == "O" and c3 !="X":
    c3="O"
elif c1 == "O" and c3 == "O" and c2 !="X":
    c2="O"
elif c2 == "O" and c3 == "O" and c1 !="X":
    c1="O"

elif a1 == "O" and b1 == "O" and c1 !="X":
    c1="O"
elif a1 == "O" and c1 == "O" and b1 !="X":
    b1="O"
elif b1 == "O" and c1 == "O" and a1 !="X":
    a1="O"

elif a2 == "O" and b2 == "O" and c2 !="X":
    c2="O"
elif a2 == "O" and c2 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and c2 == "O" and a2 !="X":
    a2="O"

elif a3 == "O" and b3 == "O" and c3 !="X":
    c3="O"
elif a3 == "O" and c3 == "O" and b3 !="X":
    b3="O"
elif b3 == "O" and c3 == "O" and a3 !="X":
    a3="O"

elif a1 == "O" and b2 == "O" and c3 !="X":
    c3="O"
elif a1 == "O" and c3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and c3 == "O" and a1 !="X":
    a1="O"

elif c1 == "O" and b2 == "O" and a3 !="X":
    a3="O"
elif c1 == "O" and a3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and a3 == "O" and c1 !="X":
    c1="O"
else:
    if a1 == "X" and a2 == "X":
        a3="O"
    elif a1 == "X" and a3 == "X":
        a2="O"
    elif a2 == "X" and a3 == "X":
        a1="O"

    if b1 == "X" and b2 == "X":
        b3="O"
    elif b1 == "X" and b3 == "X":
        b2="O"
    elif b2 == "X" and b3 == "X":
        b1="O"

    if c1 == "X" and c2 == "X":
        c3="O"
    elif c1 == "X" and c3 == "X":
        c2="O"
    elif c2 == "X" and c3 == "X":
        c1="O"

    if a1 == "X" and b1 == "X":
        c1="O"
    elif a1 == "X" and c1 == "X":
        b1="O"
    elif b1 == "X" and c1 == "X":
        a1="O"

    if a2 == "X" and b2 == "X": 
        c2="O"
    elif a2 == "X" and c2 == "X":
        b2="O"
    elif b2 == "X" and c2 == "X":   
        a2="O"

    if a3 == "X" and b3 == "X": 
        c3="O"
    elif a3 == "X" and c3 == "X":   
        b3="O"
    elif b3 == "X" and c3 == "X":   
        a3="O"

    if a1 == "X" and b2 == "X": 
        c3="O"
    elif a1 == "X" and c3 == "X":   
        b2="O"
    elif b2 == "X" and c3 == "X":   
        a1="O"

    if c1 == "X" and b2 == "X": 
        a3="O"
    elif c1 == "X" and a3 == "X":   
        b2="O"
    elif b2 == "X" and a3 == "X":   
        c1="O"

    if a1 == "O" and "a1" in all_spots:
        all_spots.remove("a1")
    elif b1 == "O" and "b1" in all_spots:
        all_spots.remove("b1")
    elif c1 == "O" and "c1" in all_spots:
        all_spots.remove("c1")
    elif a2 == "O" and "a2" in all_spots:
        all_spots.remove("a2")
    elif b2 == "O" and "b2" in all_spots:
        all_spots.remove("b2")
    elif c2 == "O" and "c2" in all_spots:
        all_spots.remove("c2")
    elif a3 == "O" and "a3" in all_spots:
        all_spots.remove("a3")
    elif b3 == "O" and "b3" in all_spots:
        all_spots.remove("b3")
    elif c3 == "O" and "c3" in all_spots:
        all_spots.remove("c3")
    else:
        if "b1" in all_spots:
            b1="O"
            all_spots.remove("b1")
        elif "a2" in all_spots:
            a2="O"
            all_spots.remove("a2")
        elif "c2" in all_spots:
            c2="O"
            all_spots.remove("c2")
        elif "b3" in all_spots:
            b3="O"
            all_spots.remove("b3")
    game="running"
if game=="over":
    print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
    print("I win, you lose.")
    exit()
    

game="over"
print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
while pm4 not in all_spots:
    pm4=input("Please make your fourth move "+name+".\n")
    if pm4 not in all_spots:
        print("Value not reconized, Please try again.")

all_spots.remove(pm4)

if pm4 in corner_spots:
    corner_spots.remove(pm4)
    if pm4 == "a1":
        a1="X"
    elif pm4 == "c1":
        c1="X"
    elif pm4 == "a3":
        a3="X"
    elif pm4 == "c3":
        c3="X"
elif pm4 in edge_spots:
    edge_spots.remove(pm4)
    if pm4 == "b1":
        b1="X"
    elif pm4 == "a2":
        a2="X"
    elif pm4 == "c2":
        c2="X"
    elif pm4 == "b3":
        b3="X"
elif pm4 in m_spot:
    m_spot.remove(pm4)
    if pm4 == "b2":
        b2="X"


if a1 == "O" and a2 == "O" and a3 !="X":
    a3="O"
elif a1 == "O" and a3 == "O" and a2 !="X":
    a2="O"
elif a2 == "O" and a3 == "O" and a1 !="X":
    a1="O"

elif b1 == "O" and b2 == "O" and b3 !="X":
    b3="O"
elif b1 == "O" and b3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and b3 == "O" and b1 !="X":
    b1="O"

elif c1 == "O" and c2 == "O" and c3 !="X":
    c3="O"
elif c1 == "O" and c3 == "O" and c2 !="X":
    c2="O"
elif c2 == "O" and c3 == "O" and c1 !="X":
    c1="O"

elif a1 == "O" and b1 == "O" and c1 !="X":
    c1="O"
elif a1 == "O" and c1 == "O" and b1 !="X":
    b1="O"
elif b1 == "O" and c1 == "O" and a1 !="X":
    a1="O"

elif a2 == "O" and b2 == "O" and c2 !="X":
    c2="O"
elif a2 == "O" and c2 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and c2 == "O" and a2 !="X":
    a2="O"

elif a3 == "O" and b3 == "O" and c3 !="X":
    c3="O"
elif a3 == "O" and c3 == "O" and b3 !="X":
    b3="O"
elif b3 == "O" and c3 == "O" and a3 !="X":
    a3="O"

elif a1 == "O" and b2 == "O" and c3 !="X":
    c3="O"
elif a1 == "O" and c3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and c3 == "O" and a1 !="X":
    a1="O"

elif c1 == "O" and b2 == "O" and a3 !="X":
    a3="O"
elif c1 == "O" and a3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and a3 == "O" and c1 !="X":
    c1="O"
else:
    if a1 == "X" and a2 == "X":
        a3="O"
    elif a1 == "X" and a3 == "X":
        a2="O"
    elif a2 == "X" and a3 == "X":
        a1="O"

    if b1 == "X" and b2 == "X":
        b3="O"
    elif b1 == "X" and b3 == "X":
        b2="O"
    elif b2 == "X" and b3 == "X":
        b1="O"

    if c1 == "X" and c2 == "X":
        c3="O"
    elif c1 == "X" and c3 == "X":
        c2="O"
    elif c2 == "X" and c3 == "X":
        c1="O"

    if a1 == "X" and b1 == "X":
        c1="O"
    elif a1 == "X" and c1 == "X":
        b1="O"
    elif b1 == "X" and c1 == "X":
        a1="O"

    if a2 == "X" and b2 == "X": 
        c2="O"
    elif a2 == "X" and c2 == "X":
        b2="O"
    elif b2 == "X" and c2 == "X":   
        a2="O"

    if a3 == "X" and b3 == "X": 
        c3="O"
    elif a3 == "X" and c3 == "X":   
        b3="O"
    elif b3 == "X" and c3 == "X":   
        a3="O"

    if a1 == "X" and b2 == "X": 
        c3="O"
    elif a1 == "X" and c3 == "X":   
        b2="O"
    elif b2 == "X" and c3 == "X":   
        a1="O"

    if c1 == "X" and b2 == "X": 
        a3="O"
    elif c1 == "X" and a3 == "X":   
        b2="O"
    elif b2 == "X" and a3 == "X":   
        c1="O"

    if a1 == "O" and "a1" in all_spots:
        all_spots.remove("a1")
    elif b1 == "O" and "b1" in all_spots:
        all_spots.remove("b1")
    elif c1 == "O" and "c1" in all_spots:
        all_spots.remove("c1")
    elif a2 == "O" and "a2" in all_spots:
        all_spots.remove("a2")
    elif b2 == "O" and "b2" in all_spots:
        all_spots.remove("b2")
    elif c2 == "O" and "c2" in all_spots:
        all_spots.remove("c2")
    elif a3 == "O" and "a3" in all_spots:
        all_spots.remove("a3")
    elif b3 == "O" and "b3" in all_spots:
        all_spots.remove("b3")
    elif c3 == "O" and "c3" in all_spots:
        all_spots.remove("c3")
    else:
        if "b1" in all_spots:
            b1="O"
            all_spots.remove("b1")
        elif "a2" in all_spots:
            a2="O"
            all_spots.remove("a2")
        elif "c2" in all_spots:
            c2="O"
            all_spots.remove("c2")
        elif "b3" in all_spots:
            b3="O"
            all_spots.remove("b3")
    game="running"
if game=="over":
    print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
    print("I win, you lose.")
    exit()
    

game="over"
print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
while pm5 not in all_spots:
    pm5=input("Please make your last move "+name+".\n")
    if pm5 not in all_spots:
        print("Value not reconized, Please try again.")
    
all_spots.remove(pm5)

if pm5 in corner_spots:
    corner_spots.remove(pm5)
    if pm5 == "a1":
        a1="X"
    elif pm5 == "c1":
        c1="X"
    elif pm5 == "a3":
        a3="X"
    elif pm5 == "c3":
        c3="X"
elif pm5 in edge_spots:
    edge_spots.remove(pm5)
    if pm5 == "b1":
        b1="X"
    elif pm5 == "a2":
        a2="X"
    elif pm5 == "c2":
        c2="X"
    elif pm5 == "b3":
        b3="X"
elif pm5 in m_spot:
    m_spot.remove(pm5)
    if pm5 == "b2":
        b2="X"


if a1 == "O" and a2 == "O" and a3 !="X":
    a3="O"
elif a1 == "O" and a3 == "O" and a2 !="X":
    a2="O"
elif a2 == "O" and a3 == "O" and a1 !="X":
    a1="O"

elif b1 == "O" and b2 == "O" and b3 !="X":
    b3="O"
elif b1 == "O" and b3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and b3 == "O" and b1 !="X":
    b1="O"

elif c1 == "O" and c2 == "O" and c3 !="X":
    c3="O"
elif c1 == "O" and c3 == "O" and c2 !="X":
    c2="O"
elif c2 == "O" and c3 == "O" and c1 !="X":
    c1="O"

elif a1 == "O" and b1 == "O" and c1 !="X":
    c1="O"
elif a1 == "O" and c1 == "O" and b1 !="X":
    b1="O"
elif b1 == "O" and c1 == "O" and a1 !="X":
    a1="O"

elif a2 == "O" and b2 == "O" and c2 !="X":
    c2="O"
elif a2 == "O" and c2 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and c2 == "O" and a2 !="X":
    a2="O"

elif a3 == "O" and b3 == "O" and c3 !="X":
    c3="O"
elif a3 == "O" and c3 == "O" and b3 !="X":
    b3="O"
elif b3 == "O" and c3 == "O" and a3 !="X":
    a3="O"

elif a1 == "O" and b2 == "O" and c3 !="X":
    c3="O"
elif a1 == "O" and c3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and c3 == "O" and a1 !="X":
    a1="O"

elif c1 == "O" and b2 == "O" and a3 !="X":
    a3="O"
elif c1 == "O" and a3 == "O" and b2 !="X":
    b2="O"
elif b2 == "O" and a3 == "O" and c1 !="X":
    c1="O"
else:
    if a1 == "X" and a2 == "X":
        a3="O"
    elif a1 == "X" and a3 == "X":
        a2="O"
    elif a2 == "X" and a3 == "X":
        a1="O"

    elif b1 == "X" and b2 == "X":
        b3="O"
    elif b1 == "X" and b3 == "X":
        b2="O"
    elif b2 == "X" and b3 == "X":
        b1="O"

    elif c1 == "X" and c2 == "X":
        c3="O"
    elif c1 == "X" and c3 == "X":
        c2="O"
    elif c2 == "X" and c3 == "X":
        c1="O"

    elif a1 == "X" and b1 == "X":
        c1="O"
    elif a1 == "X" and c1 == "X":
        b1="O"
    elif b1 == "X" and c1 == "X":
        a1="O"

    elif a2 == "X" and b2 == "X": 
        c2="O"
    elif a2 == "X" and c2 == "X":
        b2="O"
    elif b2 == "X" and c2 == "X":   
        a2="O"

    elif a3 == "X" and b3 == "X": 
        c3="O"
    elif a3 == "X" and c3 == "X":   
        b3="O"
    elif b3 == "X" and c3 == "X":   
        a3="O"

    elif a1 == "X" and b2 == "X": 
        c3="O"
    elif a1 == "X" and c3 == "X":   
        b2="O"
    elif b2 == "X" and c3 == "X":   
        a1="O"

    elif c1 == "X" and b2 == "X": 
        a3="O"
    elif c1 == "X" and a3 == "X":   
        b2="O"
    elif b2 == "X" and a3 == "X":   
        c1="O"

    if a1 == "O" and "a1" in all_spots:
        all_spots.remove("a1")
    elif b1 == "O" and "b1" in all_spots:
        all_spots.remove("b1")
    elif c1 == "O" and "c1" in all_spots:
        all_spots.remove("c1")
    elif a2 == "O" and "a2" in all_spots:
        all_spots.remove("a2")
    elif b2 == "O" and "b2" in all_spots:
        all_spots.remove("b2")
    elif c2 == "O" and "c2" in all_spots:
        all_spots.remove("c2")
    elif a3 == "O" and "a3" in all_spots:
        all_spots.remove("a3")
    elif b3 == "O" and "b3" in all_spots:
        all_spots.remove("b3")
    elif c3 == "O" and "c3" in all_spots:
        all_spots.remove("c3")
    else:
        if "b1" in all_spots:
            b1="O"
            all_spots.remove("b1")
        elif "a2" in all_spots:
            a2="O"
            all_spots.remove("a2")
        elif "c2" in all_spots:
            c2="O"
            all_spots.remove("c2")
        elif "b3" in all_spots:
            b3="O"
            all_spots.remove("b3")
    game="running"
if game=="over":
    print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
    print("I win, you lose.")
    exit()
        
game="over"
print("\n\n   a     b     c\n      |     |     \n1  "+a1+"  |  "+b1+"  |  "+c1+"  \n _____|_____|_____\n      |     |     \n2  "+a2+"  |  "+b2+"  |  "+c2+"  \n _____|_____|_____\n      |     |     \n3  "+a3+"  |  "+b3+"  |  "+c3+"  \n      |     |     ")
print("Tie.")

    </py-script>
</body>
</html>
