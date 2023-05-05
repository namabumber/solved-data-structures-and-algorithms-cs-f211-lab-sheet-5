Download Link: https://assignmentchef.com/product/solved-data-structures-and-algorithms-cs-f211-lab-sheet-5
<br>
<ol>

 <li>Captain America and Iron Man are fighting but instead of collecting other superheroes, they plan on collecting ranges. You have <strong><em>n</em></strong> ranges and have been assigned the task of dividing the ranges between the two teams. Every range <strong><em>i</em></strong> has a left limit <strong><em>l<sub>i</sub></em></strong> and a right limit <strong><em>r<sub>i</sub></em></strong>. You have to divide the groups in such a way that, there is no pair of ranges, each from a different group which have a common point. However, ranges assigned to the same group may have a common point. Each range should belong to exactly one group. You have to print <strong><em>IM</em></strong> if you assign a range to Team Iron Man and print <strong><em>CA</em></strong> if you assign the range to Team Captain America. If an assignment is impossible, print -1. There is no restriction on the number of ranges that you can assign to a team. But the assignment cannot be too skewed also, meaning that out <strong><em>n</em></strong> ranges, you can’t give (<strong><em>n</em></strong> -1) range to one team and the remaining 1 range to the other team. Note that for a given set of ranges, multiple assignments are possible. Determine any one of them. Duplicate ranges can be present also.</li>

</ol>




<strong>Input: </strong>

The first line contains one integer <strong><em>T</em></strong> (1 ≤ <strong><em>T</em></strong> ≤ 50000) — the number of queries. Each query contains description of the set of ranges. Queries are independent. First line of each query contains a single integer <strong><em>n</em></strong> (2 ≤ <strong><em>n</em></strong> ≤ 105) — the number of segments. It is guaranteed that <strong><em>∑n</em></strong> over all queries does not exceed 105. Each of the next <strong><em>n</em></strong> lines contains two integers <strong><em>l<sub>i</sub></em></strong>, <strong><em>r<sub>i</sub></em></strong> (1 ≤ <strong><em>l<sub>i</sub></em></strong> ≤ <strong><em>r<sub>i</sub></em></strong> ≤ 2105) for range <strong><em>i</em></strong>.




<strong>Example  Input: </strong>

3

<h1><a name="_Toc12868"></a>2</h1>

5 5

<h1><a name="_Toc12869"></a>2 3</h1>

<h1><a name="_Toc12870"></a>3</h1>

3 5

<a href="#_Toc12868">2                                                                                                                                                                          3 </a>

<a href="#_Toc12869">23                                                                                                                                                                        3 </a>

<a href="#_Toc12870">3                                                                                                                                                                          3 </a>

<a href="#_Toc12871">4                                                                                                                                                                          4 </a>

<a href="#_Toc12872">5                                                                                                                                                                          5 </a>







<strong>Comment: </strong>Here there are total 3 queries, i.e., there are 3 sets of ranges. The first set contains 2 ranges – (5, 5) and (2, 3). The second set contains 3 ranges – (3, 5), (2, 3) and (2, 3). The third set contains 3 ranges – (3, 3), (4, 4), (5, 5).




<strong>Output: </strong>

CA IM

-1

IM IM CA




<ol start="2">

 <li>Naruto and Sasuke are given two arrays <strong><em>A1</em></strong> and <strong><em>A2</em></strong> of size <strong><em>N</em></strong> and <strong><em>M</em></strong> respectively. Since they are in a team, they need to be in sync. Kakashi, as their Sensei, decided to sort <strong><em>A1</em></strong> in such a way that the relative of the elements will be same as that in <strong><em>A2</em></strong>. If there are some elements left in <strong><em>A2</em></strong>, their friend Sakura will append them at last in sorted order. It is also given that the number of elements in <strong><em>A2</em></strong> is smaller than or equal to number of elements in <strong><em>A1</em></strong> and <strong><em>A2</em></strong> has all distinct elements. <strong><em>A1</em></strong> can have duplicate elements. Moreover, <strong><em>A2</em></strong> can have a few elements which are not present in <strong><em>A1</em></strong>.</li>

</ol>

<strong> </strong>

<strong>Input</strong>:

<strong><em>N M </em></strong>

<strong><em>A1 </em></strong>

<strong><em>A2 </em></strong>

<strong> </strong>

<strong>Output: </strong>

The final array.




<strong>Constraints: </strong>

