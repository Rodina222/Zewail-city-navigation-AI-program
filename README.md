# Zewail-city-navigation-AI-program

Problem Formulation:
Initial State: 

Main Gate (location of the agent) with the location of the 4 items at Helmy building and 4 items at Nano building.

Goal State: 

All items delivered to the right delivery locations[ 4 items in AB and 4 items in one stop].

State: 

CrossRoad, 
State of the agent (whether the agent is carrying an item or not)-> It is boolean : if the agent carries an item then it is true but if it doesn’t carry any item then it is false.
The number of items in each building of the 4 buildings. [HB, AB, OSB,NB]

Actions: 

Depending on the agent’s state -> if the agent is in a state in which he should carry an item or drop it, then he will choose it immediately but if he is in any other state then he will choose a road from the available roads that the action function returns.

Rewards:

Positive: 

The agent takes the maximum positive reward if it terminates at one of two goals states before the limit ends which are:

Terminating at the academic building, not carrying an item and the number of items 
in both NB and HB are 0’s and the number of items in both OSB and AB are 0’s : ('AB', False, 0, 0, 4, 4).

        -  Terminating at a one-stop shop, not carrying an item and  
the number of Items in both NB and HB are 0’s and the number of items in both OSB and AB are 0’s : ('OSB', False, 0, 0, 4, 4).

The agent takes a constant positive reward if he takes the action ‘carry’ or ‘drop’.

Negative: 

The agent takes the maximum negative reward (penalty) when it terminates as the limit ends without reaching a goal state.

The agent takes a constant negative reward during moving along the map so that the agent tries to minimize its steps.
