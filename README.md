# Vending-Machine-API
# API Documentation

## Introduction:- 
A REST API (also known as RESTful API) is an application programming interface (API or web API) that conforms to the constraints of REST architectural style and allows for interaction with RESTful web services. REST stands for representational state transfer.

## Stepwise instructions to run on windows:-

### 1.	
At first , Install the requirements to run the python code.

aniso8601==8.0.0
click==7.1.2
Flask==1.1.2
Flask-RESTful==0.3.8
Flask-SQLAlchemy==2.4.3
itsdangerous==1.1.0
Jinja2==2.11.2
MarkupSafe==1.1.1
pytz==2020.1
six==1.15.0
SQLAlchemy==1.3.18
Werkzeug==1.0.1

To install this , I have already given “requirements.txt” file.

Open command prompt,
Give the instructions,

	    cd file_location 
	    pip install -r requirements.txt(file_name)

 


### 2.	
If you have “app.py” file at the same location

Give command as
	flask run
 
So the code is running
URL is given. Go to that url.
	127.0.0.1:5000/customer?drink=coke&penny=1&nickle=0&dime=0&quartet=1

 
We can give the input at URL  by changing the values so when we will make any website or when we implement it then we will get input from the URL.

 

OR

We can directly run also by changing some code. By giving the input.

 


### 3.	
If supplier wants to reset the system (vending machine)
Use the URL:-

	127.0.0.1:5000/supplier

 

So it will restart the system.
We can also add password feature in it so that only supplier who knows the password can reset the system.




## Working of the system:- 

We have 3 products:- 
Coke = 25rs 
Pepsi = 32rs 
Soda  = 47rs

So customer can select out of this 3 products and customer can pay for it in 1rs , 5rs, 10rs and 25rs.

Penny = 1rs
Nickel = 5rs 
Dime = 10rs 
Quarter = 25rs

So the code will take the input from the machine.

Example:- 
1.	If customer want “Pepsi” and If he give 1 Dime and 1 Quarter.
So he will get refund of 35-32 =3rs.

  
 So the customer will get pepsi and 3rs (3 * penny) in refund.


2.	If customer want “Coke” and If he give only 1 Dime.

 
He will get error as “Insufficient amount” and money will be refunded.

3.	If customer give much more that actual price and machine do not have that much change.

 
### FOR SUPPLIER:-
 
Data will be stored like this
