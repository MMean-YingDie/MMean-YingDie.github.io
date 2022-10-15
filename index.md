# 1 INTRODUCTION 111111

## 1.1 BACK GROUND
	Exercising has always been a habit of many people around me. But all of them knows how expensive it can cost us. The average cost of a gym membership is normally around 60$ per month. Additionally, the current pandemic takes away the accessibility of public gyms. Therefore traditional gyms are unable to satisfy many user’s needs.

Exercising using sand bags as extra weight can be very tiring and useless because it is quite heavy and takes a lot of space. With the fitny, it acts as a smart weight bag using a air bag friction system installed in a knee/arm guard, which allows for light weight and portability.



## 1.2 Current approach
	The most popular thing used to add weight on one’s body to assert more force are weight vests, They are physical weights that you have to wear on your body. Most of the time they feel uncomfortable when wearing and it is inconvenient to bring around places. Additionally, resistance bands are another way to allow the further activation of your muscles used through the form of physical resistance, but it can only account for one specific level of force, and when you want to proceed on to a heavier level, you would have to buy another band. 
	
# 2 methodology
## 2.1 Overview
	A new system needs to be used to not only allow for the customizability of weight vests when switching out weight block s but also allow for the portability like resistance bands. So I have came up with the airbag pressure system. Using this developed technology, it can be put in to a knee guard or arm guard 
## 2.2Hardware design
	the circular casing that is placed on the side of the knees would act as the axle for the arm/leg connection to turn and with the air pumped inside, the friction of the airbag and the inside surface of the circular casing would increase. Thus it would make it harder to move, therefore requiring the user to use more force on the legs or arms to fold their joints like in many exercises we do everyday.
	The electronics connection is as shown in the second diagram with the Arduino board in the center and connecting to the battery for the device, the Bluetooth board for the connect not it to the user’s mobile device and the pump and valve for the pumping and locking in of air in the airbag. 
### 2.2.1 Hardare design
![](https://github.com/PheromG/pheromg.github.io/blob/master/Screen%20Shot%202020-12-29%20at%2010.46.35%20AM.png)
### 2.2.2 electronic connections
![](https://github.com/PheromG/pheromg.github.io/blob/master/Screen%20Shot%202020-12-29%20at%2010.43.04%20AM.png)

## 2.3 Processing(Arduino code)
	The Arduino board will be connected to a bluetooth chip, the battery, the air valve and pump which will be connected to our phones through bluetooth to allow the control of the pumps wirelessly. The phone application would specify the amount of force in kg to adjust in the device. Then it will send the command to the Arduino board to turn on the valve or pump for the specified amount of time, the code is a cycle which will assess either a command for the valve or pump is there and carry it out. It the board receives a command to start pumping, it would move on to see if there was a command for the valve to turn on as well and then it would carry out the command after each part is assessed. The cycle carries on continuously when the device is turned on. 
### 2.3.1 code flow chart
![](https://github.com/PheromG/pheromg.github.io/blob/master/Screen%20Shot%202020-12-29%20at%2010.44.46%20AM.png)

 ## 2.3User interface
	A phone application will be made for the user to control the pressure for their own devices and they can either use the default 2 second pump time to send to the Arduino board or they can customize how long they want their air pump time to be. Wan the user asks for the pump to be on, the valve would automatically be on as well to secure the air inside the bag, this command is sent from the phone so it does not interfere with the arduino code at all.

# 3 Results and discussion	
The device currently works but with little pressure in reality, it is not able to achieve the goal of having over 5kg of force, more designing in to the component is needed. However, it does work and the design does provide the user with some need of force(average of 0.5 kg checked using a force measurer).

## 3.1 Graph and table 
### 3.1.1 Graph
![](https://github.com/PheromG/pheromg.github.io/blob/master/Screen%20Shot%202021-02-05%20at%202.30.37%20PM.png)
### 3.3.2 table
![](https://github.com/PheromG/pheromg.github.io/blob/master/Screen%20Shot%202021-02-05%20at%202.25.36%20PM.png)

## 3.2 Resulting product
### 3.2.1 october 2020 perototype
![](https://github.com/PheromG/pheromg.github.io/blob/master/28b8e916ceacc891419d7c5676dff0c.jpg)

### 3.2.2 december 2020 prototype
![](https://github.com/PheromG/pheromg.github.io/blob/master/Screen%20Shot%202021-02-05%20at%202.26.41%20PM%201.png)











## 3.3 Application page 
 
The application is designed with 2 pages in which the first one allows the user to send default and customized time command to the air pump and the second page is where the user and put in their height and weight for a truly optimum pressure amount.
### 3.3.1 1st page
![](https://github.com/PheromG/pheromg.github.io/blob/master/32f702175dfeca4d6abb34ec4c90701.jpg)
### 3.3.2 2nd page
![](https://github.com/PheromG/pheromg.github.io/blob/master/01f5820053f390a9daed240dbc50f1b.jpg)






 






# 4 Conclusion
To conclude, the device is using an air pump as a pressure inductor and then with the Arduino board, it makes it Abel to receive commands for it to turn on or off. Then the Arduino program makes it so that it can turn on or off for a specific amount of time and with the bluetooth board, it is able to receive commands from another pat form for it to send to the Arduino board and lastly, the application is that platform which worked out extremely well. It was a successful product and in then end it does make the user exert more force when wearing the device. Overall, it is safe to say that this device would make working out more accessible to the public.
