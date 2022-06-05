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
