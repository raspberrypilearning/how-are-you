
## Challenge: Receive a message back
The respondent wants to reply to your message. Modify the program so they can message you back.

--- task ---

+ To do this, you will need to attach two extra blocks of code to sprite 'You'. The blocks will let the respondent know that they can reply by clicking their sprite (which we've yet to make appear). 

+ Select sprite 'You' and attach the `say`{:class="block3looks"} and `translate`{:class="block3extensions"} blocks.

```blocks3
say ( translate [Please answer by clicking the character.] to (Arabic v) ::translate ) for (4) seconds
(translate [Please answer by clicking the character.] to [Arabic v] ::translate) ::tts
```
+ Don't forget to select the respondent's language again.

--- /task ---

--- task ---
+ Now select the sprite 'Respondent'.

+ To see the Respondent, you also need to switch their show 'eye' on.
!['Respondent' sprite](images/show-Respondent.png)

+ In the code area, change the language option. Choose the language you are most familiar with - the program will translate the respondent's message so you can hear and read it.
```blocks3
when this sprite clicked
set voice to [squeak v] ::tts
ask ((translate [Type in your reply here.] to [Arabic v] ::translate) ::tts) and wait
say ( translate (answer) to (English v) ::translate ) for (2) seconds
(translate (answer)  to [English v] ::translate) ::tts
```
--- /task ---

--- task ---

+ Change the look of the sprite 'Respondent' so it looks more like the Respondent i.e. your family member, friend or peer. Select the sprite, click on the Costumes tab and select one of the available costumes to represents them.
!['Respondent' sprite](images/choose-Respondent-costume.png)

--- /task ---

--- task ---

+ Run the program again. Is it working as you want it to? If so, why not try it out on a friend or family member? Share the project link or search for [How are you?](https://rpf.io/how-are-you-on) project.

--- /task ---
