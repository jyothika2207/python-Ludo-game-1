# python-Ludo-game-1

def player_A(n):
    if n<=0:
        print("Player A reached 0!! player A loses ")
        return
    move =int(input("player A,subtract 1 or 2:"))
    while move not in[1,2]:
         move=int(input("Player A,subtract 1 or 2"))
    player_B(n-move)
def player_B (n):
     if n<=0:
        print("Player B reached 0!! player B loses ")
        return
     print(f"\n player B's turn.current number{n}")
     move =int(input("player A,subtract 1 or 2:"))
     while move not in[1,2]:
        move=int(input("Player A,subtract 1 or 2"))
     player_A(n-move)
start=int(input("enter the starting number:"))
player_A(start)

======OUTPUT=========
enter the starting number: 5
player A,subtract 1 or 2: 1

 player B's turn.current number4
player A,subtract 1 or 2: 1
player A,subtract 1 or 2: 1

 player B's turn.current number2
player A,subtract 1 or 2: 2
Player A reached 0!! player A loses 

Click to add a cell.
