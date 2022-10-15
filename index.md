# 1 Animal saver under cars

## 1.Introduction

### 1.1 background

	In big city, such as Shanghai and Newyork, where is populaiton density is high and crowded, there are also plenty of wild cats and dogs. But there's an issue with is. Since cats and dogs don't know anything about road security, they might cross the road without people noticing it. That could cause injuries and even death of the poor animals. This has happens to us once where we couldn't see the animal and crush into it, causing the animal to be dead. As an animal lover and a inventor, I think there's definatly something I could do with this problem. Maybe I could invent something to save the animal's life, if no, at least decrease the amount of these trajadies.


### 1.2 Current approach
	Now, people aren't really solving the problem of animals on road. Most are discussing how to bury them or even luck. Many people make videos about what if you're driving a care fastly and met a animal, the conclusion is hold tight and bump right into the animal. People doesn't seems to see this as a serious problem. Although there are many news reports everyday, people only gets sad for a few minute about these animals, no action is really taken to solve this.

### 1.3 Objective
	We've thought about to make the use of animal's strong hearings and smelling, but that wouldn't be a good solution because if there are animals that still want to go on the road, the trajady could still happens. Moreover, sometimes it is not the animal's fault that they want to cross the road, maybe they had to go to the other side of the road for some reason. After some brainstorm, we decide to solve the problem fundamentally, that is, on the cars. Since cars are made out of irons and could run up to 100 k/h, no doubt that animal would be hurt by it. But what will happen if the things thaat crash in to animal is not iron, but something soft? Moreover, what will happen if that something soft could grab the animal and put it somewhere safe? Even if that could not save every life, just saving one more means a great thing.



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
