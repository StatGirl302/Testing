# Testing


Simulate Random Variables:  Normal vs. Poisson Distributions
```{r}
# Create Normal Random Variable with mean zero and standard deviation 1
x <- rnorm(500)  # creates 50 standard normal random variables
# Create Poison Random Variable with mean zero and standard deviation 1
y <- rpois(500,2) # creates 50 poisson random variables with lambda = 1
```

Plot histograms & density curves
```{r}
par(mfrow=c(1,1))
hist.x <- hist(x, col="blue", main= "Histogram of Standard Normal RV", xlim=c(-5,5), ylim = c(0, 0.5), prob=TRUE)
density.x <- curve(dnorm(x, 0, 1), col="purple", add=TRUE)



```
