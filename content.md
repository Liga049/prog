## Izveidot number guessing spēli ar Python prog valodu

### Saturs

#### 1. Aprakstit spēli
#### 2. Spēles loģika

Dators nejauši ģenerē vienu skaitli no 1 līz 100. Tālāk, piedāvā spēlētājam uzminēt to skaitli

Spēles loģika ir labi aprakstīta šajā koda

```py
import random

repeat = True

while repeat:
    number = random.randint(1, 100)
    guess = 0
    tries = 0

    while guess != number:
        if guess < number:
            print("pamēģini lielāku skaitli")
        else:
            print ("Pamēģini mazāku skaitli")

        guess = int(input("Uzmini skaitli: "))
        tries +=1
    else:
        if tries < 3:
            print(f"WOW, Tu uzminēji tikai pēc {tries} reizēm!")
        elif tries < 6:
            print(f"nav slikti, uzminēji pēc {tries} reizēm")
        else:
            print(f"mini labāk, uzminēji pēc {tries} reizēm")

    response = input("Vai tu gribi turpināt? y/n: ") 
    if response == "y":
        repeat = True 
    elif response =="n":
        repeat = False
        print("Paldies par spēli! bye bye")
    else:
        repeat = False
        print("Paldies par spēli! bye bye")
```
#### 3. un t.t



