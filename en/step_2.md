## Translate your message

**Online:** open the [starter project](http://rpf.io/how-are-you-on){:target="_blank"} in Scratch.
 
**Offline**: open the [project starter file](http://rpf.io/p/en/how-are-you-go){:target="_blank"} in the Scratch offline editor. If you need to, you can [download and install Scratch here](https://scratch.mit.edu/download){:target="_blank"}.

You should see two young people: one represents you, and the other represents your friend. Click on the green flag and you should see and hear one of the sprites speaking in Czech.

Think of the person that you want to send your message to. We will call that person the **respondent**. 

--- task ---

Type your own message into both the `translate`{:class="block3extensions"} blocks where it says "My message". Leave the text "Type your reply in the box." so that the **respondent** will know what to do next.

```blocks3
when flag clicked
set voice to (tenor v) ::tts
+ speak (translate [My message. Type your reply in the box.] to (Czech v) ::translate) ::tts
+ say ( translate [My message. Type your reply in the box.] to (Czech v) ::translate ) for (4) seconds
```

--- /task ---

What language does the respondent speak?

--- task ---

Choose the language that you want to translate your message into. It is currently set to `Czech`{:class="block3extensions"}. There are 40 languages to choose from in Scratch!

```blocks3
when flag clicked
set voice to (tenor v) ::tts
+ speak (translate [My message. Type your reply in the box.] to (Czech v) ::translate) ::tts
+ say ( translate [My message. Type your reply in the box.] to (Czech v) ::translate ) for (4) seconds
```

--- /task ---

--- task ---

You may need to change the value of how many seconds your message is shown for. It should be shown for enough time for it to be read, but not so long that the reader gets bored waiting.

```blocks3
when flag clicked
set voice to [tenor v] ::tts
speak (translate [My message. Type your reply in the box.] to [Czech v] ::translate) ::tts
+ say ( translate [My message. Type your reply in the box.] to (Czech v) ::translate ) for (8) seconds
```
--- /task ---

--- task ---

If you like, change the voice so that it sounds more like you.

```blocks3
when flag clicked
+ set voice to [squeak v] ::tts
speak (translate [My message. Type your reply in the box.] to [Czech v] ::translate) ::tts
say ( translate [My message. Type your reply in the box.] to (Czech v) ::translate ) for (8) seconds
```

--- /task ---

--- task ---

If you have used Scratch before, or want to try new things, try to change the sprite's costume and the backdrop.

--- /task ---

## Receive a message back

The respondent wants to reply to your message. Modify the program so that they can send you a message back.

--- task ---


To do this, you need to add a `broadcast`{:class="block3events"} block from the `Events`{:class="block3events"} blocks menu to the program in the **You** sprite's **Code** tab. The `broadcast`{:class="block3events"} block will be used as a trigger in the **Respondent** sprite's program.

Join this new `broadcast message1`{:class="block3events"} block underneath the existing code.

```blocks3
when flag clicked
set voice to [squeak v] ::tts
speak (translate [My message. Type your reply in the box.] to (Czech v) ::translate) ::tts
say ( translate [My message. Type your reply in the box.] to (Czech v) ::translate ) for (8) seconds
+ broadcast (message1 v)
```

--- /task ---

--- task ---

Now, click on the **Respondent** sprite.

--- /task ---

--- task ---

When the **Respondent** sprite receives `message1`{:class="block3events"} from the `broadcast message1`{:class="block3events"} block in the **You** sprite's program, it triggers the **Respondent** sprite's program to start, with the `when I receive`{:class="block3events"} block.

Select an `ask`{:class="block3sensing"} block so that the respondent can reply. Choose the language that the respondent is most familiar with. Check that the program will then translate the respondent's message into your chosen language so that you can both read and hear it. You may need to change the number of seconds in the `say`{:class="block3looks"} block, depending on the length of the message.


```blocks3
when I receive [message1 v]
set voice to (alto v) ::tts
+ ask (translate [] to (Czech v) ::translate) and wait
+ say ( translate (answer) to (English v) ::translate ) for (4) seconds
speak (translate (answer) to (English v) ::translate) ::tts
```

--- /task ---

--- save ---
