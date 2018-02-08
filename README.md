# A 3-part tutorial on automating everyday content conversion tasks with Tesseract, Automator, Python, and Twee2

Let's just say I've been meaning to pull this together for awhile and just didn't find the time until now. It'll move pretty quickly so you're encouraged to send questions and feedback to jc at abovethecurve dot io. 

Shall we?
***

## Part 1: Convince yourself that monkeywork is best left to simians.

How many times have you been asked to just "throw together" an e-learning module from some Powerpoints or a hardbound manual. The assumption, good or bad, is that since the content is already there, that putting it into a different format should be pretty effortless. Yeah right.

But you say "sure boss" and get to the braindeadening task of rekeying the content into a webpage or some digital format, by basically retyping what's in one form into one that more closely matches your solution. Shoot me now.

This is one of those moments where being extremely lazy will in the end pay off, and, may even scale alot better and faster.

So say we've got a hard copy of a PDF file. Why a hard copy? Because, per usual, the digital copy is nowhere to be found. Whatev.

**Step 1** is to scan the hardcopy and save it as a PDF file. We're most interested in NOT having to retype any text from the hardcopy into our solution, so on the scan's properties we'll want at least **300 dpi** and the **lowest compression** set for the scan job. If you like to wing through tutorials, just keep track of what you named your scanned file. If you want to keep in step with the tutorial, name your scanned file `ingest.pdf`. If you don't have a scanner, you could alternatively take a picture of each page of the hardcopy, but that starts to get pretty bananas, knowwhatimsayn?

**Step 2** is to set up an Automator workflow or application. I'm not going to go into the details on how to do that and just share this guy's [video](https://www.youtube.com/watch?v=UwTg-ECwVls) tutorial instead. What you want the Automator to do is convert your scanned PDF file into a JPEG or other image file. 

You might be asking your self at this point: why not just extract the text from the *scanned PDF file*? The Automator has a task that does just that. Why go through the trouble of converting the PDF into a JPEG file? 

We'll wait here while you try that out...

Done? OK. Make sure to specify where to move the image file or else Automator will bury deep deep in the directory structure. Also, if you're following along, name the file `extractme.jpeg`.

**Step 3** is to use Tesseract to extract the text from your image file and put it into a TXT file. Like with Step 2, there's plenty of good tutorials out there on how to install and use Tesseract. But if you absolutely can't Google, try this [one](https://www.youtube.com/watch?v=QhJiOCwz-_I) out. Try playing around with the page segmentation modes in Tessearct for non-standard text layouts.

## Part 2: Trick yourself into believing this is the way it should have always been.

to be continued...

