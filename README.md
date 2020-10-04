### Week 2 : Assignment - William Mutua


a) What items should the thief take, for items taken as fractions, indicate the fractions

The ratio between the profit and the weight (p/w) gives the order of priority of which objects should be considered first, from the highest ratio to the lowest ratio representing the first and last object the thief should choose. This will maximize profit and also take into consideration the max W of the knapsack

Ratio A=5, B=1.67,C=4,D=1, E=6,F=3.6, G=3
In order of priority, they should first take=E,A,C,F,G,B,D

The thief should take 
E=1,A=1,C=1,F=1,G=1,B=(16-14)/3=0.67,D=0

b)What will be the total profit the thief will achieve for selecting these items.
6+10+20+18+3+(0.67*5)=60.3


c)Solution: 
```
    Jupyter Notebook
```

SOLUTION
1. The function fractional_knapsack is defined.
2. It takes three arguments: two lists value and weight; and a number capacity.
3. It returns (max_value, fractions) where max_value is the maximum value of items with total weight not more than capacity.
4. fractions is a list where fractions[i] is the fraction that should be taken of item i, where 0 <= i < total number of items.
5. The function works by choosing an item from the remaining items that has the maximum value to weight ratio.
6. If the knapsack can include the entire weight of the item, then the full amount of the item is added to the knapsack.
7. If not, then only a fraction of this item is added such that the knapsack becomes full.
8. The above three steps are repeated until the knapsack becomes full, i.e. the total weight reaches the maximum weight.

EXECUTION

1. You will be prompted to enter the number of items n.
2. You will then asked to enter n values and n weights.
3. The function fractional_knapsack will be called to get the maxmimum value and the list of fractions.
4. The result will then displayed.
