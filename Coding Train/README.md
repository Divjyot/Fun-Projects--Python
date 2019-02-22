# Approximation of Pi
##### First 10 digits of Pi are 3.1415926535 
###### First million digits, please check https://www.piday.org/million/  .... Well, yes that esclated quickly



I set out to python and found this https://www.youtube.com/watch?v=5cNnf_7e92Q which is one the fun tutorials from The Coding Train.

Current program approximates upto two decimal digits with 1000 runs.
Idea is to have a circle with r radius and  a square of side 2r which emcompass the circle as seen in the figure :

![alt text](https://github.com/Divjyot/Fun-Projects--Python/blob/master/Coding%20Train/SquareCircle.png) 

Now let say we are throwing darts (the number of darts is important for later, keep in mind) at this and some of the darts land IN the circle : cIN ( lets ignore the ones that land ON the circle circumference for the the moment) and some land IN the sqaure but outside the circle. Let suppose the total number of darts thrown are sIN.

Now the ratio in this case can be written as  :  (Area of Circle / Area of Sqaure which emcompass the circle) ~   cIN / sIN

=> (Pi * r^2) / ((2r)^2)  = cIN / sIN
=> Pi = 4 * (cIN/sIN)

The program does is repeatedly throws darts ( i.e. creates random number (x and y coordinates) corresponding to cIN and sIN.

cIN : is releatable to the x,y random pair which is withing circle area. 
