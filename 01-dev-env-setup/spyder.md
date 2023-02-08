# Spyder Setup

<img src="../assets/images/spyder-logo-1.png" />

## Overview

We will now run out python program from within Spyder.  What is Spyder?

Spyder stands for Scientific Python Development Environment.

If you have anaconda, it should already be installed. If not, you can download and
install it from the website.

## Step-1: Install Spyder

You will need anaconda environment.

```bash
$   conda install spyder
```

You can also install it from Anaconda UI.

For more detailed instructions see [here](https://docs.spyder-ide.org/current/installation.html)

## Step-2: Start Spyder

Spyder is conveniently located in your Anaconda Navigator. Windows users can access this from the start menu.  

```bash
$   spyder
```

## Step-3: Load file

You will have use Spyder to load the file. Spyder will probably open up in your home directory.  Where is
that?  Well, it depends on your platform:

 * Windows: "C:\Users\YOURUSERNAME\"
 * Mac: "/Users/YOURUSERNAME/"
 * Linux "/home/yourusername/"

You then should naviagate to where you cloned this repo. Find this directory ("python-labs/01-helloworld/"), and then load your `helloworld.py` into spyder.

## Step-4: Run your code

You should be able to run your code using the green "Play" button on the toolbar.

When it runs, notice your varialbes a,b, and c appear on the right hand side. Those show up because they
are currently in scope.

## Step-5: Set a Breakpoint

Select a line of code (for example, the a = 10 line).

Use the menu to set a breakpoint.  It is located at Debug -> Set/Clear Breakpoint. You can also say F12.

## Step-6: Run Debug

Now go to the menu Debug -> Debug.

You should see your code stop at the breakpoint.

## Step-7: Console

Click over at the console, which should be on the lower right hand side ofhte screen.

Try evaluating some python code with your variables

```python
a
b 
```

## Step-8: Step

Go ahead and step through your code. You can do this by Debug -> Step.  

Watch the results of "a" change in the upper right hand corner.
