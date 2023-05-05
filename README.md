Download Link: https://assignmentchef.com/product/solved-csf211-assignment5
<br>
<strong>A: OS Scheduler</strong>

One of the most important tasks of an operating system is deciding which tasks gets to use the CPUs. Let us say that there are <em>T </em>tasks in the waiting list that require the CPU’s computational power at time <em>t </em>= 0. No additional tasks will be added to the wait list of tasks. Each task requires some CPU time, <em>E<sub>i</sub></em>, for completion and has a priority, <em>P<sub>i </sub></em>(ranging from 0 − 10, with 0 having the highest priority and 10 the least priority). The scheduling algorithm must work by (1) selecting <em>important tasks </em>first (as decided by <em>P<sub>i</sub></em>) and (2) in case of equal preference select the <em>shortest job first </em>(least time required). What are the indices of the first <em>k </em>tasks the scheduling algorithm prioritises? <em>Note: Your solution </em><em>must be in o</em>(<em>T </em>+ <em>k </em>· <em>log</em>(<em>T</em>)).

<strong>Input</strong>

The first line contains two integers <em>T </em>(1 ≤ <em>T </em>≤ 10<sup>5</sup>) and <em>k </em>(1 ≤ <em>k </em>≤ 10<sup>2</sup>). The next <em>N </em>lines contain two space separated integers <em>E<sub>i </sub></em>(0 ≤ <em>E<sub>i </sub></em>≤ 10<sup>9</sup>) and <em>P<sub>i </sub></em>of the tasks (tasks are zero-indexed).

<strong>Output</strong>

Print <em>k </em>space separated integers representing the indices of first <em>k </em>tasks that will be scheduled by the OS.

input

8 3

34 3

2167 5

10 0

23 0

325 3 45 6

646 7

353 7

output

2 3 0

explanation

Schedule all tasks with priority 0 and then schedule the 0<em><sup>th </sup></em>task (priority 3).

<strong>B: Altered Carbon</strong>

In the Bay City Metropolis Hospital, <em>N </em>patients are waiting to be treated outside the hospital today. Being the dystopian society it is, the hospital wishes to <em>maximise </em>it’s earning potential today. Each patient <em>i </em>has a certain <em>net wealth C<sub>i </sub></em>that is stored in an encrypted form in alphanumeric string <em>D<sub>i </sub></em>in their cortical stacks (an implant placed in the neck). The net worth <em>C<sub>i </sub></em>is the sum of all of the <em>alphabet-separated numbers </em>in the string. For example, the string “as3442jhs2323kaj22kjyu3yhdjhshdkjrhsjk211df” contains five numbers in it, and the net worth for this string would be the sum of these five numbers, i.e. <em>sum</em>(3442<em>,</em>2323<em>,</em>22<em>,</em>3<em>,</em>211) = 6001. Given that the hospital can admit only <em>k </em>(1 ≤ <em>k &lt;&lt; N</em>) patients, and wants to admit individuals with the highest net-worths, which ones should it select? What is the sum of these net worths? Since this number might be very large print it modulo 10<sup>9 </sup>+ 7.

<strong>Input</strong>

The first line contains two space separated integers: <em>N </em>(0 ≤ <em>N </em>≤ 10<sup>5</sup>) and <em>k </em>(0 ≤ <em>k </em>≤ 100). The next <em>N </em>lines contain one alphanumeric string each (of length ≤ 150) with each line containing one <em>D<sub>i</sub></em>.

<strong>Output</strong>

Print one integer representing the moduloed sums of net worths ((<sup>P</sup><em><sub>i </sub>C<sub>i</sub></em>)%(10<sup>9 </sup>+7)) of the selected individuals admitted in the hospital. Each string might contain alphabets (upper/lower case) and digits. It is guaranteed that each number inside the string will have at most 10 digits.

input

input

5 3

3 2

a1ghe2

a21b45c90

BGH54jk78

a42b1d3FG6 g3267372673hh7

98nahsg8 jhj666SHH7 apes123strong23together9

output

262 output

267373487

explanation

Person 0: 21 + 45 + 90 = 156

explanation

Person 1: 42 + 1 + 3 + 6 = 52

The net worths are (2, 132,

Person 2: 98 + 8 = 106

3267372680, 673, 155). The answer Select persons 0 and 2 is (3267372680 + 673 + 155)%(10<sub>9 </sub>+ 7).

