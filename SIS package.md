# SIS package

Automatically sets seed itself, which is different from many other R packages

To do iterations,

```for(iter in 1:500){
  set.seed(iter)
  x=matrix(rnorm(n*p),n,p)
  epsilon=rnorm(n)
  y=(x%*%beta)+epsilon
  # Run SIS based on data
  #......
}
```