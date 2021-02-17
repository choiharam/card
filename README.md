# Card playing with Circuitry

**Card playing with Circuitry** is a set of cards designed to play a game with a breadboard and many different electric components.

It's design and used components are inspired from the Seminar **Circuitry-based sound.**



The title of this game is not defined yet.

#### Contents
1. [Basic HOWTO of the Game](#Basic-HOWTO-of-the-Game)
2. [Printing the Cards](#Printing-the-Cards)


# Basic HOWTO of the Game
1. This game is designed for **2 players**.
2. One of them will play the role of **Defender** and the other one will be the **Attacker**.
3. The goal of the **Defender** is to generate **OUTPUTs** with the circuit. (see below for more detail of **OUTPUT**)
4. The goal of the **Attacker** is to neutralize every **OUTPUT** made by the **Defender**.
5. Each of two will start the game with **6 cards**.
6. **One breadboard** needs to be prepared.(one board for two players, not for each)
7. The **Defender** will play the **first turn**.
8. In each turn, the player will flip one card from the holding 6 cards, and then **execute the command** written on the flipped card. *(i.e. Use one new capacitor, Remove one resistor)*
9. The one who just completed the turn, should **draw a new card** from the deck. *(So each player always has to hold 6 cards in the hand until the deck is empty)*
10. There are two different senarios of **how to end this game**:
  
  
#### Ending SENARIO 01 (I would call it _simple_)

	The game ends if one of these two conditions is met:  
	
		- The deck is empty, and both player has no card holding.  
		- The Defender generates an OUTPUT. (see below for the detail).  
		
	The Attacker wins, when the game ends with the first condition.  
	The Defender wins, when the game ends with the second condition. 

#### Ending SENARIO 02 (with a score system)

	The game ends only if the deck is empty.
	And the winner will be the one who has more points at the end.
	
		- The Defender gets 1 point for each OUTPUT.
		- The Defender gets 1 point in every turn, when the Loudspeaker is making sound.
		- The Attacker gets 1 point when anyone of the OUTPUT is neutralized.
		- The player who burns or destroys a component will loose 1 point for each.

#### What means **OUTPUT** in this Game?
- **OUTPUT** means,
	1. sound generated through the **Loudspeaker**. (Floating noise is excluded)
	2. Light emitted from the **LED**. Possibly in any frequency.
	3. More possible candidates: (not included yet)
		- Piezo buzzer
		- Stepper motor(?)
		- Any kind of component that can generate a kinetic or acoustic output
		- (any idea?)

		
# Printing the Cards
I'm planning to print out and make it as a physical card.  
It will look like any conventional game cards.  
The design of the cards is still under construction.  
  
Here below, you can see what I have done so far:

![cards](https://github.com/choiharam/card/blob/main/images/cards.gif)
  
![card01](https://github.com/choiharam/card/blob/main/images/card01.jpg)
![card02](https://github.com/choiharam/card/blob/main/images/card02.jpg)  

![card03](https://github.com/choiharam/card/blob/main/images/card03.jpg)
![card04](https://github.com/choiharam/card/blob/main/images/card04.jpg)  

![card05](https://github.com/choiharam/card/blob/main/images/card05.jpg)  

These are the possible front side of the cards.  
The back side design is not planned yet.

## List of Commands
- A Command is a sentence written on the card.  
- Each card has a different command and a corresponding simple illustration.
- Total of 38 commands are made so far, but can be added more.

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


## Possible applications
This project is not done yet, and has so many things to be decided or adjusted.  
The way of how to develop this game could vary depending on what I want to do, or what we want to do with this.  

What I think would be nice to make is...  

1. a **Performance on the stage.**
	- The main concern from this perspective is that, there might be no OUTPUT(sound) for a long time. And having no dynamic stuffs on a stage for a long time is not good at all, since it will make it boring. And as you might know, this game is somewhat too difficult for the audience to follow. So there needs to be many more considerations in order to perform it on a stage.(like having a ready-made-senario of how to play each turn, combining with a different kind of performance, etc.)	
2. an **Educational Tool** by which people can learn simple rules of how to use electric components.
	- For this, the game itself needs to be more simplified. If there is no CMOS chip in this game, and if we do this only with LED, resistor and capacitor, then even people without any background knowledge of electricity could also play this game(by learning a tiny bit of the components, like anode and cathode of the LED, etc.)
3. just a Game. like Chess or Go.
	- Let's grab some beer and play this!
