# MDP REPRESENTATION

## AIM:
The aim of this MDP is to model the decision-making process of a person while coding, considering two levels of concentration - full concentration and half concentration, and to maximize productivity

## PROBLEM STATEMENT:

### Problem Description

#### In this scenario ,The team wants to win the football tournament,they has two choice,one is move right and reach the final win the cupand another one is move left ,get knocked from tournament.

### State Space

Knocked out ,Semi's ,Final.

### Sample State
Semi's.

### Action Space

Right , Left

### Sample Action

Right(1) and Left(0).

### Reward Function

Right= 1,Left= 0

### Graphical Representation

![307220710-bcf2e24b-b3c6-4108-8f95-ffd7830c5005](https://github.com/user-attachments/assets/e3881428-c956-4b83-af1f-ab033fb345cb)



## PYTHON REPRESENTATION:
```
mdp = {
    "Final": {
         0 : [(0.7, "Semi's", 0, False),(0.3, "Final", 1, True)],
        1 : [(0.8, "Final", 1, True),(0.2, "Semi's", 0, False)]
    },
    "Semi's": {
        0 : [(0.8, "Knocked out", 0, False),(0.2, "Semi's", 0, False)],
        1 : [(0.9, "Final", 1, True),(0.1, "Semi's", 0, False)]
    },
    "Knocked out": {
        0 : [(0.8, "Knocked out", 0, False),(0.2, "Semi's", 0, False)],
        1 : [(0.7, "Semi's`", 0, False),(0.3, "Knocked out", 0.0, False)]
    }
}
```

## OUTPUT
![307220327-4d6cc091-559e-4cbd-8210-f217ed484f85](https://github.com/user-attachments/assets/ac32409d-345d-479a-94e5-9610f1e74709)
:


## RESULT:
The result of solving this MDP would be an optimal policy that tells the person which action to take in each state to maximize their productivity while coding.

