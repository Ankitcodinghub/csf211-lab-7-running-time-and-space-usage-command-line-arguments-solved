# csf211-lab-7-running-time-and-space-usage-command-line-arguments-solved
**TO GET THIS SOLUTION VISIT:** [CSF211 Lab 7-Running Time and Space Usage, Command Line Arguments Solved](https://www.ankitcodinghub.com/product/csf211-lab-7-running-time-and-space-usage-command-line-arguments-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91913&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSF211 Lab 7-Running Time and Space Usage, Command Line Arguments Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
Topics: QuickSort, Performance Measurements – Running Time and Space Usage, Command Line Arguments

Programming Environment: C on Linux

In all the exercises in this lab sheet, you must construct an array of employee records containing the following fields – {name and empID}, where name is a string containing a maximum of 10 characters and empID is an integer value containing the employee ID. You must use empID as the key for all comparisons in your sorting algorithms. Sample input files are given along with this sheet, which can be used in the exercises as input files. Note that all input files have the fields name and empID separated by space.

Exercise 1:

<ol>
<li>a) &nbsp;Implement the iterative version of QuickSort with an explicit stack such that sub-lists
of size less than or equal to S are left untouched (i.e. not sorted). S is passed as a parameter to QuickSort. Note that S&lt;1 should result in QuickSort running completely i.e. all sub-lists get sorted.
</li>
<li>b) &nbsp;Implement the iterative version of Insertion Sort algorithm.</li>
<li>c) &nbsp;Implement a sorting procedure that (i) invokes QuickSort (your solution to (a)) on the
input list, with a cutoff value for size, followed by (ii) an insertion sort of the entire list.
</li>
</ol>
Exercise 2: [Expected Time: 30 minutes]

a) Write a bisection procedure to decide the cutoff size, above which QuickSort is faster than insertion sort:

define testRun(Ls, size) {

run InsertionSort and QuickSort – separately – on Ls; return the running time measurements (IStime, QStime);

}

define estimateCutoff {

tt1 = testRun(Ls, min); // assert tt1.IStime &lt; tt1.QStime tt2 = testRun(Ls, max); // assert tt1.IStime &gt; tt1.QStime

repeat { mid =(min+max)/2; tt = testRun(Ls, mid);

use tt to narrow the range (i.e. min=mid or max=mid) } (until tt.IStime approximately== tt.QStime)

return mid; }

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
b) Write a main function in C that takes an input file name, an output file name as command line arguments and then:

<ol>
<li>Runs estimateCutoff to decide the cutoff size;</li>
<li>For N=10^4, 10^5, 10^6, … 10^9:
 Read N values from input file

 Call sorting procedure in 1.c) with cutoff size as estimated in (i).  Measure the time taken for sorting and store it

 Write the sorted list into the output file.
</li>
</ol>
Exercise 3:

Repeat 2. (b) for a few different input files and plot curves (one per input file) of size versus time taken. Do curve fitting to find out the closest defining function per curve and match it with estimated time complexity.

Assignment with respect to this lab: Solve Exercise 3 and upload the solution. There might be issues with your system while varying N (in 2(b) above) from 10^4 to 10^9. In such case, you can put upper limit on the value of N. Also, you need not to do curve fitting as a part of this assignment.

In addition to all the .c files, your submission should have one file, named complete.c, in which all the functions you have written must be there. Just copy all the functions and main in this “complete.c” file.

</div>
</div>
</div>
