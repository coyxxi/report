# Report Project
# 숫자 맞추기 게임

import random

count = 0

print('게임하자. 컴퓨터인 내가 생각하는 수를 6번 안에 맞추면 돼. 준비됐으면 Enter를 쳐.')
input()

goal = random.randint(1, 100)
print('좋아. 숫자를 정했으니 한번 맞춰봐.')

while count < 6 :
    guess = input('당신이 예상하는 숫자는?')
    guess = int(guess)

    count += 1

    if guess == goal:
        break
    elif guess > goal:
        print('더 작은 수야..')
        goal = str(goal)
        print('이런.. 내가 생각하는 숫자는 ' + goal + '인데..')
        
print ('프로그램 종료')