<strong>C: Largest Number</strong>

Given two numbers <em>N</em><sub>1</sub>, <em>N</em><sub>2 </sub>(as digit strings) find the <em>largest </em>number you can create by following these steps. To merge the numbers:

<ol>

 <li>start with an empty string <em>M</em>.</li>

 <li>At each step you can choose to:

  <ul>

   <li>append the first digit of <em>N</em><sub>1 </sub>to the back of M and delete the first digit in <em>N</em><sub>1 </sub>(or)</li>

   <li>append the first digit of <em>N</em><sub>2 </sub>to the back of M and delete the first digit in <em>N</em><sub>2</sub></li>

  </ul></li>

 <li>Keep repeating this process till both <em>N</em><sub>1 </sub>and <em>N</em><sub>2 </sub>are empty</li>

</ol>

What is the largest possible number you can create by merging <em>N</em><sub>1 </sub>and <em>N</em><sub>2</sub>.

<strong>Input</strong>

There will be two lines of input, with each line containing one very large number (≤ 200 digits).

<strong>Output</strong>

Output a single line, containing the maximal merged number.

input 7756453241 82715243

output 877564532724152431

input 965 453

output 965453

input 775 769

output 777695

<strong>D: Valentine’s Day</strong>

As an an unscrupulous store owner on a college campus, you decide to sell chocolates on Valentine’s Eve in a bid to earn more money. Your supplier has <em>M </em>different kinds of chocolates all of which have different qualities (<em>Q<sub>i</sub></em>), and you want to select <em>exactly two </em>varieties of chocolates to stock. Since you intend to sell chocolates at a grossly overpriced sales price, you decide that you want to <em>maximise </em>the <em>difference </em>in qualities of the two selected chocolates – to make it <em>seem </em>like the chocolate of higher quality is worth the price relative to the lesser, even when both of them aren’t worth it. Given a list of qualities of each type of chocolates, select the types that <em>maximise </em>this difference of qualities of chocolates. What is this maximal difference? And how many ways can you achieve this?

<strong>Input</strong>

The first line has the integer <em>M </em>(2 ≤ <em>N </em>≤ 10<sup>6</sup>). The next line has <em>M </em>space separated integers containing the <em>quality </em>of each type of chocolate (0 ≤ <em>Q<sub>i </sub></em>≤ 10<sup>9</sup>).

<strong>Output</strong>

Print two space-separated integers <em>X </em>and <em>Y </em>. <em>X </em>is the the largest possible difference of qualities of the two selected chocolate types. <em>Y </em>is the number of <em>ways </em>this maximum can be achieved.

input 2

9 278

output

<h1><a name="_Toc12674"></a>269    1</h1>

input

<h1><a name="_Toc12675"></a>3</h1>

19 23 24

output

5 1

input 5

24 15 19 15 24

output

9 4

explanation

There are 4 sets of indices that get the maxmimal difference of 9: (0, 1),

(1, 4), (0, 3), (4, 0)

<strong>E: A Foreshadowing of Array Operations</strong>

You are given an array <em>a </em>of size <em>N </em>in non-decreasing order. In one operation you can choose any two adjacent elements and insert the floor of their average between them. This operation would increase the length of the array by 1. Let the maximum difference between any pair adjacent numbers in the array be <em>m</em>. Using at most <em>k </em>operations, find the minimum possible value of <em>m </em>that can be achieved after these operations.

<em>As an extra challenge (will not be asked in the lab), try solving this if you can insert any integer such that the array remains non-decreasing</em>.

<strong>Input</strong>

The first line contains two integers <em>N </em>and <em>k </em>(1 ≤ <em>N,k </em>≤ 10<sup>5</sup>). The second line contains <em>N </em>integers representing the array <em>a </em>(1 ≤ <em>a<sub>i </sub></em>≤ 10<sup>9</sup>).

<strong>Output</strong>

Print one integer, the minimum possible maximum difference between any two adjacent integers after all operations.

input

5 2

10 13 15 16 17

output 2

explanation you can add up to 2 numbers. Adding 11 and 14 in the appropriate positions would give a maximum difference as 2. It is not possible to do better in this situation

<strong>F: The Maxim</strong>

