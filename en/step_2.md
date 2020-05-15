**Online**: Open the 'How are you?' starter Scratch project online at [rpf.io/how-are-you-on](https://scratch.mit.edu/projects/394360639){:target="_blank"}

If you have a Scratch account you can make a copy by clicking **Remix**.

You should see a little yellow dot on a white background. We really need you to jazz things up! 

Click the green flag to run the project. It will sound and read like double-dutch! It is infact Arabic. Read on to find out  what's being said.

<div>
<iframe src="https://scratch.mit.edu/projects/395701995/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

## Translate your message

Think of the person you want to send your message to. We will call that person the 'respondent'. 

What langauge does the respondent speak?

--- task ---

+ Open the code editor. The current message says "How are things going in Palenstine?". Delete the message that is there and type in your message.

--- /task ---

--- task ---

+ Choose the respondent's language i.e. the language you want to translate your message in to. There are 40 languages in Scratch to choose from! Let's hope the language the respondent speaks is included in those 40.
--- /task ---
```blocks3
when flag clicked
set voice to [tenor v] ::tts
(translate [How are things going in Palenstine?] to [Arabic v] ::translate) ::tts
say ( translate [How are things going in Palenstine?] to (Arabic v) ::translate ) for (4) seconds
```
Notice you need to select the language twice and paste your message in twice in order to create both spoken and written translation.

--- task ---

+ If your message is long, you may need to change the value of how long your message is shown for. Why not run the program again to check if the timing fits.
```blocks3
say ( translate [How are things going in Palenstine?] to (Arabic v) ::translate ) for (4) seconds
```
+ If you like, change the tone of the voice so it  represents you.
```blocks3
set voice to [tenor v] ::tts
```
--- /task ---

## Take a selfie

![Access Stage](images/you.png)

As the message is from you, why not make sure the sprite looks a bit like you as well so it appears that you’re the one speaking and typing the message.

--- task ---
+ Go to Costumes. Select by highlighting one of the ten cosutmes listed.

![Access Stage](images/Costumes.png)

+ Select 'Choose a Backdrop'. Then select Camera and Take a Photo.

![Access Camera](images/Choose-a-Backdrop-Camera.png)

--- /task ---

Run the program to see if the callout looks like you are speaking.

--- task ---

+ Adjust the position of callout by dragging the little yellow dot to the centre of your mouth.

+ Run the program again. Do you need to adjust the little yellow dot again?

--- /task ---

## Nine more to go!

In this project you experienced two Scratch Extension Blocks: Translate and Text to Speech. There are another nine more to get to know! Why not begin to explore them? 

![Extension Blocks tab](images/extension-blocks.png)


--- save ---
