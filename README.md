# Stone-pape
n = int(input("Enter no of rounds:"))
user_wins=0
computer_wins=0
for i in range(n) :
  player= input("player 1(stone/paper/scissor):").lower()
  computer=input("player 2(stone/paper/scissor):").lower()
  if player == computer:
    print("draw")
    draw+=1
  elif (player == "stone" and computer == "scissor") or \
       (player == "paper" and computer == "stone") or \
       (player == "scissor" and computer == "paper"):
       print("player 1 wins")
       user_wins+=1
  else:
    print("player 2 wins")
    computer_wins+=1
  print("draw:",draw)
  print("player 1 wins:",user_wins)
  print("player 2 wins:",computer_wins)
