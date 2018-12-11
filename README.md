					# DSND-Capstone
<Holds files and other artifacts for the DSND Capstone project>

Hello and Welcome to my project - ''Robot Motion Planning'' - for the capstone of Udacity's Data Science Nanodegree program

## Executive Summary ##

This project is about developing a virtual robot that will navigate a virtual maze utilizing different methods.

It is inspired by the micromouse competition popularized by IEEE – for a very interesting article please see this link [The Amazing MicroMouse  Contest](http://spectrum.ieee.org/consumer-electronics/gadgets/the-amazing-micromouse-contest "The Amazing MicroMouse  Contest").

In this project except for the maze dimensions nothing else is known. So the robot has to first explore and then exploit the maze.

The objective is for the robot to reach the goal i.e., the center of the maze, using the best possible algorithm in the best possible time. 

Three maze definition files are given. The solution needs to apply different methods of navigation to reach the center of these mazes. 

A tester program is provided (from the starter code set) that applies the solution to solve a given maze and reports the score at the end.

The method with the lowest score would be the best solution.

I have created the solution to search using multiple popular algorithms 
	– Follow the Wall, Breadth First Search, Depth First Search, Uniform Cost Search, A* (aka A Star) search and the Flood Fill search. 
	
All these methods are well documented on the Internet as the micromouse problem has been extensively researched.	

This report details the approach, the methodology and the results. 

**The conclusion is that the __Flood Fill method__ is the best algorithm to solve the navigation of a maze effectively.**


## Project Definition##
The project relates to the domain of robot localization and movement planning. It is necessary for a robot to know its position in a real or virtual world situation, decide on the action to take and then complete the action – while considering the goal at all times. This problem is common across all mobile robots – be it a competition robot or a self-driving car or lunar rovers! This area has been of interest since the DARPA grand challenges that motivated the development of cars that could navigate open land routes. 
The core idea of this project is based on the popular maze solving competition for robots –  the Micromouse (wikipedia description) competition. I have also come across the Trinity College Firefighting Robot competition where a robot must find a room in a home (a maze) with an open fire and extinguish it in the shortest possible time. Trinity College competition references: ( Tufts University description ) (Rules of the competition).
	In both competitions, the robot has to locate a goal (either the center of the maze or a lit candle) in the shortest possible time and consistently over multiple trials. The robot depends on sensor readings – the sensors can be touch, IR, SONAR, LIDAR and/or on-board cameras. Due to the limited size of the robots the level of hardware was limited as no off-board computing is allowed. With the introduction very powerful MCUs and integrated SBCs like arduinos and Raspberry PIs the current robots have become very powerful in computing. 
	From these beginnings, one can go on to other areas such as non-maze navigation and real world mobility. Studying and solving this problem of navigating a virtual maze builds a very good foundation for further explorations. 
	
### Problem Statement ###

### Metrics ###

## Analysis ##

### Data Exploration ###

## Implementation ##
## Refinnement ##

## Results ##

## Conclusion ##
