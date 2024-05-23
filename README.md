# KBC_game

















#game
questions = [
    ["what is the national game of India", "cricket", "baseball", "hockey", "football", "none", 3],
    ["who was the first PM of India", "narendra modi", "jawaharlal nehru", "br ambedkar", "rabindranath tagore", "none", 2],
    ["what is the oldest dam in India", "Hirakud dam", "farakka barage", "bhakra nangal dam", "somnath dam", "none", 1],
   ...more questions
]
levels = (1000, 2000, 3000, 5000, 10000, 20000, 40000, 80000, 160000, 320000)
money = 0
for i in range(0, len(questions)):
  question = questions[i]
  print(f"the question is on your screen for {levels[i]}")
  print(questions[i][0])
  print("the options ar on your screen now")
  print(f"a.{questions[i][1]}")
  print(f"b.{questions[i][2]}")
  print(f"c.{questions[i][3]}")
  print(f"d.{questions[i][4]}")
  reply = int(input("enter the option"))
  if (reply == questions[i][-1]):
    print(f"correct answer you won Rs.{levels[i]}")
    if(i==4):
      money=10000
    elif(i==9):
      money=320000
    elif(i==14):
      money=10000000
  else:
    print("wrong answer")
    break
