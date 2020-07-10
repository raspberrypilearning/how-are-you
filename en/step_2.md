If working **online**, open the [starter project](http://rpf.io/how-are-you-on){:target="_blank"} in Scratch.
 
If working **offline**, open the project [starter file](http://rpf.io/p/en/how-are-you-get){:target="_blank"} in the Scratch offline editor. If you need to download and install Scratch, you can find it [here](https://scratch.mit.edu/download){:target="_blank"}.

You should see two young people - one is you and the other is your friend. Click the green flag and you should see and hear one of the spirtes, speaking in Arabic.

## Translate your message

Think of the person you want to send your message to. We will call that person the 'respondent'. 

What language does the respondent speak?

--- task ---

In the `translate`{:class="block3extensions"} and  `say`{:class="block3looks"} blocks "Type your message here" is written. Type your own messages into each block.

```blocks3
when flag clicked
set voice to (tenor v) ::tts
+ translate [My own message] to (Arabic v) ::tts
+ say ( translate [My own message] to (Arabic v) ::tts ) for (4) seconds
```

--- /task ---

--- task ---

Choose the language you want to translate your message in to. It's currently set to Arabic.  There are 40 languages in Scratch to choose from!

```blocks3
when flag clicked
set voice to (tenor v) ::tts
+ translate [My own message] to (Czech v) ::tts
+ say ( translate [My own message] to (Czech v) ::tts ) for (4) seconds
```

--- /task ---

--- task ---

You may need to change the value of how long your message is shown for.

```blocks3
when flag clicked
set voice to [tenor v] ::tts
translate [My own message] to [Czech v] ::tts
+ say ( translate [My own message] to (Czech v) ::tts ) for (8) seconds
```
--- /task ---

--- task ---

If you like, change the voice so it sounds more like you.

```blocks3
when flag clicked
+ set voice to [squeak v] ::tts
translate [My own message] to [Czech v] ::tts
say ( translate [My own message] to (Czech v) ::tts ) for (8) seconds

```

--- /task ---

--- task ---

If you have used Scratch before, or want to try new things out, try changing the sprite's costume and the backdrop.

--- /task ---

## Respondent's reply

The respondent wants to reply to your message. Modify the program so they can message you back.

--- task ---

To do this, you will need to attach two extra lines of code to the **You** sprite. The blocks will let the respondent know that they can reply by clicking their sprite. 

+ Select the **You** sprite.
+ Go to `Looks`{:class="block3looks"} and select the `say`{:class="block3looks"} block. 
+ Got to `Text to Speech`{:class="block3extensions"} and add a `speak`{:class="block3extensions"} block underneath the `say`{:class="block3looks"} block. 
+ Got to Translate{:class="block3extensions"} and add a `translate`{:class="block3extensions"} into the both these new blocks. 
+ Type the following in to both blocks: "Reply by clicking the other sprite."


```blocks3
when flag clicked
set voice to [squeak v] ::tts
translate [My own message] to [Czech v] ::tts
say ( translate [My own message] to (Czech v) ::tts ) for (8) seconds
+ say (translate [Reply by clicking the other sprite] to (Czech v) ::tts) for (4) seconds [Reply by clicking the other sprite] to (Czech v) :tts
+ translate 

```
```blocks3
when this sprite clicked
set voice to (squeak v)
ask (translate [Type in your message here] to (Czech v)) and wait
+ say ( translate [Reply by clicking the other sprite.] to (Czech v) ::tts ) for (4) seconds
+ translate [Reply by clicking the other sprite.] to [Czech v] ::tts
```

+ Don't forget to select the respondent's language again.

--- /task ---

--- task ---

+ Now click on the **Respondent** sprite.

--- /task ---

--- task ---

+ Choose the language you are most familiar with - the program will translate the respondent's message so you can hear and read it.

```blocks3
when this sprite clicked
set voice to (squeak v)
ask (translate [Type in your message here] to (Czech v)) and wait
+ say ( translate [Reply by clicking the other sprite.] to (Czech v) ::tts ) for (4) seconds
+ translate [Reply by clicking the other sprite.] to [Czech v] ::tts
```

--- /task ---

--- save ---
