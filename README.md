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

Hour: time of order (in hours)
weekday: day of the week on which order placed
accept_time_null: 1 if NAN else 0

Missing vales in a column data are filled by mean of the column.

## **MODEL**

The dataset was trained on ANN model.
