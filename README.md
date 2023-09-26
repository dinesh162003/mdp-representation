# MDP REPRESENTATION

## AIM:
To create an environment to check whether the child plays or stay at home according to the weather conditions.

## PROBLEM STATEMENT:

### Problem Description
Children looking for playing outdoor games. Action is based on the weather conditions, if it is a sunny day there is a high chance of playing or if it is a cloudy day, they simply stay at home.

### State Space
{C,W,S} -> {0,1,2}
where,
C-cloudy, W-weather, S-sunny

### Sample State
Sunny

### Action Space
{play, stay}

### Sample Action
play

### Reward Function
1: happy if they play
0: pale if they stay

### Graphical Representation
![image](https://github.com/Kavya-Bollineni22/mdp-representation/assets/75235813/c40558a6-6c62-4bb9-bfac-7f5a53b11408)

## PYTHON REPRESENTATION:
```
MDP = {
    "S": {
         0 : [(0.7, "W", 0, False),(0.3, "S", 1, True)],
        1 : [(0.8, "S", 1, True),(0.2, "W", 0, False)]
    },
    "W": {
        0 : [(0.8, "C", 0, False),(0.2, "W", 0, False)],
        1 : [(0.9, "S", 1, True),(0.1, "W", 0, False)]
    },
    "C": {
         0 : [(0.8, "C", 0, False),(0.2, "W", 0, False)],
        1 : [(0.7, "W", 0, False),(0.3, "C", 0.0, False)]
    }
}
```

## OUTPUT:
![image](https://github.com/Kavya-Bollineni22/mdp-representation/assets/75235813/7d3f8d2c-ebf0-4273-a8d0-dbe22e7aa4d6)

## RESULT:
Thus, an environment to check whether the child plays or stay at home is created according to the weather conditions.
