
Lets split into three groups.

 
Group A: 1 2 3 4

Group B: 5 6 7 8

Group C: 9 10 11 12

Now we first weight A and B,

1. if A = B, then the defective ball must be in Group C. Now we weight {9, 10}, if 9 < 10, we weight {9, 11}, if 9 = 11, then ball 10 is the defective one. if 9 = 10,
then we weight 9 and 11, if 9 < 11 then the defective ball is 11, otherwise its 12.

2. if A < B, then the defective ball must be either in Group A or Group B. We weight {1, 2, 5} and {3, 6, 9}.
if {1, 2, 5} = {3, 6, 9}, then the defective ball must be in {4, 7, 8}. To find it, we weight {7, 8}. if 7 = 8, then 4 is the defective ball, otherwise the heavier one is
the defective ball. Now if {1, 2, 5} < {3, 6, 9}, then we weight {1, 2}, if 1 < 2 then 1 is the defective ball. otherwise if 1 = 2 then 6 is the defective ball.

The rest should be easy to deduce.
