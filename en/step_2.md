**Online:** open the [starter project](http://rpf.io/how-are-you-on){:target="_blank"} in Scratch.
 
**Offline**: open the [project starter file](http://rpf.io/p/en/how-are-you-go){:target="_blank"} in the Scratch offline editor. If you need to, you can [download and install Scratch here](https://scratch.mit.edu/download){:target="_blank"}.

You should see two young people: one represents you, and the other represents your friend. Click on the green flag and you should see and hear one of the sprites speaking in Czech.

## Translate your message

Think of the person that you want to send your message to. We will call that person the **respondent**. 

--- task ---

Type your own message into both the `translate`{:class="block3extensions"} blocks.

```blocks3
when flag clicked
set voice to (tenor v) ::tts
+ speak (translate [type your own message here] to (Czech v) ::translate) ::tts
+ say ( translate [type your own message here] to (Czech v) ::translate ) for (4) seconds
```

--- /task ---

What language does the respondent speak?

--- task ---

Choose the language that you want to translate your message into. It is currently set to `Czech`{:class="block3extensions"}. There are 40 languages to choose from in Scratch!

```blocks3
when flag clicked
set voice to (tenor v) ::tts
+ speak (translate [My message] to (Czech v) ::translate) ::tts
+ say ( translate [My message] to (Czech v) ::translate ) for (4) seconds
```

--- /task ---

--- task ---

You may need to change the value of how many seconds your message is shown for. It should be shown for enough time for it to be read, but not so long that the reader gets bored waiting.

```blocks3
when flag clicked
set voice to [tenor v] ::tts
speak (translate [My message] to [Czech v] ::translate) ::tts
+ say ( translate [My message] to (Czech v) ::translate ) for (8) seconds
```
--- /task ---

--- task ---

If you like, change the voice so that it sounds more like you.

```blocks3
when flag clicked
+ set voice to [squeak v] ::tts
speak (translate [My message] to [Czech v] ::translate) ::tts
say ( translate [My message] to (Czech v) ::translate ) for (8) seconds
```

--- /task ---

--- task ---

If you have used Scratch before, or want to try new things, try to change the sprite's costume and the backdrop.

--- /task ---

## Receive a message back

The respondent wants to reply to your message. Modify the program so that they can send you a message back.

--- task ---

To do this, you will need to add a `broadcast message1`{:class="block3events"} block from the `Events`{:class="block3events"} blocks menu.

Add this new `broadcast message1`{:class="block3events"} block underneath the existing code.

```blocks3
when flag clicked
set voice to [squeak v] ::tts
speak (translate [My message] to (Czech v) ::translate) ::tts
say ( translate [My message] to (Czech v) ::translate ) for (8) seconds
+ broadcast (message1 v)
```

--- /task ---

--- task ---

Now, click on the **Respondent** sprite.

--- /task ---

--- task ---

Choose the language that you are most familiar with. The program will translate the respondent's message so that you can hear and read it.

```blocks3
when I receive [message1 v]
set voice to (squeak v) ::tts
ask (translate [Type in your message here] to (Czech v) ::translate) and wait
+ say ( translate (answer) to (English v) ::translate ) for (4) seconds
+ speak (translate (answer) to (English v) ::translate) ::tts
```

--- /task ---

--- save ---
