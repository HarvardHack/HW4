Inference 1

babies = read.table("babies.txt", header=TRUE)

q1:

bwt.nonsmoke = babies$bwt[babies$smoke==0]
bwt.smoke = babies$bwt[babies$smoke==1]
dat.ns = head(bwt.nonsmoke, 30)
dat.s = head(bwt.smoke, 30)
t.test(dat.ns, dat.s)$statistic

q2:

2*pnorm(-abs(tval)) 

q3:

The probability of making a Type I error is equal to the probability that the null hypothesis is true. 