1 ≤ <strong><em>N</em></strong>, <strong><em>M</em></strong> ≤ 106

|<strong><em>A1</em></strong>|&lt;= 106, |<strong><em>A2</em></strong>| &lt;= 106




<strong>Example: Input: </strong>

<h1><a name="_Toc12871"></a>11 4</h1>

2 1 2 5 7 1 9 3 6 8 8 2 1 8 3




<strong>Output: </strong>

2 2 1 1 8 8 3 5 6 7 9




<strong>Input: </strong>

<h1><a name="_Toc12872"></a>10 5</h1>

3 1 4 6 2 1 8 5 3 6

6 1 7 9 8




<strong>Output: </strong>

6 6 1 1 8 2 3 3 4 5




<ol start="3">

 <li>Aroma is a very unique restaurant. They don’t ask for money, but instead request you to carry out certain operations on their behalf. They ask you to insert an element into an already sorted list, delete an element from the sorted list, swap pairs of elements of the list and finally sort the list after swapping(s). You are also required to print the list after every operation. Note that you are not allowed to have vacant positions in the list after deletions and no insertion will be done after swapping (since after every insertion the list needs to remain sorted). Insertions are possible after deletions. After swapping(s), deletions are however, possible. At any point of time, the list will contain only unique elements, assuming that you will not be asked to insert a duplicate element in the list at any point of time. Moreover, you do not know apriori, how many insertion and deletions you will be asked to carry out.</li>

</ol>




<strong>Input</strong>:

The first line contains the elements for the existing list in sorted (ascending) order.

The second line contains the number <strong><em>N </em></strong>of operations to be carried out.

Following <strong><em>N</em></strong> lines contain the details of the operations

<ul>

 <li>For insertion – I Number to be inserted</li>

 <li>For deletion – D Number to be deleted</li>

 <li>For swapping – SW Numbers to be swapped</li>

 <li>For sorting – SO</li>

</ul>




<strong>Output: </strong>

The intermediate array after every operation




<strong>Example  Input: </strong>

3 5 6 8 10 15

13

I 1

I 7

I 18

D 5

D 10

I 2

I 4

I 9

SW 4 18

SW 1 6

D 1

D 7 SO




<strong>Output: </strong>

1 3 5 6 8 10 15

1 3 5 6 7 8 10 15

1 3 5 6 7 8 10 15 18

1 3 6 7 8 10 15 18

1 3 6 7 8 15 18

1 2 3 6 7 8 15 18

1 2 3 4 6 7 8 15 18

1 2 3 4 6 7 8 9 15 18

1 2 3 18 6 7 8 9 15 4

6 2 3 18 1 7 8 9 15 4

6 2 3 18 7 8 9 15 4

6 2 3 18 8 9 15 4

2 3 4 6 8 9 15 18

<strong> </strong>

<ol start="4">

 <li>Aman, Ketan and Shreya always hangout on marine drive. But whenever they ask Apoorva to hang out, she is busy doing homework. They want to help her finish the homework faster. Can you help them understand Apoorva’s homework so that she can hang out with them?</li>

</ol>

Consider an array of <strong><em>arr</em></strong> of <strong><em>n</em></strong> distinct integers. Any two elements of the array can be swapped any number of times. An array is beautiful if the sum of all <strong>|<em>arr[i] – arr[i-1]</em>|</strong> (absolute value) for <strong><em>1 &lt;= i &lt;= (n -1)</em></strong> is minimal. Given the array <strong><em>arr</em></strong>, determine the minimum number of swaps that should be performed in order to make the array beautiful. Note that you are not allowed to make any extra swaps other than what you are displaying as output.

<strong> </strong>

<strong>Input: </strong>

The first line contains the number of elements of the array. The second line contains the elements of the array




<strong>Output: </strong>

The number of swaps required to make the array beautiful.




<strong>Example  Input: </strong>

4

7 15 12 3




<strong>Output: </strong>2




<strong>Explanation: </strong>

After first swap à 3 15 12 7

After second swap à 3 7 12 15




<strong>Input: </strong>4

2 5 3 1




<strong>Output: </strong>2

<strong> </strong>

<strong>Explanation: </strong>

After first swap à 2 1 3 5

After second swap à 1 2 3 5