Migi the parasite is in a human host and trying to take over. To completely take over the host it must first take over all its organs which are numbered from 1 to <em>N</em>. You are given the pairs of organs that are connected to each other. Initially Migi is at organ 1. Migi can only take over a particular organ if it is not already occupied and it is connected to an occupied organ. The human host is fighting back pretty hard so Migi decides to do the following: <strong>at every step choose the smallest numbered organ that is currently unoccupied and is connected to an occupied organ. Occupy the chosen organ</strong>. Migi doesn’t have much time so he asks you to tell him the exact order of organs to occupy including the starting organ.

<strong>Input</strong>

The first line consists of two integers <em>N,M </em>(1 ≤ <em>N,M </em>≤ 10<sup>5</sup>). The next <em>M </em>lines contain two integers <em>u<sub>i </sub></em>and <em>v<sub>i</sub></em>, indicating that organ <em>u<sub>i </sub></em>and organ <em>v<sub>i </sub></em>are connected (1 ≤ <em>u<sub>i</sub>,v<sub>i </sub></em>≤ <em>N</em>). It is guaranteed that all the organs form a connected graph.

<strong>Output</strong>

Print a single line consisting of <em>N </em>integers representing the order of organs Migi occupies (including the starting organ).

input

<a href="#_Toc12673">5                                                                                                                                                                                                     4</a>

<a href="#_Toc12674">1                                                                                                                                                                                                     4</a>

<a href="#_Toc12675">3                                                                                                                                                                                                     4</a>




2 3

1 5

output

1 4 3 2 5

explanation

Initially Migi is at organ 1. Out of the connected organs 4 and 5, we choose 4 as it is the smallest. Now, 4 is connected to 3 and 1 is connected to 5, out of which 3 is the smallest so he occupies that. Now the remaining possible nodes are 2 and 5 so Migi goes to 2 first and then 5.

<strong>G: Array Operations</strong>

You are given an array of size <em>N </em>where the <em>i<sup>th </sup></em>element is <em>a<sub>i</sub></em>. In one operation you will remove the smallest and the largest elements in the array and insert the absolute value of their difference into the end of the array. If multiple elements are smallest or largest pick any one. You are given <em>q </em>queries, each of which consist of a single number <em>k<sub>i</sub></em>. For every <em>i </em>from 1 to <em>q</em>, you have to find the sum of elements after performing <em>k<sub>i </sub></em>operations on the <strong>initial array </strong><em>a</em>.

<strong>Input</strong>

The first line contains two integers <em>N </em>and <em>q </em>(1 ≤ <em>N,q </em>≤ 10<sup>5</sup>). The second line contains <em>N </em>integers, representing the array <em>a</em>. The next <em>q </em>lines contain one integer each, representing the query <em>k<sub>i </sub></em>(1 ≤ <em>k<sub>i </sub></em>≤ <em>N</em>),

<strong>Output</strong>

Output <em>q </em>lines, each line containing one integer representing the answer for the <em>i<sup>th </sup></em>query.

input

5 2

3 2 1 4 5

1 2

output 13 9

explanation after the first operation, the array becomes 3 2 4 4. After the second operation the array becomes 3 4 2.

<strong>H: More Array Operations</strong>

After solving the previous problem, you wanted to challenge yourself some more so you decided to try a slightly different problem. You are given an array of size <em>N </em>where the <em>i<sup>th </sup></em>element is <em>a<sub>i</sub></em>. You have a new array <em>b </em>which is initially empty. In one operation you remove the leftmost element in <em>a </em>and add it somewhere in <em>b</em>. You do this <em>N </em>times until the array <em>a </em>is completely empty. After each step you have to print the median of all the elements in <em>b</em>. Median is defined in the following way: Let <em>M </em>be the size of array <em>b</em>. If <em>M </em>is even, then median is ]. Otherwise, the median is . <em>Hint: Could you use heaps here?</em>

<strong>Input</strong>

The first line contains a single integer <em>N </em>representing the size of the array <em>a</em>. The second line contains <em>N </em>integers where the <em>i<sup>th </sup></em>integer is <em>a<sub>i</sub></em>.

<strong>Output</strong>

output <em>N </em>space separated integers where the <em>i<sup>th </sup></em>integer is the median of <em>b </em>after the <em>i<sup>th </sup></em>operation

input 4

5 15 1 3

output

5 10 5 4

explanation

