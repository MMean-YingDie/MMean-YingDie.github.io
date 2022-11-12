# AI-based On-Car Security Net

## 1.Introduction

### 1.1 background

In big city such as Shanghai and Newyork, where is populaiton density is high and crowded, there are also plenty of wild cats and dogs. But there's an issue with is. 
Since cats and dogs don't know anything about road security, they might cross the road without people noticing it. That could cause injuries and even death of  the poor animals. This has happens to us once where we couldn't see the animal and crush into it, causing the animal to be dead. As an animal lover and a inventor, I  think there's difinately something I could do with this problem. Maybe I could invent something to save the animal's life, if no, at least decrease the amount of these  tragedies.

![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/main/u%3D490135195%2C4184572886%26fm%3D253%26fmt%3Dauto%26app%3D138%26f%3DJPEG.webp)

This is a picture of a dog that crash into a car in China.

### 1.2 Current approach

Now, people aren't really solving the problem of animals on road. Most are discussing how to bury them or even luck. Many people make videos about what if  you're driving a care fastly and met a animal, the conclusion is hold tight and bump right into the animal. People doesn't seems to see this as a serious problem.m  Although there are many news reports everyday, people only gets sad for a few minute about these animals, no action is really taken to solve this.

### 1.3 Objective

After some brainstorm, we decide to solve the problem fundamentally, that is, on the cars. Since cars are made out of irons and could run up to 100 k/h, no  doubt that  animal would be hurt by it. But what will happen if the things thaat crash in to animal is not iron, but something soft? Moreover, what will happen if that  something soft could grab the animal and put it somewhere safe? Even if that could not save every life, just saving one more means a great thing. Thus, we decide to  use YOLO to detect animal and use a soft net infront of the car to capture it, this allows the animal to be seen and capture all atomatically without the need of  manuale act.
![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/main/lQLPJxbdmTejMwXNAZDNAZCwr1ZxZWwWvigDbCIf7sCFAA_400_400.png_720x720q90g.jpg)

This is an example of a net that could be used as our prototype module

## 2 Mthodology
![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/main/logic%20map.png)

This is a flow chart of how our logic works. It start from reading an image to detect animal, it decides whether there is an animal in it. If yes, it starts to release  scent and sounds to drive the animal away. If this didn't work, we will ned to lower the net and capture the animal. When that happens, the system tells the driver to  stop and release the animal.

### 2.1 Overview

By placing a net in front of the car, the damage can be lower to none. Our product can be divided into 2 parts, software and hardware. The soft ware is used to  detect animal, and tells the hardware what to do. It is kind of like an eye and a brain. The hardware is like our hand, it is use to capture animal and what really  saves the life of a animal. We also have a part on the harcore which could spread smells and supersonic to drive away the animal. But if the animal didn't the net will  capture the animal and turn off smells and sounds.
	
### 2.2 ACNet

The ACnet is the main part of our product. The net is used to capture animals and protect them. It is also the main part of our product. The net include the  actual net and the soft holder. The soft holder could prevent the animal from being harmed when it crash in to the car. The net is what hold the animal and takes it  away from the dangerous road.

### 2.3 Animal detection

Animal detection is a critical part on our product. If it fails, the animal can still end up dead. Or if it detect something else as an animal, the net could  comes out too early, causing many air resistance, which make the car go slow and lower its aesthetics. In the code, we make teddy bear, dogs, cats, cows, pigs and  sheep all count as animal and will activate the net. Not only because those animal could be found on street, but because the algorism some times mess things up, and  consider cats and dogs as other animal. So by this consideration, out code should be more comprehensive.
![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/main/dog%20crossing%20street%201.PNG)

This is a picture of our Yolo algorithm detecting dog from a video tape.

### 2.4 Sounds and smells

Because dogs and cats and other animals have a lot stronger hearings and smellings, they could easily smell or hears things we couldn't. And some of those  sounds or smells make them uncomfortable, which drives them away. We have a recorder and smeller on our net and is both acitivated when no animal is in the net. And  that could drive animal away from the road, which also could prevent the crash. Still, the net will be used incase some animal didn't get out of the way. The device  will close once an animal is captured because we don't want any animals to be uncomfortable.


### 2.5 System 

#### VTK simulation

The VTK is a software we used to show our 3D model. It helped us to see our net, and can stimulate the movement of nets, including turn, capture, open, and  close.
![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/main/simulation.PNG)

This is a picture of our VTK car and it's net reacting to a dog in a video.

#### Hardware

For the hardware, we had arduino board, which acts like a brain in human body. All the direction are given to the arduino board and arduino tells the other  parts what to do. The parts it control include seering engine; which controls the open and close of net; the camera; the scents and sounds; and most importantly,  determine whether it is an animal infront. 
![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/f33a60cb7e63aee40d7ac1ca791acea4f14a3879/%E7%BB%93%E6%9E%84.PNG)

This is our 3D module I made in 123D, it includes all the hardware and their placement our VTK module also is from this module.

#### Power supply

Our power is supplied by batteries, huge ones like used in Tesla, these batteries can supply the system for many hours so even a long distance trip would be  enough. The batteries are hide inside the net cover where it is safe ane easy to charge.

#### Software

Our software is mainly made out of the animal detection and mixly coding. We first use YOLO algorism to detect animal and then commands the spread of scents  and sounds. If it didn't work, accroding to our mixly coding, the nets will open to capture the animal. The software is like the mind we got in our head.

#### User interface	

We also created a switch on the user's phone, connected to the net. Sometimes the camera might misdetect and thus open the net when it should not. This also  might cause injury if there's someone infront of the car or cause alot of air resistance. Thus, this switch on the user's phone is useful when something goes wrong.

## 3.RESULTS AND DISCUSSION

### 3.1 Simulation Result

We first put a model dog infront of the camera, and see if the code detect it. And when it did, VTK also successfully responds by emmiting smells and sounds.  And when the code still detects the dog, VTK responds by lower the net and ready to capture the dog while close the sound and smells. After that, when the dog is  successfully captured, VTK tells the car to slow down and put the dog aside. More detailes is in this flow chart.

### 3.2 Graph Result

We found multiple video clips online with dogs on the street and see if our simulation VTK is working. In the first video, there is a cat that appears for a  minute continuously, our VTK have successfully react to the cat and lower the net to capture the dog, the net remain lowers until the cat can no longer be detected by  the camera.
In the second video, there is multiple dogs that shows up at different times. The first dog appears at 1 minute, the second dog appears at 3 minute, the final  dog appears at 4 minute. The VTK react as usual and successfully at the first and second dog, however, in the third dog, probably because the gap between the 2 dogs is  too small, it took VTK sometime to react to it, this might cause injure in real life.
In the final video, there is only one dog that appears suddenly on highway and only exist for 2 second. The VTK successfully react to it in 2 second. However,  on a highway, this reaction time might be too slow to safe the life

![](https://raw.githubusercontent.com/MMean-YingDie/MMean-YingDie.github.io/main/u%3D11001331%2C1772941715%26fm%3D253%26fmt%3Dauto%26app%3D138%26f%3DJPEG.webp)

This is a picture of one of the video we used to test our net and code.
	

# 4 Conclusion

In conclusion, this device although may seem useless and can not save animals in all conditions, this is for saving lifes. If an animal got caught up bu cars,  it will be injured or die, certainly. However, with this device, it can decrease the damage to none. Even if it can't save every single animals, saving just one is a  great thing. The overall statistics support our idea and this canw be used to future events and lifes. However, most of these are just a code or based on theory, if there's a chance, in the future, I would like to make an actual module on a real car and test it, perhaps make this in to a product if it is possible and actually useful.
