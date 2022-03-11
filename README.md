# Rider-Driven-Cancellation-Prediction
At Shadowfax, part of our business includes delivering food orders from clients such as Swiggy and Zomato to customers. The typical order flow goes something like this:
A client creates the order in our system

1. The order gets allocated to a rider
2. The rider accepts the order
3. The rider goes to the pickup location
4. The rider picks up the order
5. The rider goes to the delivery location and delivers the order

The rider also has the option to get the order cancelled before delivery by calling the client’s call centre. We would like to predict this kind of cancellation before it happens so that we can try and reassign the order to another rider before it gets cancelled.

Training Data: https://www.kaggle.com/c/cascade-cup-22/data

## Problem Statement
Given the order and rider details as described below, create a model that can predict rider-driven cancellation in advance (i.e. before getting marked as cancelled or delivered)

## Our initial approach towards the problem statment:
