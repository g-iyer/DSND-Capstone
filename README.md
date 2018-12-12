					# DSND-Capstone
<Holds files and other artifacts for the DSND Capstone project>

Hello and Welcome to my project - ''Robot Motion Planning'' - for the capstone of Udacity's Data Science Nanodegree program

## Executive Summary ##

For my capstone project I decided to use the Robot Motion Planning project. This project is about developing a virtual robot 
that will navigate a virtual maze utilizing different methods.

It is inspired by the micromouse competition popularized by IEEE – for a very interesting article please see this link [The Amazing MicroMouse  Contest](http://spectrum.ieee.org/consumer-electronics/gadgets/the-amazing-micromouse-contest "The Amazing MicroMouse  Contest").

In this project except for the maze dimensions nothing else is known. So the robot has to _first explore and then exploit_ the maze.
The objective is for the robot to reach the goal i.e., the center of the maze, using the best possible algorithm in the best possible time. 

Three *maze definition files* are given. The solution needs to apply different methods of navigation to reach the center of these mazes. 
A *tester* program is provided (from the *starter code* set) that applies the solution to solve a given maze and reports the score at the end.
The navigation method with the lowest score would be the best solution.

I have created the solution to search using multiple popular algorithms 
	– Follow the Wall, Breadth First Search, Depth First Search, Uniform Cost Search, A* (aka A Star) search and the Flood Fill search. 
	
All these methods are well documented on the Internet as the micromouse problem has been extensively researched.	

This report details the approach, the methodology and the results. 

**The conclusion is that the __Flood Fill method__ is the best algorithm to solve the navigation of a maze effectively.**


## Project Definition ##
The project relates to the domain of robot localization and movement planning. It is necessary for a robot to know its position in a real or virtual world situation, decide on the action to take and then complete the action – while considering the goal at all times. This problem is common across all mobile robots – be it a competition robot or a self-driving car or lunar rovers! This area has been of interest since the DARPA grand challenges that motivated the development of cars that could navigate open land routes. 
The core idea of this project is based on the popular maze solving competition for robots –  the Micromouse (wikipedia description) competition. I have also come across the Trinity College Firefighting Robot competition where a robot must find a room in a home (a maze) with an open fire and extinguish it in the shortest possible time. Trinity College competition references: ( Tufts University description ) (Rules of the competition).
	In both competitions, the robot has to locate a goal (either the center of the maze or a lit candle) in the shortest possible time and consistently over multiple trials. The robot depends on sensor readings – the sensors can be touch, IR, SONAR, LIDAR and/or on-board cameras. Due to the limited size of the robots the level of hardware was limited as no off-board computing is allowed. With the introduction very powerful MCUs and integrated SBCs like arduinos and Raspberry PIs the current robots have become very powerful in computing. 
	From these beginnings, one can go on to other areas such as non-maze navigation and real world mobility. Studying and solving this problem of navigating a virtual maze builds a very good foundation for further explorations. 
	
### Problem Statement ###

### Metrics ###

## Analysis ##

### Data Exploration ###

#### Datasets and inputs ###


![test_maze_01.txt](/images/test_maze_01_txt.jpg)

## Implementation ##

### Files ###

[link to AI Starter code](https://docs.google.com/document/d/1ZFCH6jS3A5At7_v5IUM5OpAXJYiutFuSIjTzV_E-vdE/pub) - 
**Pplease note that this code is not in Python 3.+ . I have updated the files and posted them to this repository**
*You must use the files from this repository - not from the starter code zip file*

### Files ###
1. Files included 
	tester.py		supplied - to test the robot and provide scores for succesful runs 
	maze.py			supplied - creating and managing the maze for tester.py
	showmaze.py		supplied - standalone to print maze using turtle
	
	robot.py		supplied and modified to select algorithm and interface with tester.py
	maze_managment.py	Maze related functions implemented
	flood_fill.py		Flood Fill algorithm
	graph_search.py		Search algorithms including BFS, DFS, UC and A*
	follow_wall.py		Follow Wall algorithm
	
	util.py			Graph search utilities file form UC Berkley CS188 course website
	
	options.txt		Search method options (please see instructions below)
	
	/doc			folder with documentation files
		Navigate-Virtual-Maze-Project-Report.pdf		Project report
		Robot-motion-project-proposal-rev1.pdf			Project proposal - link to review https://review.udacity.com/#!/reviews/446660
		navigate-maze-trials.xlsx				Run results
		A-Star-sample-run.txt					Console output of A Star search
		Flood-fill-sample-run.txt				Console output of Flood Fill search
		
		test_maze_**.jpg					screen shot files of mazes
2. Operating instructions
	2.A	Edit the options.txt file with one of these 6 values (enter ONLY the text in quotes)
		"WF"	- Follow Wall 
		"BF"	- Breadth First
		"DF"	- Depth First
		"UC"	- Uniform Cost
		"ASTAR"	- A Star
		"FF"	- Flood Fill
	2.B	The trial is executed by this command - replace xx with 01, 02 or 03 as required.
		python tester.py test_maze_xx.txt







## Refinement ##

## Results ##

## Conclusion ##
