# Numerical-Updating
Website built in javascript using the jsPsych library to test memory in a numerical updating task. A running example of the most recent version of this script can be found here: https://g3ihsqn6sb.cognition.run/?sequence=Demo

This script was developed in jsPsych 6.1, which can be downloaded here: https://github.com/jspsych/jsPsych/releases/tag/v6.1.0 . It probably works with newer versions of jsPsych, but I haven't tested it.

If you want to run this program locally you will need to run a local web server so the GET request for the sequence json file is not blocked. I use the Web Server For Chrome app for debugging purposes, but you may want to do some research and decide what works best for you. When testing participants, we use a version of this program hosted on cognition.run

Once you have downloaded jsPsych, the NumericalUpdating.html file, and the Demo.json expeirmental sequence, you can open the website in a web browser through your server and it should bring up the task instructions.

This script implements a numerical updating task as described by Wilhelm et al. (2013, Frontiers in Psych). Each trial presents between digits sequentially in a series of boxes, as defined in the experimental sequence file, with each digit presented for 1600 ms and no time between digits. The goal is to remember the _last_ number shown in each box and then type those digits in each box when prompted. Each trial is defined in the json file as an array of arrays. Each inner array corresponding to the text shown at each time step, and the outer array defines the sequence in which those steps should be shown.  The length of the inner arrays should be fixed within each trial, and is used to determine how many boxes to render on screen. We will share the full experimental sequence and scripts for scoring data on request (adam.bosen@boystown.org).