<ol start="5">

 <li>Klay Thompson is one the best 3-pointer shooters in the history of NBA. He is so much obsessed with the number 3 that his team mates gave him a task. They gave him an array of numbers 0-9 (not necessarily containing all the 10 digits and not necessarily containing only unique digits in sorted order) and asked him to come up with the largest number that is divisible by 3 using these digits. If no such number is possible, he will have to say “No such number”.</li>

</ol>




<strong>Input: </strong>

The first line contains the size of the array.

The second line contains the elements of the array.




<strong>Output: </strong>

The largest number divisible by 3.




<strong>Example  Input: </strong>

5

5 4 3 1 1




<strong>Output: </strong>4311




<strong>Input: </strong>

5

0 5 5 5 7




<strong>Output: </strong>

750




<ol start="6">

 <li>You are given an unsorted array <strong><em>a</em></strong>. You have to find out all the unordered pairs in the array. An unordered pair is defined as a pair <strong><em>(a[i], a[j])</em></strong>, such that <strong><em>i</em></strong> &lt; <strong><em>j</em></strong> but <strong><em>a[i]</em></strong> &gt; <strong><em>a[j]</em></strong>. For example, if the array <strong><em>a</em></strong> contains 2, 3, 1, 4, then the unordered pairs are (2, 1) and (3, 1).</li>

</ol>

<strong> </strong>

<strong>Input: </strong>

The first line contains <strong><em>n</em></strong> (the size of the array).

The second line contains <strong><em>n</em></strong> different integers as elements of <strong><em>a</em></strong>.

<strong> </strong>

<strong>Output: </strong>

The number of unordered pairs in less than O(<strong><em>n<sup>2</sup></em></strong>) time.




<strong>Example: </strong>

<strong>Input: </strong>

5

2 4 1 3 5

<strong> </strong>

<strong>Output: </strong>

3




<ol start="7">

 <li>You are given an undirected, unweighted, connected graph without self-loops consisting of <strong><em>n</em></strong> vertices. For convenience, we will assume that the graph vertices are indexed using integers from 1 to <strong><em>n</em></strong>. One day, you counted the shortest distances from one of the graph vertices to all others and wrote them in an array <strong><em>d</em></strong>. Thus, element <strong><em>d[i]</em></strong> of the array shows the shortest distance from the vertex you chose to vertex number <strong><em>i</em></strong>. Then you lost the graph and also forgot which vertex you chose as the source. Form the graph using the array <strong><em>d</em></strong>.</li>

</ol>

<strong> </strong>

<strong>Input: </strong>

One integer <strong><em>n</em></strong>.

The array <strong><em>d</em></strong> of size <strong><em>n</em></strong>.




<strong>Output: </strong>

If there is no such graph print -1. Otherwise output the integer <strong><em>m</em></strong> which is the number of edges. In each of the next <strong><em>m</em></strong> lines, print two integers, <strong><em>a<sub>i</sub></em></strong> and <strong><em>b<sub>i</sub></em></strong>, separated by a space, denoting the edge that connects vertices with numbers <strong><em>a<sub>i</sub></em></strong> and <strong><em>b<sub>i</sub></em></strong>. The graph shouldn’t contain self-loops and should have only one edge between a pair of vertices. If there are multiple possible answers, print any one of them. <strong><em>m</em></strong> &gt;= |<strong><em>d</em></strong>| meaning you are allowed to add a few extra edges apart from the information derived from the array <strong><em>d</em></strong> keeping in mind the constraint that you have to create exactly one cycle and that cycle should consist of the minimum number of edges. In other words, if multiple cycles are possible, you are allowed to include the one containing the minimum number of edges. If there is a tie in this regard, you can select any one of the cycles.




<strong>Example: </strong>

<strong>Input: </strong>

3

<ul>

 <li>1 1</li>

</ul>




<strong>Output: </strong>

3

<ul>

 <li>2</li>

</ul>

1 3

3 2




<strong>Explanation: </strong>

Here only one cycle is possible.




<strong>Input: </strong>

5

1 0 2 1 1




<strong>Output: </strong>

5

1 2

<ul>

 <li>3</li>

 <li>4</li>

</ul>

2 5

1 4

<strong> </strong>

<strong>Explanation: </strong>(1 4) is the additional edge. Instead of (1 4), (2 3), (1 5), (4 5) could also have been selected. However, (3 4) would have been a wrong choice.




