Name - Navaneeth Thekkumpat

UTA ID - 1001656413

Programming Language used: Java

How the code is structured.
			-Programmed in Java.
			-The find_route class contains the following 
				1)main method 2)class inputnode 3)method addlist 4)method route 
			1) main method
				-I stored the input and heuristic files to the arraylists.
				-Each source destination names in the input file is considered bidirectional.
				-Fringe list is sorted using the compareTo method in the class inputnode which implements Comparable.
				-Once the backtracking is done, the Route is displayed with distance between the places displayed.
			2)class inputnode
				-I made a class with node,parentnode and distance as members.
				-For sorting the objects of fringe linkedlist of the class defined, used the compareTo() method
				-The LinkedLists of this class is used to store the fringe and closed elements.
			3)method addlist
				-Uninformed search is implemented using uniform cost search technique.
				-Elements are added to the fringes.
				-Elements expanded are added to the visited list and closed list.
				-Informed search is implemented using A* algorithm technique,
			 	 leading lesser nodes expanded than the uniform cost search technique.	
			4)method route 
				-Finding the route from the start to the destination along with the distances.
				-Fetching the distance once, the destination is found from the closed linkedlist.
				 I have backtracked the nodes in the path.  	

Files		   :	-Submited a ZIPPED directory called assignment1_nxt6413.zip in the blackboard. 
			-This zip directory includes find_route.java and readme.txt files.

How to run the code: 	1)Compile the find_route.java using the following command
				javac find_route.java
		    	2)Run the file using the following command
				java find_route <inf/uninf> input_filename sourcecity destinationcity <heuristicfilename>
				Eg:
				- java find_route uninf input.txt Bremen Kassel 
				Or
				- java find_route inf input.txt Bremen Kassel h_kassel.txt

			NOTE PLEASE ADD THE INPUT AND HEURISTIC FILES(.txt) in the same directory.	

References	   : 	1)For fetching the files and putting into the list, used the implementations from the following links
		     	- http://www.avajava.com/tutorials/lessons/how-do-i-read-a-string-from-a-file-line-by-line.html 
			
			2)For sorting the objects of fringe linkedlist of the class defined, used only the compareTo() method implementation 
			  specified in the below link
			- https://dzone.com/articles/how-to-sort-objects-in-java




