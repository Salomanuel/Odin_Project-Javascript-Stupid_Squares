# stupid-squares

old one:
http://htmlpreview.github.io/?https://github.com/Salomanuel/stupid-squares/blob/master/prova3%20backup1.html

updated and fancy one:
http://htmlpreview.github.io/?https://github.com/Salomanuel/stupid-squares/blob/master/prova3.html

Project: Javascript/jQuery

In this project, you'll get a chance to actually build a pretty nifty tool to flex your Javascript and jQuery muscles. Up until now, you've had your hand held quite a bit by Codecademy. Now it's time to do it on your own. You're going to build a browser version of something between a sketchpad and an Etch-A-Sketch.

This should NOT be trivially easy for you. You'll probably have to Google frequently to get the right jQuery methods or CSS to use. In fact, that's the point! You CAN build this, and the resources are out there. We'll walk through the basic steps but it'll be up to you to find out how to actually implement them. For instance, where does a hover effect come from?

The key is to break it down into little manageable steps and then figure out how to solve each step in turn.

If you get totally stuck, solutions from other students are listed below. I'd encourage you to struggle for a bit on your own before checking them out.

    Follow the instructions atop the Google Homepage project to set up a Github repository for this project (of course you'll need to change the title).
    Create a web page (or use JSFiddle) with a 16x16 grid of square divs.
        Create your divs using Javascript/jQuery... don't try making them by hand with copy-pasting!
        Best to put your grid squares inside another "container" div.
        If you need to add jQuery to your file, you can grab it directly in your HTML by adding <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script> inside your <head> tag above any other JS files.
        There are several different ways to make the divs appear as a grid (versus just one on each line) -- float/clear, using a table, and inline-block displays. Play with each of them.
        Careful with your border or margins... they'll add size to the squares!
        "OMFG, Why isn't my grid being created???"
            Open your browser's developer tools
            Check if there are any errors in the Javascript console
            Check your "elements" pane to see if the elements have actually shown up but are somehow hidden.
            Go willy-nilly and add console.log statements in your javascript to see if it's actually being loaded.
    Set up a hover effect so it changes the color of the square when your mouse passes over it, leaving a (pixelated) trail through your grid like a pen would.
        What happens when you hover? Well, you're hovering, you need to enter the div with your mouse and you need to leave the div. Any of those events should be a useful place to start.
        There are again several ways to change the color -- adding a new class (addClass()), changing that div's background color individually, etc.
    Add a button to the top of the screen which will clear the current grid and send the user a popup asking for how many squares per side to make the new grid. Once entered, the new grid should be generated in the same total space as before (e.g. 960px wide) and now you've got a new sketch pad.
        Research button tags in HTML and how you can make a javascript function run when one is clicked.
        You'll also want to check out prompts.
        You should be able to enter 64 and have a new 64x64 grid pop up in front of you without changing the total amount of pixels used.
        Why is it so slow?? Remember that when you call a jQuery selector like $(".square"), it actually returns you ALL the elements that fit the description. So if you're doing those types of operations hundreds of times inside a loop, it can get very time consuming... try pulling those outside your loops.
        See how many grid squares you can get before it becomes unusably slow.
    (Optional): Instead of just changing the color of your grid from black to white (for example), have each pass through it with the mouse change to a completely random RGB value. Then try having each pass just add another 10% of black to it, so only after 10 passes is the square completely black.
    Push your project to Github
