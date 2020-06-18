**Online**: Open the 'How are you?' starter Scratch project [online](http://rpf.io/how-are-you-on){:target="_blank"}.  If you have a Scratch account you can make a copy by clicking **Remix**.

If you are working offline, you will need the Scratch software installed from [rpf.io/scratch-off](https://rpf.io/scratch-off){:target="_blank"}. You can then download the Starter project at [rpf.io/p/en/how-are-you-go](https://rpf.io/p/en/how-are-you-go).

You should see a young person - that's you (for now!). Click the green flag to run the project. Read on to find out what you are saying in Arabic.

<div>
<iframe src="https://scratch.mit.edu/projects/399133454/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

## Translate your message

Think of the person you want to send your message to. We will call that person the 'respondent'. 

What language does the respondent speak?

--- task ---

+ Open the code editor. Currently in the `say`{:class="block3looks"} block you say "Type your message here". Delete the message that is there and type in your own personal message.

+ Choose the respondent's language, i.e. the language you want to translate your message in to. It's currently set to Arabic.  There are 40 languages in Scratch to choose from! Let's hope the language the respondent speaks is included in those 40.
```blocks3
when flag clicked
set voice to [tenor v] ::tts
(translate [Type your message here] to [Arabic v] ::translate) ::tts
say ( translate [Type your message here] to (Arabic v) ::translate ) for (4) seconds
```
Notice you need to select the language twice and paste your message in twice in order to create both spoken and written translation.

+ If your message is long, you may need to change the value of how long your message is shown for. Try to run the program again to check if the timing fits.
```blocks3
say ( translate [Type your message here] to (Arabic v) ::translate ) for (4) seconds
```
+ If you like, change the tone of the voice so it  represents you.
```blocks3
set voice to [tenor v] ::tts
```
--- /task ---

## Change your sprite

![Access You](images/you.png){:width="100px"}

As the message is from you, choose a sprite costume to represent you. It will then appear that you’re the one speaking and typing the message!

--- task ---
+ Go to **Costumes**. Select one of the ten costumes available by clicking on it. Your costume will become highlighted and your sprite will automatically change to that costume on the stage.

+ Run the program to see and hear yourself speaking another langauge. Impressive!

![Access Costumes](images/costumes.png){:width="350px"}

--- /task ---
## Choose a Backdrop
--- task ---

+ The current backdrop is little too plain! Why not choose a different one? Go to **Choose a Backdrop**. There are loads in the gallery to choose from.

![Access Choose a Backdrop](images/choose-a-backdrop.png){:width="350px"}

--- /task ---

## Respondent's reply

The respondent wants to reply to your message. Modify the program so they can message you back.

--- task ---

+ To do this, you will need to attach two extra lines of code to the **You** sprite. The blocks will let the respondent know that they can reply by clicking their sprite (which we've yet to make appear). 

+ Select the **You** sprite.
+ Go to `Looks`{:class="block3looks"} and select the `say`{:class="block3looks"} block. 
+ Got to `Text to Speech`{:class="block3looks"} and add a `speak`{:class="block3extensions"} block underneath the `say`{:class="block3looks"} block. 
+ Got to Translate{:class="block3extensions"} and add a rounded `translate`{:class="block3extensions"} into the text field of both these new blocks. 
+ Type the following in to both blocks: "Reply by clicking the other sprite."

```blocks3
say ( translate [Reply by clicking the other sprite.] to (Arabic v) ::translate ) for (4) seconds
(translate [Reply by clicking the other sprite.] to [Arabic v] ::translate) ::tts
```
+ Don't forget to select the respondent's language again. It's currently set to Arabic.

--- /task ---

--- task ---
+ Now select the **Respondent** sprite.

+ To see the **Respondent** sprite, you also need to switch their show **eye** on.
!['Respondent' sprite](images/show-respondent.png){:width="350px"}

+ In the program, change the language option - see the blocks highlighted in black below. Choose the language you are most familiar with - the program will translate the respondent's message so you can hear and read it.
```blocks3
when this sprite clicked
set voice to [squeak v] ::tts
ask ((translate [Type in your reply here.] to [Arabic v] ::translate) ::tts) and wait
+say ( translate (answer) to (English v) ::translate ) for (2) seconds
+(translate (answer) to [English v] ::translate) ::tts
```
--- /task ---

--- task ---

+ Change the look of the **Respondent** sprite so it looks more like the respondent i.e. the family member, friend or peer you are sending the mesage tp. Select the sprite, click on the **Costumes** tab and select one of the available costumes to represents them.

!['Respondent' sprite](images/choose-respondent-costume.png){:width="400px"}

--- /task ---

--- task ---

+ Run the program again. Is it working as you want it to?

--- /task ---

--- save ---
