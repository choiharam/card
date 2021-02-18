# Card playing with Circuitry

<img width="1000" alt="banner" src="https://github.com/choiharam/card/blob/main/images/banner.jpg">  

**Card playing with Circuitry** is a set of cards designed to play a game with a breadboard and many different electronic components. This page describes how to play the game with this card. It's still in the process of prototyping, so any suggestion is welcome!
It's design and used components are inspired from the Seminar [**Circuitry-based sound.**](https://github.com/SCLW/Circuitry-Based-Sound)  

(The title of this game is not defined yet.)


# Contents
> - [Requirement](#Requirement)
> - [Basic rule of the Game](#Basic-rule-of-the-Game)
> - [Things to decide before the Game](#Things-to-decide-before-the-Game)
> - [Printing the Cards](#Printing-the-Cards)
> - [List of Commands](#List-of-Commands)
> - [Possible application](#Possible-applications)

# Requirement

The required components to play this game are:

- A set of this card
- Breadboard x1
- An active loudspeaker
- Many jumper cables
- Many capacitors
- Many resistors
- Many LEDs
- Many diodes
- CMOS chips(CD40106, CD4093, CD4070)
- Some knowledge of how to use these components

The CMOS chips used in this game is limited to above mentioned three chips. There needs to be a more detailed rule in order to use additional chips like CD4040.



# Basic rule of the Game
1. This game is designed for **2 players**.
2. One of them will play the role of **Defender** and the other one will be the **Attacker**.
3. The goal of the **Defender** is to generate **OUTPUTs** with the circuit. (see below for more detail of [**OUTPUT**](#What-means-OUTPUT-in-this-Game))
4. The goal of the **Attacker** is to neutralize every **OUTPUT** made by the **Defender**.
5. The players will start the game with **6 cards** for each.
6. **One breadboard** needs to be prepared.(one board for two players, not for each)
7. The **Defender** will play the **first turn**.
8. In each turn, the player will flip one card from the holding 6 cards, and then **execute the command** written on the flipped card. *(e.g. Use one new capacitor, Remove one resistor)*
9. The one who just completed the turn, should **draw a new card** from the deck. *(So each player always has to hold 6 cards in the hand until the deck is empty)*
10. There are two different senarios of **how to end this game**:
  
  
#### Ending Senario_01 (I would call it _simple_)

	The game ends if one of these two conditions is met:  
	
		- The deck is empty, and both player has no card holding.  
		- The Defender generates an OUTPUT. (see below for the detail).  
		
	The Attacker wins, when the game ends with the first condition.  
	The Defender wins, when the game ends with the second condition. 

#### Ending Senario_02 (with a score system)

	The game ends only if the deck is empty.
	And the winner will be the one who has more points at the end.
	But if both player has the same point and the deck is empty at the same time, then the Attacker wins.
	
		- The Defender gets 1 point for each OUTPUT.
		- The Defender gets 1 point in every turn, when the Loudspeaker is making sound.
		- The Attacker gets 1 point when anyone of the OUTPUT is neutralized.
		- The player who burns or destroys a component will loose 1 point for each.

#### What means OUTPUT in this Game?
- **OUTPUT** means,
	1. sound generated through the **Loudspeaker**. (Floating noise is excluded)
	2. Light emitted from the **LED**. Possibly in any frequency.
	3. More possible candidates: (not included yet)

		> - Piezo buzzer
		> - Stepper motor(?)
		> - Any kind of component that can generate a kinetic or acoustic output
		> - (any idea?)

# Things to decide before the Game
There are several rules that need to be decided by the players. This is because, it works as a variable that can be adjusted to the actual condition of the players. (e.g. knowledge, total number of the components, etc.) And most of all, different variable can create more interesting procedure and results.

1. **What do you want to have on the breadboard at the beginning?**
	- Few examples:  
		1) Start with an empty breadboard. (not recommended)  
		2) Start with a CMOS chip on the breadboard.  
		3) Start with a complete circuitry on the breadboard.(e.g. square wave oscillator, LED sequencer, random function, etc.)
2. **Who will play the first turn?**
	- Above in the basic rule, it's written that the Defender shall play the first turn. This is because defending(generating an OUTPUT) is more difficult in many cases. Additionally, it will make less sense to neutralize the circuit if the game begins with an empty circuit. **BUT** it's up to what the players want. So it should be decided before the game begins.
3. **How many turns do you want to play?**
	- As mentioned above, the game will end in a certain condition. But it might be too long to continue the game until the deck of the cards is empty. So one might want to have a limit of the card, or the number of the playing count. **OR** you can also decide to use two sets of the card. Then, each card will have double of the chance to appear.
		
# Printing the Cards
The design of the card is still under construction. But I'm planning to print out and make it as a physical card. It will look like any conventional game card. The back side design is not planned yet. Here you can see what I have done so far:

![cards](https://github.com/choiharam/card/blob/main/images/cards.gif)
  
![card01](https://github.com/choiharam/card/blob/main/images/card01.jpg)
![card02](https://github.com/choiharam/card/blob/main/images/card02.jpg)  

![card03](https://github.com/choiharam/card/blob/main/images/card03.jpg)
![card04](https://github.com/choiharam/card/blob/main/images/card04.jpg)  

![card05](https://github.com/choiharam/card/blob/main/images/card05.jpg)  


## List of Commands
- A Command is a sentence written on the card.  
- Each card has a different command and a corresponding simple illustration.
- Total of 38 commands are made so far, but can be added more.
<details>
	<summary> <i>Show the list</i> </summary>
	
1. "Use one new jumper cable, and connect at least two existing components."
2. "Use one new jumper cable, and connect two different pins of a CMOS chip."
3. "Use two new jumper cables, and connect at least two existing components."
4. "Use two new jumper cables, and connect at least three existing components."
5. "Use a new capacitor."
6. "Use a new resistor."
7. "Use a new diode."
8. "Use a new LED."
9. "Use two new capacitors."
10. "Use two new resistors."
11. "Use two new diodes."
12. "Use two new LEDs."
13. "Use one new capacitor and one new resistor."
14. "Use one new capacitor and one new diode."
15. "Use one new capacitor and one new LED."
16. "Use one new resistor and one new diode."
17. "Use one new resistor and one new LED."
18. "Use one new diode and one new LED."
19. "Use one new CD40106, and connect the VDD and VCC respectively."
20. "Use one new CD4093, and connect the VDD and VCC respectively."
21. "Use one new CD4070, and connect the VDD and VCC respectively."
22. "Remove one jumper cable, but not the one connected to the Loudspeaker."
23. "Remove one jumper cable, only that is connected to CMOS chip."
24. "Remove one of any existing jumper cable."
25. "Remove one capacitor."
26. "Remove one resistor."
27. "Remove one diode."
28. "Remove one LED."
29. "Change the position of one end of a jumper cable to somewhere else."
30. "Pull out one jumper cable and place it somewhere else. (removing excluded)"
31. "Pull out one resistor and place it somewhere else. (removing excluded)"
32. "Pull out one capacitor and place it somewhere else. (removing excluded)"
33. "Pull out one diode and place it somewhere else. (removing excluded)"
34. "Pull out one LED and place it somewhere else. (removing excluded)"
35. "Swap a passive component to another new passive component."
36. "Swap a passive component with another existing passive component."
37. "Swap an existing CMOS chip to another new CMOS chip"
38. "Swap an existing CMOS chip with another existing CMOS chip"

</details>

## Possible applications
This project is not done yet, and has so many things to be decided or adjusted.  
The way of how to develop this game could vary depending on what I want to do, or what we want to do with this.  

What I think would be nice to make is...  

1. **a Performance on the stage.**
	- The main concern from this perspective is that, there might be no OUTPUT(sound) for a long time. And having no dynamic stuffs on a stage for a long time is not good at all, since it will make it boring. And as you might know, this game is somewhat too difficult for the audience to follow. So there needs to be many more considerations in order to perform it on a stage.(like having a ready-made-senario of how to play each turn, combining with a different kind of performance, etc.)	
2. **an Educational Tool by which people can learn simple rules of how to use electronic components.**
	- For this, the game itself needs to be more simplified. If there is no CMOS chip in this game, and if we do this only with LED, resistor and capacitor, then even people without any background knowledge of electronics could also play this game(by learning a tiny bit of the components, like anode and cathode of the LED, etc.)
3. **just a Game. like Chess or Go.**
	- Let's grab some beer and play this!