first operation → <em>b </em>= [5]. Second operation → <em>b </em>= [5<em>,</em>15] so median is 10. Third move <em>b </em>= [5<em>,</em>15<em>,</em>1] and here median is 5. In the final operation <em>b </em>= [51513] where median is

4

<strong>I: Chocolates</strong>

Upon his return from the States, your father has brought you a lot of chocolates. On the first day, he arranges N bowls and adds a few chocolates to each bowl. Everyday (starting from day one), you decide to eat the chocolates from the bowls and select one bowl at random and eat <em>all </em>X chocolates (assuming that the bowl has X chocolates) from it. The next day, your dad replenishes the bowl (from which you ate the chocolates) with bX/3c chocolates. You now start thinking about the <em>maximum </em>number of chocolates you can eat in a span of few days and decide to write a simple program that will calculate the same for you.

<strong>Input</strong>

The first line of input contains two space-separated integers N (1 ≤ N ≤ 10<sup>5</sup>) and D (1 ≤ D ≤ 10<sup>5</sup>) denoting the number of bowls and the number of days for which you want to make the calculation respectively. The following line contains N space-separated integers (0 ≤ <em>A<sub>i </sub></em>≤ 10<sup>9</sup>) denoting the number of chocolates put in each of bowls (the <em>i<sup>th </sup></em>integer denotes the number of chocolates put in the <em>i<sup>th </sup></em>bowl). Assume the bowls are numbered serially from 1 onwards.

<strong>Output</strong>

Print a single integer Y, denoting the maximum number of chocolates you can eat by the end of D days. As the number can be large, print it to modulo 10<sup>9 </sup>+ 7.

input

5 7 4 16 6 27 8

output 75

explanation

It can be observed that you eat 27 + 16 + 9 + 8 + 6 + 5 + 4 = 75 chocolates in 7 days.

<ol>

 <li><strong> Dijkstra</strong></li>

</ol>

Dijkstra’s Single Source Shortest Path Algorithm is perhaps the most used procedure to find shortest paths in a weighted graph. The algorithm is greedy in nature and is optimally done with a minpriority queue (a heap). The pseudo-code for it is as follows:

<ol>

 <li>Mark source vertex with 0 cost initially and rest all vertices with a cost of ∞.</li>

 <li>With the cost of the source vertex, relax the cost of all its neighbours, i.e. cost(v) = min(cost(<em>v</em>), cost(<em>u</em>) + W(<em>u</em>, <em>v</em>)) ∀ vertices <em>v </em>that are neighbors of source vertex <em>u</em>.</li>

 <li>Mark <em>u </em>as visited and from those relaxed, choose the minimum cost vertex and make it the source vertex.</li>

 <li>Go to step 2 and repeat till all vertices are visited.</li>

</ol>

Now given a weighted undirected connected graph G(V, E) and a source vertex <em>s </em>∈ G(V, E), your task is to find the shortest path from <em>s </em>to all the remaining vertices in the graph. <em>Additional: Can you guess the time complexity of Dijkstra using heaps?</em>

<strong>Input</strong>

The first line contains three space-separated integers N (3 ≤ N ≤ 500), M (N-1 and S (0 ≤ S ≤ N-1) denoting the number of vertices, edges and source vertex respectively. The following M lines contain three space separated integers <em>U<sub>i</sub></em>, <em>V<sub>i </sub></em>and <em>W<sub>i </sub></em>(0 ≤ <em>U<sub>i</sub>,V<sub>i </sub></em>≤ N-1, 0 ≤ <em>W<sub>i </sub></em>≤ 10<sup>7</sup>) denoting an edge of weight <em>W<sub>i </sub></em>between vertices <em>U<sub>i </sub></em>and <em>V<sub>i</sub></em>.

<strong>Output</strong>

Print a sequence of N space-separated integers where the <em>i<sup>th </sup></em>integer denotes the shortest path distance to the <em>i<sup>th </sup></em>vertex from the given source vertex.

input

7 13 3

5 6 10

0 5 5

0 1 2                                                                       output

0 2 2                                                                          9 7 8 0 7 8 8

2 3 8

1 4 8                                                                        explanation

<ul>

 <li>3 7 It can be observed by running</li>

 <li>4 5 the algorithm that we get the</li>

</ul>

4 3 7                                                                             distances as mentioned above for

<ul>

 <li>5 8 the vertices 0 to 6</li>

 <li>5 1</li>

</ul>

4 6 1

2 6 2