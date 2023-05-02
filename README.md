Download Link: https://assignmentchef.com/product/solved-cmsc401-assignment-4-minimum-cost-rod-cutting
<br>
<h1></h1>

<ul>

 <li>You are given a rod that is N inches long and a set of M cutting points on the rod.</li>

 <li>You will need to cut the rod from these M points.</li>

 <li>You can perform the cuts in any order of these points.</li>

 <li>After a cut, rod gets divided into two smaller subrods.</li>

 <li>The cost of making a cut is the length of the current sub-rod in which you are making a cut.</li>

 <li>Your goal is to minimize the total cost of cutting.</li>

 <li>Output will show only the minimum cost.</li>

</ul>

<h1>Assignment 4</h1>

<ul>

 <li>Write a program cmsc401.java that reads the size of the rod and cutting points in the format below:</li>

 <li>The size of the rod, N, in the first line. N&gt;=2, N&lt;=100 <strong><sup>10</sup></strong><strong><sub>4</sub></strong></li>

 <li>The number of cutting points, M, in the second line. M&gt;=1, M&lt;=N-1 <strong><sub>1</sub></strong></li>

 <li>The location of each of M distinct cutting points (will be &gt;0 and &lt;N) <strong>5 </strong>– Only integer values <strong>7</strong></li>

</ul>

<strong>9</strong>

0         1         2           3         4         5          6         7           8         9        10

Cutting points

<h1>Example</h1>

Input in correct format       Correct output

23

10

4

1             0         1         2           3         4         5          6        7                 8                                         9        10

5

7

9




Order                     Cost

<ul>

 <li>Cutting at 5: 10</li>

 <li>Cutting at 1: 5 3) Cutting at 7:   5</li>

</ul>

4) Cutting at 9:                   3

———————————

Total Cost:                        23

Cutting points

An order of cutting points that gives the min

cost is 5,1,7,9 (there are also others giving

the same minimum)




<h1>Hint</h1>

<h2>• Define the problem in terms of cutting the rod from one point to another one</h2>

– C(i,j) = cost of cutting the rod from point i to point j

<ul>

 <li>Find the recursive formula</li>

 <li>Apply a dynamic programming method</li>

 <li>Target O(M<sup>3</sup>) complexity</li>

</ul>