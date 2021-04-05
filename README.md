## Group 6
1. Md. Maksudur Rahamn (CSE-01306093)
2. Anisur Rahman (CSE-01306134)
3. Toha moni Mojomder (CSE-01306087)
4. Asma fowzia (CSE-01306132)

## CONDITIONS FOR SINGLE CHANNEL QUEUING MODEL
The single channel queuing model can be fitted in situations where the following seven conditions are fulfilled:

The number of arrivals per unit of time is described by poisson distribution. The mean arrival rate is denoted by λ.
The service time has exponential distribution. The average service rate is denoted by μ.
Arrivals are from infinite population.
The queue discipline is FIFO, that is, the customers are served on a first come first serve basis.
There is only a single service station.
The mean arrival rate is less than the mean service rate i.e. λ < μ.
The waiting space available for customers in the queue is infinite.


## Introduction:
 
To describe queuing problems through mathematical formulation, some assumptions are made by considering arrivals and services as patterned by known function. Equations representing the distribution of the time between arrivals are used with other equations depicting other features such as the distribution of the service time. The relationship existing between these equations is the matter studied in waiting line theory. Arrivals of people or entry requirements (events) are customarily Poisson distributed. The duration of the service provided by people is usually exponentially distributed. For generating interarrival and service times, gamma and Weibull distributions are also utilized depending on the model as the exponential distribution is said to be a special case of both of the gamma and Weibull distributions.


## Random Variable:

A random variable is a variable whose possible values are numerical outcomes of a random phenomenon. There are two types of random variables, discrete and continuous.

A discrete random variable may take on only a countable number of distinct values and thus can be quantified. For example, you can define a random variable X to be the number that comes up when you roll a fair dice. X can take values : [1,2,3,4,5,6] and therefore is a discrete random variable.

Some examples of discrete probability distributions are Bernoulli distribution, Binomial distribution, Poisson distribution, etc.

A continuous random variable takes an infinite number of possible values. For example, you can define a random variable X to be the height of students in a class. Since the continuous random variable is defined for values, it is represented by the area under a curve (or the integral).

A curve meeting needed requirements is often known as a density curve. Some examples of continuous probability distributions are normal distribution, exponential distribution, beta distribution, etc.

There’s another type of distribution that often pops up in literature which you should know about called cumulative distribution function. All random variables (discrete and continuous) have a cumulative distribution function. It is a function giving the probability that the random variable X is less than or equal to x, for every value x. For a discrete random variable, the cumulative distribution function is found by summing up the probabilities.


## Single Channel Queuing Problems:

Single-station or single-channel queuing problem is the name applied to those problems in which only one unit (station) is delivering the service as illustrated in Fig, where circles represent the arrival elements (events) and a square represents a station which contains an element being serviced.

## Poisson Arrivals:

The Poisson is a discrete probability distribution and yields the number of arrivals in a given time. The exponential distribution is a continuous function and yields the distribution of the time intervals between arrivals. The Poisson distribution considers the behavior of arrivals as occurring at random and postulates the presence of a constant “λ” which is independent of the time. The constant λ represents the mean arrival rate or the number of arrivals per unit of time, and λ 1 is the length of the time interval between two consecutive arrivals.

## Exponential Service Times:

In Exponential Distribution, we can generate an exponentially distributed random variable using scipy.stats module's expon.rvs() method which takes shape parameter scale as its argument which is nothing but 1/lambda in the equation. To shift distribution use the loc argument, size decides the number of random variates in the distribution.

## Mathematical Analysis:

So first we import scipy.stats package for importing necessary function. Here we use Poisson and Exponential Distribution to generate interarrival time and service time respectively. µ=5.6 customers/minute (arrival rate) λ=1 customers/minute (service rate) for 20 customers.
