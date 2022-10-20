Solution:

let f(n) be the distribution of gold for n pirates.

Clearly, f(1) = {100}

Then we can tell f(2) = {0, 100}, why? Because the second pirate can always win no matter what he proposes as he is the 50%.

What about f(3)? 
Observation 1: Pirate 2 would disagree with whatever pirate 3 proposes. Since if he can get rid of pirate 3, 
then the situation changes to f(2) and he can get all of the gold.

Observation 2: As long as you give something to pirate 1, he is going to agree with whatever proposal pirate 3 makes.
This is because pirate 2 would disagree (observation 1), and pirate 1 would get 0 gold from case f(2), therefore the best 
distribution pirate 3 can propose is to give pirate 1 one gold, and take 99 gold. Then pirate 1 and pirate 3 can have 66% vote.

Therefore, f(3) = {1, 0, 99}

Following this method, we can see f(4) = {0, 1, 0, 99} as pirate 2 doesnt want f(4)->f(3).

So we will have f(5) = {1, 0, 1, 0, 98} as pirate 1 and pirate 3 doesnt want f(5)->f(4).

.
.
.

Generally, 

if n is even, f(n) = {0, 1, 0, 1, ...., 101-n/2}
if n is odd, f(n) = {1, 0, 1, 0, ..., 100-floor(n/2)}
