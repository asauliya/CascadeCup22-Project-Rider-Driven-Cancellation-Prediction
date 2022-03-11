# Cascade_Cup_2022
## Rider-Driven-Cancellation-Prediction
#### **Background:**

At Shadowfax, part of the business includes delivering food orders from clients such as Swiggy and Zomato to customers. The typical order flow goes something like this:
- A client creates the order in our system
- The order gets allocated to a rider
- The rider accepts the order
- The rider goes to the pickup location
- The rider picks up the order
- The rider goes to the delivery location and delivers the order

The rider also has the option to get the order cancelled before delivery by calling the client’s call centre. We would like to predict this kind of cancellation before it happens so that we can try and reassign the order to another rider before it gets cancelled.

#### **Problem Statement:**

Given the order and rider details as described below, create a model that can predict rider-driven cancellation in advance (i.e. before getting marked as cancelled or delivered).

## **DATASET**
Kaggle link : https://www.kaggle.com/c/cascade-cup-22/data

## **FEATURE ENGINEERING**
### **New features added**

Average_mile_distance : Average distance the rider has to cover to deliver the order

diff1 : Timestamps difference between allot_time and order_time

diff2 : Timestamps difference between accept_time and order_time

Reassignment_method was encoded as follows:

reassignment_method ={'auto':1 ,'manual':2 ,'nan':3}

order_day and month: Day and month on which the order was placed

riders: Frequency of orders alloted to each rider in train and test dataset

order_change_final : Binary encoding of change in undelivered orders of a particular rider

## **MODEL**

The dataset was trained on catboost model and the AUC on validation data was around 0.95.

AUC on private dataset : 0.90134
