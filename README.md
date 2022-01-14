# Number-of-squares-with-N-random-points

In the beginning, I generated random points in a plane and used a dynamic programming idea that in the way that we should fix two points (X1, Y 1) and (X2, Y2), and iterate all pairs of fixed points and rotate the deference vector by 90 to obtain two other points of the square by the following equations. 
X3 = X1 + (Y2 − Y1) 
X4 = X2 + (Y2 − Y1) 
Y3 = Y1 + (X1 − X2) 
Y4 = Y2 + (X1 − X2) 
It would be notable that the time complexity of this idea is around O(n^4); therefore, I sorted points at the start of the algorithm using the dictionary. This simple point decreases the time complexity to O(n^2).
Firstly, I ran the code for nine fixed points to check the results’ truth. Next, I generated N random numbers and ran the code at the plant. As the results showed,
there is five possible square for the following fixed points:
(0, 0),(2, 2),(0, 2),(2, 0),(4, 2),(4, 0),(2, 4),(0, 4),(4, 4) 
Additionally, the program computed that There are 29 possible squares for 50 generated random points (visible at the python code)
