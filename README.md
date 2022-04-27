# RPG

Create Hero, Barbarian, Wizard, Hunter and Kobold classes

Hero
- every hero has HitPoint (never be lower than 0), AttackNumber and DefenseNumber
- you can create default Hero() by default HP, AttackNumber and DefenseNumber, but you can also create Hero(number) with another number of HP, e. g. Wizard(7) starts with 7 HP
- every hero can Attack(), DrinkPotion() a GetStatus() method
- Attack(enemy) attacks the enemy (another Hero or Kobold) and lower enemy`s HitPoint by Hero`s AttackNumber minus enemy`s DefenseNumber
- DrinkPotion() heals 5 HP, maximum to max HitPoint
- GetStatus print this: „Hi, I am a barbarian/wizard/hunter with 10 HP“ or „I am dead“ (if there aren‘t any HP)

Babarian
- starts with 20 HP, max. 30
- AttackNumber = 10
- DefenseNumber = 1

Hunter
- starts with 15 HP, max. 20
- AttackNumber = 8, but attack to Cobold every time kill the kobold (kobold’s HP to 0)
- DefenseNumber = 3

Wizard
- starts with 10 HP, max. 15
- AttackNumber = 5
- DefenseNumber = 0
- GetStatus is little different, prints: „Hi, I am a wizard with 10 HP and I can spell“ or „I am ghost“ (if there arent any HP)
- DrinkPotion() is little different, heals to maximum HP
- wizrad can Spell(enemy, power) – it attack to enemy, parametres are enemy and power (integer) - attacks the enemy (another Hero or Kobold) and lower enemy`s HitPoint by spell Power

Kobold
- starts with 15 HP, max. 15
- AttackNumber = 5
- DefenseNumber = 1
- every Kobold can Attack() and GetStatus() method
- Attack(hero) attacks hero (not to Kobold) and lower hero`s HitPoint by Kobold`s AttackNumber minus enemy`s DefenseNumber
- GetStatus print this: „Hi, I am a kobold with 10 HP“ or „I am dead kobold“ (if there aren‘t any HP)
![image](https://user-images.githubusercontent.com/99694929/165537552-f8963d83-25c2-4840-874d-bed327eb4420.png)
