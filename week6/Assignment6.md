# Assignment 6: Rock Paper Scissors

### Question 1

In a classic schoolyard game, each player has three moves: rock, paper, and scissors, represented here as R, P, and S respectively. In this exercise, you will write a script that tries to predict the next move of an opponent using a rather naïve learning algorithm. The rules are simple: your script will predict the probability of each possible move based on the opponent’s previous four moves. For every possible sequence of four moves, you should maintain beliefs about the probability of every possible next move. To do this, use a dictionary in which the keys are four-move sequences, and the values are tuples representing the probability of an R, P, and S.

When a sequence of four moves appears for the first time, you should initialize your beliefs about the opponents next move to be (1/3, 1/3, 1/3). When you observe the opponent’s actual move, you should update your beliefs using a weighting factor, a. Multiply all three probabilities by (1 - a) then add a to the one corresponding to the opponent’s move. You should begin this learning process with the opponent’s fifth move and continue updating with every move after that.

For this exercise, use a value of a = 0.10.

According to this model, what is the most likely next move after the following sequences?

#### Sequence 1:

PSSPRPPPPSSRPRRPRSRSSRPPRSSSSSPSRSSRPSSSRPRPSSPRPP

Select one:
- a. R
- b. P
- c. S

#### Sequence 2:

RPSSPRRSRSPSPRPPPPSRSPPRRRSPSSRSSSSPPSSPRRSSRPRSPPSRSRPRRRSSSSPSRSPRSRRPPSR

Select one:
- a. R
- b. P
- c. S

#### Sequence 3:

SPPPPSRSPPPRSPRRSRPPSPRPSRRRSSRRPRRSPSPSPSRRRRSSSRPPSPRPSRSRPRSRPRSRRSPRPRRRSRRPSSRSRSRSPSSPRRRRRPRR

Select one:
- a. R
- b. P
- c. S

#### Sequence 4:

PPSRPPPSSPSPSRRSPRRPPRPRRPRRRSPPRPSPRRSRPRRSSRSPPPRRSSPRSPSPSRPPSSPSRRRRSSRPRRPPPRSPPSPRPRSPRPPSRRSRPPRSPRSSPPPRRRPSRPPSPSRSPRPPPRRPPPPSRRSPPSPPSPRPPP

Select one:
- a. R
- b. P
- c. S