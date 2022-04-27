# RPG

Create `Hero`, `Barbarian`, `Wizard`, `Hunter` and `Kobold` classes

### Hero
- every hero has `HitPoint` (never be lower than 0), `AttackNumber` and `DefenseNumber` props
- you can create default `Hero()` by default HP, `AttackNumber` and `DefenseNumber`, but you can also create `Hero(number)` with another number of HP, e. g. `Wizard(7)` starts with 7 HP
- every hero can `Attack()`, `DrinkPotion()` a `GetStatus()` method
- `Attack(enemy)` attacks the enemy (another `Hero` or `Kobold`) and lower enemy\`s `HitPoint` by hero\`s `AttackNumber` minus enemy\`s `DefenseNumber`
- `DrinkPotion()` heals 5 HP, maximum to max `HitPoint`
- `GetStatus()` print: `Hi, I am a barbarian/wizard/hunter with 10 HP` or `I am dead` (if there aren‘t any HP)

### Babarian
- starts with 20 HP, max. 30
- `AttackNumber` is 10
- `DefenseNumber` is 1

### Hunter
- starts with 15 HP, max. 20
- `AttackNumber` is 8, but attack against `Kobold` always kills the kobold (kobold’s HP to 0)
- `DefenseNumber` is 3

### Wizard
- starts with 10 HP, max. 15
- `AttackNumber` is 5
- `DefenseNumber` is 0
- `GetStatus()` is little different, prints: `Hi, I am a wizard with 10 HP and I can spell` or `I am ghost` (if there aren't any HP)
- `DrinkPotion()` is little different, heals to maximum HP
- wizard can `Spell(enemy, power)` which attacks the enemy, parameters are `enemy` and `power` (integer) - attacks the enemy (another `Hero` or `Kobold`) and lower enemy\`s `HitPoint` by spell `Power`

### Kobold
- starts with 15 HP, max. 15
- `AttackNumber` is 5
- `DefenseNumber` is 1
- every kobold can `Attack()` and `GetStatus()` method
- `Attack(hero)` attacks hero (not the kobold) and lowers hero\`s `HitPoint` by kobold\`s `AttackNumber` minus enemy\`s `DefenseNumber`
- `GetStatus()` print this: `Hi, I am a kobold with 10 HP` or `I am dead kobold` (if there aren‘t any HP)
<br>

![image](https://user-images.githubusercontent.com/99694929/165537552-f8963d83-25c2-4840-874d-bed327eb4420.png)
