🚧 Note to myself.
The use of a tool that convert shortcut line composed of grammar token & Unicode token to actions. Is reusable in many project.
And maybe I should rename this repository or make a dependency.

For example: WOMI is use here for 🐁◲800:40 but could be use to 🔈0.5 or 📋>🗁TextArchive
- 📷🗔Wow>🗁Screenshot
- 📷💻Main>🗁Screenshot

--------------------------
# Abstract Omi Action Parser

Unicode used: ➤ ☗ | ↓ ← → ↑ _ ‾ ∨ ∧ ¬ ⊗ ≡ ≤ ≥ ⌃ ⌄ ⊓⇅ ⊔⇵ ⊏ ⊐ ↱↳ ∑ -no unity ⤒ ⤓ ⌈ ⌊ 🀲 🀸 ⌛ ⏰ ▸ ▹ 🐁 🖱 💾 ↕ ♺ 💻 🗔 🖧 ◩◪⬔⬕⬓⬒◧◨◰◱◲◳⯐

The goal of this repository is to recovert a string and convert it to a group of abstraction action to do that is parse at the end by the developer like he want it to be implemented.

### Specific: 
#### 'Compile'/reused line
If the line start by "♺", it means that this line will be called a lot's of time and can store when parsed to be reused.
Example:

In general, you should use "♺" with line that will be used every n < 5 minutes with not variation.
Bonus: You win 0.001-2 milliseconds on bad optimised, complex and long commands to parse
Malus: More you use it, more we store text in the RAM.

//This line that will be use by the player all the time in the game should use '♺'
♺Space↓ 200> Space↑ 80 Ctrl↓ 200> Ctrl↑  

//This line that will be use one in while to do a specific task like the following don't need it. 
🐁◱800:900 1000> 🐁◱800:600 80 LeftClick⇵ 

- " 80> "= Wait 80 milliseconds between action
- " A↓ " = Press key A
- " A↑ " = Release key A
- " 🐁◱800:900 " move at Main Screen 800: 900 px
- " 🐁1◱800:900 " move at Main Screen 800: 900 px
- " 🐁2◲50:0.1 " move at Second Screen 50px left of right border and 0.1 percent of top from bottom border
- " 🐁3◳800:900 " move at Third Screen 800 left to right: 900 px top down

🎘 Send Midi note to window default
♩ 
- 🎤 Request your default "Jarvice" to say an sentence; 
- 🎮 Simulate a xbox controler move if you have install the driver to simulate one

# Post Message
Not sure if there is the option on mac and linux, but on window you can send send event of mouse or key stroke to the system and let's the application catch it.
Or you can directly target the application and send a kind of "fake" message.
Bonus:
- You don't need focus for keystroke
- You don't need to move your mouse for mouse action ( but still the app focus)
Malus: 
- Not recognize by all application
- Could lead to ban automatic detection on some game 
🖅📮✉
