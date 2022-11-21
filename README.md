# P-S
```
x <- runif(100,-6,6)
dt(x,1)
dt(x,4)
dt(x,10)
dt(x,30)
df = c(1,4,10,30)
colour = c("red", "orange", "green", "yellow","black")
plot(x, dnorm(x), type = "l", lty = 2, xlab = "t-value", ylab = "Density",main = "Comparis
on of t-distributions", col = "black")
for (i in 1:4){
lines(x, dt(x, df[i]), col = colour[i])
}
legend("topright", c("df = 1", "df = 4", "df = 10", "df = 30", "normal"),col = colour, tit
le = "t-distributions", lty = c(1,1,1,1,2))
```
