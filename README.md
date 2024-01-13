# Hackspace Badger Badge Layout

## What is it?
This repo stores the basic info and python code to push to the [Badger 2040][1]
It was written for the _old style_ badger but should still work with the newer versions 

Files contained in the repo:
- badge.txt - this contains the text to be displayed on the badge
- badge-image.bin - the binary form of the logo to display on the badge - in this the HS logo
- main.py - this is the code that displays date  on the badge
- README.md - this file


You can of course edit this to customise however you like! (More instructions on the [getting started][2] page)
This repo is just to allow you to quickly make a _hackspace_ badge, it also assumes you've already installed micro python on the badger, again go to the [getting started][2] page for how to do this

### badge.txt
The `badge.txt` file has the following layout
```
<Title> <-- This is displayed at the top of the badge screen
<Name> <-- This bit is the largest text section so it displays in the middle you don't have to put your name here but thats kinda standard 
<email> <-- the next section is split into two formatting sections , i've named them email and @emaildomain here
<@emaildomain> <-- but you can put what ever you like in it - social media tags for example
<free text> <-- the _free text_ sections work in a similar way - put what ever you like here
<free text2>

```

### badge-image.bin
This is just a monochrome image (on the badger2040 I have anyway) converted to a binary - one thing to note here - use a _small_ image (resolution wise)
otherwise you'll not get what you're expecting as an image when converting it - although i believe the later versions of the device can use straight up jpegs now! (although I don't have one of those to test with)

### main.py
The main.py is from the old example files of the original badger2040 project; as mentioned previously, it's in this repo to give you a somewhat drag and drop experience!


[1]: <https://pimoroni.com/badger2040> "Badger2040"
[2]: <https://learn.pimoroni.com/article/getting-started-with-badger-2040> "Getting Started"
