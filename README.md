🚧 Note to myself.
The use of a tool that convert shortcut line composed of grammar token & Unicode token to actions. Is reusable in many project.
And maybe I should rename this repository or make a dependency.

For example: WOMI is use here for 🐁◲800:40 but could be use to 🔈0.5 or 📋>🗁TextArchive
- 📋↱🖹TextArchive Appent clipboard at start
- 📋↳🖹TextArchive Append clipboard at end
- 📋>🖹TextArchive set text file with clipboard
- 🖹TextArchive>📋 set text file with clipboard
- 📷🗔Wow>🗁Screenshot
- 📷💻Main>🗁Screenshot
- 🌐LocalNew>🖨️  
- 🔗Eloistree.com> >🖨️
- RSS:MyReddit>🖨️ 80> IFTTT:AmAwake
- 🔒Main>⌨️
- 🎲(0,100)  Do a random between 0,100
- 🌏⌚+2(Hour,Minute) >🎤Alexa  Ask what time it is on the global at country +2h and to make it read to Alexa  
-📋1↳🍪ToDoList store the clipboard in a app half ram, half file state

Injection in app et out of app:
Un personne doit savoir facilement ajouter son propre code dans l'application:
-Cmd|  GitLog:ActiveMe:In   Will note that you start to work by commit a message as in in the gitlog you added to the project.
  - "Si tu as besoin d'écrire des valeurs et du text c'est que une commande est plus adhéqua que une shortcut"
- 🐦LastMessage > ⌨️
- 🐦Elon > ⌨️
- 📋↳GDOC:Note
- 📋↳:Note
- 🖩(2*5354)>🪵 
- 🐸🎤   play a sound of "It is wednesday my dude
- g🗺️Japon  open google map focusing japon
- 📋>📖 Open dictionnary with clipboard content
- ✂️>💬(FR,EN,Google)  Cut the selected text and send it to google to translate
- >💬(FR,EN,Default)  Cut the selected text and send it to google to translate
-✂️>💬(FR,EN,Default)>🤖🎤

-Youtube:EloiStree  Cerche si il y a un FetchId qui correspond à EloiStree localement, sinon fait une recherhe youtube.
-Youtube:IPenser
-YT:Creator:Eloi
-YT:Search:Eloi

- 📋>🖧|MainComputer>📋
  - 🖧|MainComputer->In 5000|womi:📋80>
- 📋>📮🧍Eloi
- 🎤Last>🔎
- 🔎(Putin)

-🔒Main>📋 80> CTRL+V
-📋>🔐>📋  set the key of the current locker and write in the clipboard the corresponding password
-💻👀>🔒>📋  Look for app context and send the info to locker that if found will set the clipboard with password
Note:
- ⚔

- 🎲 Lib
  - 🎲{0123456789_}
  - 🎲Regex{0-9a-Z}
  - 🎲AlphaNum
  - 🎲🌐Name  Fetch random in a given collection of web api
  - 🎲Name   Fetch random in a given collection of name
  - 🎲🌐Mail 
  - 🎲Mail
  - 🎲📚FR
  - 🎲📚DE
  - 🎲📚Germany
- 📋HelloWorld>LUA 
- 🖹PyHelloWorld>Python


- Write some text ✂️>🖧|OmiSecondaryComputer   Envoyer à l'interpreter du second ordinateur une instructionc copier coller sur cette ordinateur
  - Just the idea that I could have that macro is mind blowing.
![Mind blow](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ6rV0IBxo1PxdmgQIlOidTpAfjfdA4qoqzNahFOpCF63zTVMcHzvB7qssoA7sWUsr3_UY&usqp=CAU)


What should I use to translate:
Command line macro:nameofthemacrotolaunch
Idea: ⚙🚀🎬📜⚡♨📝


Question to myself should I attack variable ...
🎚Volume:0.5 

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