<ol start="8">

 <li>It is Christmas time and you have offered to be the Santa Clause for your village. You want to gift the children XBOX or PS4. For this, you will have to buy PS4s and XBOXs, but you want to spend as little as possible. Now, you know the demand of each child. Some of them are Sony fanatics and only want PS4, some of them love Microsoft products and only want XBOXs and some of them are happy with either of them, i.e., you can gift them any. You have found a shop which sells both PS4s and XBOXs at variable prices. Different types of PS4s come in different prices and so do different types of XBOXs. The total number of devices sold by the shop is <strong><em>m</em></strong>. You want to buy a set of XBOXs and PS4s such that you want to maximize the number of children you can gift (it is not guaranteed that you can gift all the children) and minimize the amount you will be spending. However, your priority is to gift as many children as possible. A child does not care about the variety or cost of a PS4 or an XBOX.</li>

</ol>

<strong> </strong>

<strong>Input:  </strong>

First line contains <strong><em>a</em></strong>, <strong><em>b</em></strong>, <strong><em>c</em></strong>. <strong><em>a</em></strong> denotes the number of children who want a PS4, <strong><em>b</em></strong> denotes the number of children who want an XBOX and <strong><em>c</em></strong> denotes the number of children will do with either (0 ≤ <strong><em>a</em></strong>, <strong><em>b</em></strong>, <strong><em>c</em></strong> ≤ 10^5).

The next line contains <strong><em>m</em></strong> (the number of devices the shop sells). (0 ≤ <strong><em>m</em></strong> ≤ 10^5).

Each of the next <strong><em>m</em></strong> lines describes the device. The <strong><em>i<sup>th</sup></em></strong> line contains first integer <strong><em>val[i]</em></strong> (1 ≤ <strong><em>val[i]</em></strong> ≤ 100)  — the cost of the <strong><em>i<sup>th</sup></em></strong> device, then the type of device (PS4 or XBOX).

<strong> </strong>

<strong>Output:  </strong>

Output two integers. The number of children you will be able to gift (maximize the number) and the cost you will be spending (minimize the cost).

<strong> </strong>

<strong>Example: Input: </strong>

2 1 1

4

<ul>

 <li>PS4</li>

 <li>XBOX</li>

</ul>

3 XBOX

7 XBOX




<strong>Output: </strong>

3 14

<strong> </strong>

<strong>Explanation:</strong> 2 children want PS4 but the shop only has 1 PS4. So 1 child from <strong><em>a</em></strong> category will be left unsatisfied. Only 1 wants XBOX and only 1 will do with either of them. So you will buy 1 PS4 worth 5 INR (to satisfy <strong><em>a</em></strong>). Then, you will get 1 XBOX worth 3 INR (to satisfy <strong><em>b</em></strong>). Then, you will get another XBOX worth 6 INR (to satisfy <strong><em>c</em></strong>). Total 3 devices worth 5+3+6 = 14 INR.




<ol start="9">

 <li>You are performing a Physics experiment. You have recorded <strong><em>n</em></strong> measurements in your notebook. After that, you remembered that the largest and the smallest measurements should differ by more than two times. However, you do not have enough time to record all the measurements and want to somehow manage with the <strong><em>n</em></strong> measurements that you have. You will erase some of the recorded measurements, so as to make the largest and the smallest results of the remaining measurements differ in no more than two times. In other words, if the remaining measurements (after removal) have the smallest value <strong><em>x</em></strong>, and the largest value <strong><em>y</em></strong>, then the inequality <strong><em>y</em></strong> ≤ 2·<strong><em>x</em></strong> must be fulfilled. Also, the largest and the smallest measurements should appear only once in the measurement set. If that is not the case with your recorded set of measurements, you will have to ensure that as well. Of course, to avoid the teacher’s suspicion, you want to remove the minimum number of measurements.</li>

</ol>




<strong>Input:  </strong>

First line contains <strong><em>n</em></strong>, the size of array.

The second line contains <strong><em>n</em></strong> integers <strong><em>c1</em></strong>, <strong><em>c2</em></strong>, …, <strong><em>cn</em></strong> (1 ≤ <strong><em>ci</em></strong> ≤ 5000) — the recorded measurements.




<strong>Output: </strong>

Print a single integer — the minimum number of measurements you will have to remove

<strong> </strong>

<strong>Example: </strong>

<strong>Input: </strong>

6

4 5 3 8 3 7 8




<strong>Output: </strong>3

<strong> </strong>

<strong>Explanation: </strong>Two 3 and one 8 is removed. Now the largest is 8 and the smallest is 4.