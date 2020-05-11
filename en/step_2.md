**Online**: Open the 'How are you?' starter Scratch project online at [rpf.io/how-are-you-on]. (http://rpf.io/how-are-you-on {:target="_blank"}

If you have a Scratch account you can make a copy by clicking Remix.

Offline: open the starter project in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at ?

You should see a little yellow dot on a white background. We really need you to jazz things up! Click the green flag to run  the starter project.

<div>
<iframe src="https://scratch.mit.edu/projects/390185573/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

## Translate your message

Think of the person you want to send your message to. We will call that person the 'respondent'. 

What langauge does the respondent speak?

--- task ---

+ Choose the respondent's language i.e. the langaue you want to translate your message in to. There are 40 languages in Scratch to choose from! Let's hope the language the respondent speaks is included in those 40.

--- /task ---

--- task ---

+ Open the code editor and delete the message that is there. Type in your message.

+ Notice you need to select the language twice and paste your message in twice in order to create both spoken and written translation.

```blocks3
when flag clicked
set voice to [tenor v] ::tts
(translate [How are things going in Palenstine?] to [Arabic v] ::translate) ::tts
say ( translate [How are things going in Palenstine?] to (Arabic v) ::translate ) for (4) seconds
```
--- /task ---

--- task ---

+ If your message is long, you may need to change the value of how long your message is shown for.
```blocks3
say ( translate [How are things going in Palenstine?] to (Arabic v) ::translate ) for (4) seconds
```

+ If you like, change the tone of the voice so it  represents you.
```blocks3
set voice to [tenor v] ::tts
```
--- /task ---

## Take a selfie

+ As the message is from you, why not take a selfie so that it looks like you’re the one speaking and typing the message?

--- task ---
+ Go to Stage. Select the Backdrop tab.

![Access Stage](images/stage.png)

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
