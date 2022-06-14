# Probability Description Language

PDL is used to calculate discrete probability problems. The answer to many probability questions is counterintuitive and not obvious. DSL designs a way to describe the probability problem as code, and then calculate the probability value.

## sample1
There are four balls in a bag, with the numbers 1 to 4 on the balls.
Take out a ball twice. What is the probability that their sum equals 6?

  
```javascript
bag 1,2,3,4 //Define a bag with 4 balls inside
select 1 ball1 from bag  //Take a ball from the bag and name it ball1
select 1 ball2 from bag  //Do it again and name it ball2
ball1+ball2=6 //Calculate the probability that their sum equals 6
```

sampling without replacement：
```javascript
select 2 balls from bag
balls[1] + balls[2] = 6 //Calculate the probability that their sum equals 6
```
