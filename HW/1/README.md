#Exam Questions <img src="../../Resources/exam.png" width=50px alt="Tick Sheet">

##Instructions
Edit this document and answer the questions in the sections surrounded by ```.

There are 30 marks available and are awarded grades as follows:

|Score|Grade|
|-----|-----|
|<6|U|
|6+|G|
|9+|F|
|12+|E|
|15+|D|
|18+|C|
|21+|B|
|24+|A|
|27+|A*|


##Data Representation

###1 - Why do we represent data using binary when using computers *(1 mark)*

```
Because the computer reads it as on or off
```
###2 - How would we represent the number 147 in binary? *(1 mark)*
```
10010011
```
###3 - Can you convert the hexadecimal number **b5** to denary, there is a mark for you working. *(2 marks)*
```
115
```
###4 - Here is a function written is **pseudocode**.
```
FUNCTION validUser (users , user)
    FOR x <-1 to LEN(users)
        IF users[x] = user
			RETURN True
		ENDIF
	ENDFOR
	RETURN False
ENDFUNCTION
```

(a) What type of data is **users**? **(1 mark)**
```
String
```

(b) What type of data is returned by this function? **(1 mark)**
```
Boolean
```

##Errors
###6 - This program is supposed to find the mean of a list of numbers and print it out for the user:
```
line1:		tot <- 0
line2:		nums <- [1,6,4,2,5,3]
line3:		FOR x <- to LEN(nums)
line4:			tot <- nums[x]
line5:		ENDFOR
line6:		mean <- tot
line7:		OUTPT mean
```

(a) On which line is there a **syntax** error? **(1 mark)**
```
7
```

(b) What is meant by a **syntax** error? **(1 mark)**
```
answer here
```

(c) Identify a logical error in the program and suggest how this might be fixed. **(2 marks)**
```
4 it needs to be tot=tot <- nums[x]
```

(d) Describe and give an example of the 3rd kind of programming error. **(2 marks)**
```
run time divide by 0
```

##Algortithms
###7 - Write an **algorithm** that if given a list of numbers could find the largest. Try to use [pseudocode](http://filestore2.aqa.org.uk/subjects/AQA-GCSE-COMPSCI-W-TRB-PSEU.PDF).
```
NumberList=[54,3,67,93,95,-64,7338,6.945,848,884,56565,334.34,56.34,45,-1]

isSorted=False

while isSorted==False:
    for element in range(len(NumberList)-1):
        if NumberList[element] > NumberList [element+1]:
            isSorted=False
            temp=NumberList[element]
            NumberList[element] = NumberList[element+1]
            NumberList[element+1] = temp
            print(NumberList)

```

##Networking
###8 - Research the following methods (*topologies*) for connecting devices to a network. In each case give a description and at least 1 advantage and 1 disadvantage.

**Bus Topology (6 marks)**
```
Describe:A bus network is a network topology in which nodes are connected in a daisy chain by a linear sequence of buses.



Advantages:
It works well for small networks.
Disadvantages:
Entire network shuts down if there is a break in the main cable
```

**Ring Topology (6 marks)**
```
Describe:A ring network is a network topology in which each node connects to exactly two other nodes, forming a single continuous pathway for signals through each node - a ring. Data travel from node to node, with each node along the way handling every packet.

Advantages:Very orderly network where every device has access to the token and the opportunity to transmit

Disadvantages:Communication delay is directly proportional to number of nodes in the network
```

**Star Topology (6 marks)**
```
Describe:Star networks are one of the most common computer network topologies.

Advantages:star topology prevents the passing of data packets through an excessive number of nodes. At most, 3 devices and 2 links are involved in any communication between any two devices. Although this topology places a huge overhead on the central hub, with adequate capacity, the hub very high utilization by one device without affecting others.


Disadvantages:Failure of the central hub renders the network inoperable
```
