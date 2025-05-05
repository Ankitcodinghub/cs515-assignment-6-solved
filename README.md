# cs515-assignment-6-solved
**TO GET THIS SOLUTION VISIT:** [CS515 Assignment 6 Solved](https://www.ankitcodinghub.com/product/cs515-assignment-6-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100701&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS515 Assignment 6 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1 Overview

The learning objective of this assignment is for students to gain some programming experience on designing a Bloom Filter which is commonly used to eliminate unnecessary accesses to slower storage or expensive lookups. Bloom Filter is a data structure for storing an unordered set using hash functions.

Suppose we are given a set S, drawn from a universe U and queries of the form is x ∈ S?, we define a Bloom filter as follows:

<ul>
<li>Take an array A with n elements and take m hash functions h1, h2, ···, and hm. Each hash function maps the universe U to [0, n − 1].</li>
<li>Suppose we start with S being the emptyset, then A[i] is set to 0 for all i.</li>
<li>Now, suppose we insert an element e into the set S. We set A[h1(e)], A[h2(e)], ··· A[hm(e)] all to 1</li>
<li>If any of these m positions were already set to 1 then we just leave it at 1.
Membership Queries: Given a query is x ∈ S? we look at A[h1(x)], A[h2(x)], · · · , A[hm(x)]. If they are all 1 then
</li>
</ul>
we return yes as the answer, otherwise we return no.

Note that it is possible that x ̸∈ S but A[h1(x)], A[h2(x)], · · · , A[hm(x)] are all set to 1 (due to some other elements being in S which have set those positions to 1). This phenomena is called a false positive i.e. the query returns a yes answer although the element is not in the set.

2 Task to be carried out

For this task you will implement a Bloom filter on the universe U = {0, 1, 2, …, n − 1}. Your array should have size n. You will choose any m hash functions of the from h(x) = ((ax + b) mod c) mod n where a, b and c are large positive integers.

Now, you should do the followings:

<ol>
<li>Initialization of Bloom Filter: Initialize your Bloom Filter by inserting any k elements at random from U. Let
us denote this randomly generated k elements as S. Display the Bloom filter created using S.
</li>
<li>Membership Queries &amp; Finding Causes for False Positives: Once the state of the Bloom filter has been displayed, then the program should ask to move forward with a keypress. After that the program should launch queries on each of the remaining n − k items. If any one of these returns a yes answer, the program should pause and find out why this false positive has been returned i.e. it should locate the hash function collisions that have caused this false positive to occur. More formally, if we get a yes answer for x although x is not in S, this means that A[h1(x)], A[h2(x)] and A[h3(x)] are all 1. Your program should return (at most) m elements u1, u2, ···, um from S which hash to the positions h1(x), h2(x), ···, hm(x) through one of the m hash functions. Your program should display which location has been set to 1 by which element of S through which hash function.</li>
<li>Summarizing False Positive Cases: Finally the program should count the total number of false positives
occurring in all n − k membership queries and display the false positive probability p i.e. the fraction of false

positivesoutofn−k. Formallypcanbedefinedasp=∀x∈{U−S}(count((x∈S)=yes)) |U|−|S|
</li>
<li>Input File Format: The entries of the input file is as follows-
m //no of hash functions

a1 b1 c1 // a b c parameters of hash function 1 a2 b2 c2 // a b c parameters of hash function 2 …

am bm cm // a b c parameters of hash function m n // The array size of the bloom filter

k // No. of elements to be inserted

S // elements of S
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
5. Output File Format: The entries of the output file will be as follows-

</div>
</div>
<div class="layoutArea">
<div class="column">
m= n= k=

The Bloom filter is

//Should generate the sequence of n length binary string

Membership queries x ∈ S ∀x ∈ {U − S}

x, false positive (y/n), collusion cases

Fraction of false positives , p =

3 Assumption

We will assume that there is no deletion for the purposes of this assignment i.e. only insertion and membership queries have to be implemented

4 Submission

You need to implement the bloom filter either using c or c++. Your need to include the followings in your submission file-

<ul>
<li>Your C or C++ code</li>
<li>A README file (assign6README.txt) comprising the necessary documentation required to execute your program must also be created. You must also mention the input filename and output filename. Try to generate the output filename using the combination of m, n and k values. For example, if m = 3, n = 100 and k = 25 then the output filename could be op m3n100k25.txt.</li>
</ul>
</div>
</div>
</div>
