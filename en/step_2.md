If working **online**, open the [starter project](http://rpf.io/how-are-you-on){:target="_blank"} in Scratch.
 
If working **offline**, open the project [starter file](http://rpf.io/p/en/how-are-you-get){:target="_blank"} in the Scratch offline editor. If you need to download and install Scratch, you can find it [here](https://scratch.mit.edu/download){:target="_blank"}.

You should see a young person - that's you (for now!). Click the green flag to run the project. Read on to find out what you are saying in Arabic.

<div>
<iframe src="https://scratch.mit.edu/projects/399133454/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

## Translate your message

Think of the person you want to send your message to. We will call that person the 'respondent'. 

What language does the respondent speak?

--- task ---

+ Open the code editor. Currently in the `say`{:class="block3looks"} block "Type your message here" is written. Delete this message and type in your own message.

+ Choose the language you want to translate your message in to. It's currently set to Arabic.  There are 40 languages in Scratch to choose from!

```blocks3
when flag clicked
set voice to [tenor v] ::tts
(translate [Type your message here] to [Arabic v] ::translate) ::tts
say ( translate [Type your message here] to (Arabic v) ::translate ) for (4) seconds
```

Notice you need to select the language twice and paste your message in twice in order to create both spoken and written translation.

+ You may need to change the value of how long your message is shown for.

```blocks3
when flag clicked
set voice to [tenor v] ::tts
(translate [Type your message here] to [Arabic v] ::translate) ::tts
+ say ( translate [Type your message here] to (Arabic v) ::translate ) for (8) seconds
```

+ If you like, change the tone of the voice so it represents you.

```blocks3
when flag clicked
+ set voice to [squeak v] ::tts
(translate [Type your message here] to [Arabic v] ::translate) ::tts
+ say ( translate [Type your message here] to (Arabic v) ::translate ) for (8) seconds
```

--- /task ---

--- task ---

If you have used Scratch before, or want to try new things out, try changing the sprite or the backdrop.

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

+ Now click on the **Respondent** sprite.

--- /task ---

--- task ---

+ In the program, change the language option - see the blocks highlighted in black below. Choose the language you are most familiar with - the program will translate the respondent's message so you can hear and read it.

```blocks3
when this sprite clicked
set voice to [squeak v] ::tts
ask ((translate [Type in your reply here.] to [Arabic v] ::translate) ::tts) and wait
+say ( translate (answer) to (English v) ::translate ) for (2) seconds
+(translate (answer) to [English v] ::translate) ::tts
```

--- /task ---

--- save ---
