This is a small project i made to help improve women's safety,especially in situations where someone feels unsafe or needs help quickly.The idea is to make something simple just a system that can send an sos message along with location and also give a basic idea of how safe the area might be.
i kept the project lightweight and easy to understand because during emergencies,people don't have the time to deal with complicated apps.
What this system can do
sends an sos message with your live location
checks the safety level of an area using a simple ML model
very easy to trigger(just one action)
Can be extended with UI later
Tech i used
Python
scikit learn for the small ML model
Any SMS API(like Fast2SMS)
How to run
clone the project
Install the reqired python modules
Run the main file
That's it no complicated setup.
Main code Example
Here is a short sample of how the system works.
```python
from sos import send_sos
from location import get_location
from safety import check_safety

def main():
    print("opening Women Safety System...\n")
    location = get_location()
    print ("Your Location:", location)

    safety_status =
  check_safety(crime_score=7)
    print("Safety Status:", safety_status)

    send_sos("9876543210", location)
    print("sos alert has been sent successfully!")

if__name__ == "__main_":
```



Why i chose this project
women's safey is something that affects almost everyone we know,directly or indirectly.I wanted to build something that at least tries to solve a small part of this bigger problem.
Even if this system is simple,the idea is meaningful.
Future Plans
Adding a proper app interface
Real time tracking
Auto trigger sos by phone shake
connecting with emergency services
This project is just a step towards something helpful.Even a simple system can make a difference if it reaches the right people at the right moment.




