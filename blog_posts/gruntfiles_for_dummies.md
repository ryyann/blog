## Don't repeat yourself - Workflow edition
If you've ever worked a project larger than a three page static website you've probably found that you repeating the same steps over and over. Maybe that means copying a file to another directory again and again, maybe it measns typing `sass *** ENTER COMMAND HERE *** ` into your terminal over and over, maybe that means refreshing your browser window whenever you make a change to a file. Doing the same thing over and over, even if it only takes a few seconds, can add up to a ton of wasted time. Stop wasting your time. Use a Gruntfile!

## Use a whatfile?
Use a Gruntfile! It's a little piece of Javascript that you use with a program called Grunt, which is built on the Node.js platform. Does that sound really confusing? Don't worry, you don't have to pay attention to too much. Just follow the bouncing ball: 

If you don't have Node.js, first [get it here](https://nodejs.org/) and install the package that's on the front page.

In your terminal window (`⌘spacebar` and then type `terminal` and hit `return`), type:

```
npm install -g grunt grunt-cli
```

If this gives you an error message, try this instead (you'll need to enter your admin password):

```
sudo npm install -g grunt grunt-cli
```

#### Okay, let's write it!
Great! you're ready to start writing the file. In your favourite text editor (I really like [Sublime](https://www.sublimetext.com)), save a new folder to the directory you're working in called Gruntfile.js.