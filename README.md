# numerical-computing-project-1--pagerank-algorithm-and-social-networks-solved
**TO GET THIS SOLUTION VISIT:** [Numerical Computing Project 1- PageRank Algorithm and Social Networks  Solved](https://www.ankitcodinghub.com/product/numerical-computing-project-1-pagerank-algorithm-and-social-networks-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;134167&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Numerical Computing Project 1- PageRank Algorithm and Social Networks&nbsp; Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
Project 1 – PageRank Algorithm and Social Networks

The purpose of the first part of this project<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> is to learn the importance of numerical algorithms in the solution of fundamental linear algebra problems frequently occurring in search engines. The second part of the mini-project<a href="#_ftn2" name="_ftnref2"><sup>[2]</sup></a>deals—on the other hand—with the application of sparse linear algebra algorithms to the solution of problems pertaining to social network analysis.

<h1>1. Linear Systems and the PageRank Algorithm</h1>
One of the reasons why Google<sup>TM </sup>is such an effective search engine is the Page-Rank<sup>TM </sup>algorithm developed by Google’s founders, Larry Page and Sergey Brin, when they were graduate students at Stanford University. PageRank is determined entirely by the link structure of the World Wide Web. It is recomputed about once a month and does not involve the actual content of any Web pages or individual queries. Then, for any particular query, Google finds the pages on the Web that match that query and lists those pages in the order of their PageRank. Imagine surfing the Web, going from page to page by randomly choosing an outgoing link from one page to get to the next. This can lead to dead ends at pages with no outgoing links, or cycles around cliques of interconnected pages. So, a certain fraction of the time, simply choose a random page from the Web. This theoretical random walk is known as a <em>Markov chain </em>or <em>Markov process</em>. The limiting probability that an infinitely dedicated random surfer visits any particular page is its PageRank. A page has high rank if other pages with high rank link to it.

Let <em>W </em>be the set of Web pages that can be reached by following a chain of hyperlinks starting at some root page and let n be the number of pages in <em>W</em>. For Google, the set <em>W </em>highly fluctuates over time and is not exactly known, but was estimated to be about 30 billion in 2016<a href="#_ftn3" name="_ftnref3"><sup>[3]</sup></a>. Let <em>G </em>be the <em>n</em>-by-<em>n </em>connectivity matrix of a portion of the Web, that is <em>g<sub>ij </sub></em>= 1 if there is a hyperlink to page <em>i </em>from page <em>j </em>and zero otherwise. The matrix <em>G </em>can be huge, but it is very sparse. Its <em>j</em>-th column shows the links on the <em>j</em>-th page. The number of nonzeros in <em>G </em>is the total number of hyperlinks in <em>W</em>. Let <em>r<sub>i </sub></em>and <em>c<sub>j </sub></em>be the row and column sums of <em>G</em>:

<em>r</em><em>i </em>= X<em>g</em><em>ij </em>and <em>c</em><em>j </em>= X<em>g</em><em>ij</em><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(1)

<em>j&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i</em>

The quantities <em>r<sub>j </sub></em>and <em>c<sub>j </sub></em>are the <em>in-degree </em>and <em>out-degree </em>of the <em>j</em>-th page. Let <em>p </em>be the probability that the random walk follows a link. A typical value is <em>p </em>= 0<em>.</em>85. Then 1 − <em>p </em>is the probability that some arbitrary page is chosen and <em>δ </em>= (1 − <em>p</em>)<em>/n </em>is the probability that a particular random page is chosen. Let <em>A </em>be a <em>n</em>-by-<em>n </em>matrix with elements

<em>,</em>

(2)

Notice that <em>A </em>comes from scaling the connectivity matrix by its column sums. The <em>j</em>-th column is the probability of jumping from the <em>j</em>-th page to the other pages on the Web. If the <em>j</em>-th page is a dead end – i.e., it has no out-links – then we assign a uniform probability of 1<em>/n </em>to all the elements in its column. Most of the elements of <em>A </em>are equal to <em>δ</em>, the probability of jumping from one page to another without following a link. If <em>n </em>= 4 · 10<sup>9 </sup>and <em>p </em>= 0<em>.</em>85, then <em>δ </em>= 3<em>.</em>75 · 10<sup>−11</sup>. Matrix <em>A </em>is the transition probability matrix of the Markov chain. Its elements are all strictly between zero and one and its column sums are all equal to one. An important result from matrix theory, known as the <em>Perron-Frobenius theorem</em>, applies to such matrices: a nonzero solution of the equation

<table width="680">
<tbody>
<tr>
<td width="663"><em>x </em>= <em>Ax</em>

exists and is unique to within a scaling factor. If this scaling factor is chosen so that
</td>
<td width="17">(3)</td>
</tr>
<tr>
<td width="663">X

<em>x<sub>i </sub></em>= 1<em>,</em>
</td>
<td width="17">(4)</td>
</tr>
</tbody>
</table>
<em>i</em>

then <em>x </em>is the <em>state vector </em>of the Markov chain and corresponds to <em>Google’s PageRank</em>. The elements of <em>x </em>are all positive and less than one. Vector <em>x </em>is the solution to the singular, homogeneous linear system

(<em>I </em>− <em>A</em>)<em>x </em>= 0&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (5)

For modest <em>n</em>, an easy way to compute <em>x </em>in Matlab is to start with some approximate solution, such as the PageRanks from the previous month, or

x = ones(n, 1) / n

Then simply repeat the assignment statement

x = A * x

until the difference between successive vectors is within a specified tolerance. This is known as the power method and is about the only possible approach for very large <em>n</em>. In practice, the matrices <em>G </em>and <em>A </em>are never actually formed. One step of the power method would be done by one pass over a database of Web pages, updating weighted reference counts generated by the hyperlinks between pages. The best way to compute PageRank in Matlab is to take advantage of the particular structure of the Markov matrix. Here is an approach that preserves the sparsity of <em>G</em>. The transition matrix can be written

<em>A </em>= <em>pGD </em>+ <em>ez</em><sup>|</sup><em>,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(6)

where <em>D </em>is the diagonal matrix formed from the reciprocals of the out-degrees,

(7)

<em>.</em>

<em>e </em>is the <em>n</em>-vector of all ones, and <em>z </em>is the vector with components

(8)

<em>.</em>

The rank-one matrix <em>ez</em><sup>| </sup>accounts for the random choices of Web pages that do not follow links. The equation

<em>x </em>= <em>Ax&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(9)

can be written as

(<em>I </em>− <em>pGD</em>)<em>x </em>= <em>γe&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(10)

where

<em>γ </em>= <em>z</em><sup>|</sup><em>x.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(11)

We do not know the value of <em>γ </em>because it depends on the unknown vector <em>x</em>, but we can temporarily take <em>γ </em>= 1. As long as <em>p </em>is strictly less than one, the coefficient matrix <em>I </em>− <em>pGD </em>is nonsingular and the equation

(<em>I </em>− <em>pGD</em>)<em>x </em>= <em>e&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(12)

can be solved for <em>x</em>. Then the resulting <em>x </em>can be rescaled so that

X

<em>x<sub>i </sub></em>= 1<em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(13)

<em>i</em>

Notice that vector <em>z </em>is not involved in this calculation. The following Matlab statements implement this approach.

<table width="675">
<tbody>
<tr>
<td width="675">c = sum(G,1); k = find(c˜=0);

D = sparse(k,k,1./c(k),n,n); e = ones(n,1); I = speye(n,n); x = (I – p*G*D)\e; x = x/norm(x,1);
</td>
</tr>
</tbody>
</table>
The power method [1, 2] can also be implemented in a way that does not actually form the Markov matrix and so preserves sparsity. Compute

G = p*G*D;

z = ((1-p)*(c˜=0) + (c==0))/n;

Start with

x = e / n;

Then repeat the statement

x = G*x + e*(z*x);

until <em>x </em>settles down to several decimal places.

It is also possible to use an algorithm known as inverse iteration [1, 3] where one defines

x = e/n A = p*G*D + e*z

and then the following statement is repeated until convergence given a suitable value <em>α</em>.

x = (alpha*I – A)\x x = x/norm(x,1)

For details of when and why this method works, please refer to the references cited above. However, we would like to briefly observe what happens when we take <em>α </em>= 1 in the expression (<em>αI </em>− <em>A</em>). Since the resulting matrix (<em>I </em>− <em>A</em>) is theoretically singular, with exact computation some diagonal elements of the upper triangular factor of (<em>I </em>− <em>A</em>) would, in principle, be zero and this computation should fail. But with roundoff error, the computed matrix (<em>I </em>−<em>A</em>) is probably not exactly singular. Even if it is singular, roundoff during Gaussian elimination will most likely prevent any exact zero diagonal elements. We know that Gaussian elimination with partial pivoting always produces a solution with a small residual, relative to the computed solution, even if the matrix is badly conditioned. The vector obtained with the backslash operation, (<em>I </em>− <em>A</em>)\<em>x</em>, usually has very large components. If it is rescaled by its sum, the residual is scaled by the same factor and becomes very small. Consequently, the two vectors <em>x </em>and <em>Ax </em>equal each other to within roundoff error. In this setting, solving the singular system with Gaussian elimination blows up, but it blows up in exactly the right direction.

Figure 1 is the graph for a tiny example, with <em>n </em>= 6 instead of <em>n </em>= 4 · 10<sup>9</sup>. The pages on the Web are identified by strings known as uniform resource locators, or URLs. Most URLs begin with https because they use the hypertext transfer protocol. In Matlab, we can store the URLs as an array of strings in a cell array. The example in Figure 1 can be written as follows by using a 6-by-1 cell array:

<table width="675">
<tbody>
<tr>
<td width="675">U = {’https://www.alpha.com’

’https://www.beta.com’

’https://www.gamma.com’

’https://www.delta.com’

’https://www.rho.com’

’https://www.sigma.com’}
</td>
</tr>
</tbody>
</table>
Figure 1: A tiny web graph.

In order to access the string contained in a cell we can simply write <em>U</em>(<em>k</em>), with <em>k </em>= 1<em>,…,</em>6 in this small web graph. Thus, <em>U</em>(1) would, e.g., correspond to the string ”https://www.alpha.com”.

We can generate the connectivity matrix by specifying the pairs of indices (<em>i,j</em>) of the nonzero elements. Because there is a link to beta.com from alpha.com, the (2<em>,</em>1) element of <em>G </em>is nonzero. The nine connections are described by

i = [ 2 6 3 4 4 5 6 1 1] j = [ 1 1 2 2 3 3 3 4 6]

A sparse matrix is stored in a data structure that requires memory only for the nonzero elements and their indices. This is hardly necessary for a 6-by-6 matrix with only 27 zero entries, but it becomes crucially important for larger problems. The statements

n = 6 G = sparse(i,j,1,n,n); full(G)

generate the sparse representation of an <em>n</em>-by-<em>n </em>matrix with ones in the positions specified by the vectors <em>i </em>and <em>j </em>and display its full representation.

<table width="675">
<tbody>
<tr>
<td width="81">0</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="43">1</td>
<td width="43">0</td>
<td width="422">1</td>
</tr>
<tr>
<td width="81">1</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="422">0</td>
</tr>
<tr>
<td width="81">0</td>
<td width="43">1</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="422">0</td>
</tr>
<tr>
<td width="81">0</td>
<td width="43">1</td>
<td width="43">1</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="422">0</td>
</tr>
<tr>
<td width="81">0</td>
<td width="43">0</td>
<td width="43">1</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="422">0</td>
</tr>
<tr>
<td width="81">1</td>
<td width="43">0</td>
<td width="43">1</td>
<td width="43">0</td>
<td width="43">0</td>
<td width="422">0</td>
</tr>
</tbody>
</table>
The statement

c = full(sum(G))

computes the column sums

<table width="675">
<tbody>
<tr>
<td width="53">2</td>
<td width="43">2</td>
<td width="43">3</td>
<td width="29">1</td>
<td width="43">0</td>
<td width="465">1</td>
</tr>
</tbody>
</table>
Notice that <em>c</em>(5) = 0 because the 5th page, labeled <em>rho</em>, has no out-links. The statements

x = (I – p*G*D)\e x = x/norm(x,1)

solve the sparse linear system to produce

x = 0.3210

0.1705

0.1066

0.1368

0.0643

0.2007

Figure 2: Page Rank for the tiny web graph

The bar graph of <em>x </em>is shown in Figure 2. If the URLs are sorted in PageRank order and listed along with their in- and out-degrees, the result is

<table width="675">
<tbody>
<tr>
<td width="110">page-rank</td>
<td width="57">in</td>
<td width="50">out</td>
<td width="458">url</td>
</tr>
<tr>
<td width="110">1 0.3210</td>
<td width="57">2</td>
<td width="50">2</td>
<td width="458">https://www.alpha.com</td>
</tr>
<tr>
<td width="110">6 0.2007</td>
<td width="57">2</td>
<td width="50">1</td>
<td width="458">https://www.sigma.com</td>
</tr>
<tr>
<td width="110">2 0.1705</td>
<td width="57">1</td>
<td width="50">2</td>
<td width="458">https://www.beta.com</td>
</tr>
<tr>
<td width="110">4 0.1368</td>
<td width="57">2</td>
<td width="50">1</td>
<td width="458">https://www.delta.com</td>
</tr>
<tr>
<td width="110">3 0.1066</td>
<td width="57">1</td>
<td width="50">3</td>
<td width="458">https://www.gamma.com</td>
</tr>
<tr>
<td width="110">5 0.0643</td>
<td width="57">1</td>
<td width="50">0</td>
<td width="458">https://www.rho.com</td>
</tr>
</tbody>
</table>
We see that alpha has a higher PageRank than delta or sigma, even though they all have the same number of in-links. A random surfer will visit alpha over 32% of the time and rho only about 6% of the time.

For this tiny example with <em>p </em>= <em>.</em>85, the smallest element of the Markov transition matrix is <em>δ </em>= <em>.</em>15<em>/</em>6 = <em>.</em>0250.

<table width="675">
<tbody>
<tr>
<td width="675">A =

0.0250 0.0250 0.0250 0.8750 0.1667 0.8750

0.4500 0.0250 0.0250 0.0250 0.1667 0.0250

0.0250 0.4500 0.0250 0.0250 0.1667 0.0250

0.0250 0.4500 0.3083 0.0250 0.1667 0.0250

0.0250 0.0250 0.3083 0.0250 0.1667 0.0250

0.4500 0.0250 0.3083 0.0250 0.1667 0.0250
</td>
</tr>
</tbody>
</table>
We can notice that all the columns of matrix <em>A </em>sum to one, thus agreeing with the definition of left stochastic matrix. This mini-project includes the Matlab file surfer.m. A statement like

[U,G] = surfer(’https://www.xxx.zzz’,n)

starts at a specified URL and tries to surf the Web until it has visited <em>n </em>pages. If successful, it returns an <em>n</em>-by-1 cell array of URLs and an n-by-n sparse connectivity matrix. Surfing the Web automatically is a dangerous undertaking and this function must be used with care. Some URLs contain typographical errors and illegal characters. There is a list of URLs to avoid that includes .gif files and Web sites known to cause difficulties. Most importantly, surfer can get completely bogged down trying to read a page from a site that appears to be responding, but that never delivers the complete page. When this happens, it may be necessary to have the computer’s operating system ruthlessly terminate Matlab. With these precautions in mind, you can use surfer to generate your own PageRank examples. The statement

[U, G] = surfer(’https://inf.ethz.ch/’,500);

accesses the home page of the Department of Computer Science at the Swiss Federal Institute of Technology in Zurich (ETH) and generates a 500-by-500 test case. The file ETH500.mat included in the code folder was generated by using this function in September 2014. In the following, it is indicated as the <em>ETH500 data set</em>. The statement

spy(G)

produces a spy plot (Figure 3) that shows the nonzero structure of the connectivity matrix. The statement

pagerank(U, G)

computes the page ranks, produces a bar graph (Figure 4) of the ranks, and prints the most highly ranked URLs in

PageRank order. The highly ranked pages are

<table width="675">
<tbody>
<tr>
<td colspan="2" width="146">&gt;&gt; pagerank(U,G) page-rank</td>
<td colspan="2" width="529">in out url</td>
</tr>
<tr>
<td width="60">57</td>
<td width="86">0.145755</td>
<td width="72">292 1</td>
<td width="458">http://www.zope.org</td>
</tr>
<tr>
<td width="60">466</td>
<td width="86">0.049996</td>
<td width="72">19&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1</td>
<td width="458">http://purl.org/dc/elements/1.1</td>
</tr>
<tr>
<td width="60">39</td>
<td width="86">0.028766</td>
<td width="72">311 0</td>
<td width="458">http://www.ethz.ch</td>
</tr>
<tr>
<td width="60">58</td>
<td width="86">0.021863</td>
<td width="72">291 0</td>
<td width="458">http://www.infrae.com</td>
</tr>
<tr>
<td width="60">53</td>
<td width="86">0.021202</td>
<td width="72">288 0</td>
<td width="458">http://www.cd.ethz.ch/services/web</td>
</tr>
<tr>
<td width="60">101</td>
<td width="86">0.016601</td>
<td width="72">234 6</td>
<td width="458">http://www.hk.ethz.ch/index_EN</td>
</tr>
<tr>
<td width="60">72</td>
<td width="86">0.016473</td>
<td width="72">235 0</td>
<td width="458">http://www.ethz.ch/index_EN</td>
</tr>
<tr>
<td width="60">486</td>
<td width="86">0.007374</td>
<td width="72">14&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2</td>
<td width="458">http://www.handelszeitung.ch</td>
</tr>
<tr>
<td width="60">463</td>
<td width="86">0.006896</td>
<td width="72">17&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0</td>
<td width="458">http://ns.adobe.com/xap/1.0</td>
</tr>
</tbody>
</table>
Figure 3: Spy plot of the Department of Computer Science (ETH Zurich) web graph.

Figure 4: PageRank of the Department of Computer Science (ETH Zurich) web graph.

<h1>2. Social Networks and the Householder XII Meeting</h1>
In June, 1993, the UCLA Lake Arrowhead Conference Center in the San Bernardino Mountains, 90 miles east of Los Angeles, was the site of the Householder XII Symposium on Numerical Linear Algebra, organized by Gene Golub<a href="#_ftn4" name="_ftnref4"><sup>[4]</sup></a>and Tony Chan. Nick Trefethen posted a flip chart with Gene Golub’s name in the center. He invited everyone present to add their name to the chart and draw lines connecting their name with the names of all their coauthors. The diagram grew denser throughout the week. At the end it was a graph with 104 vertices (or people) and 211 edges. John Gilbert entered the names and coauthor connections into Matlab, creating an adjacency matrix <em>A</em>. Using Matlab, we can start by retrieving the names and matrix stored in the PARC archive (housegraph.mat), which is available on iCorsi.

load housegraph

The variable who shows which variables are stored in the data file.

who

Your variables are:

A&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Bunch&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Funderlic Ipsen&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Moler&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Reichel

ATrefethen BunseGerstner George&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Jessup&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; MuntheKaas Ruhe

Ammar&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Byers&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gilbert&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Kagstrom&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NHigham&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Saied

Anjos&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Chandrasekaran Gill&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Kahan&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NTrefethen Sameh

Arioli&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Crevelli&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Golub&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Kaufman&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Nachtigal&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Saunders

Ashby&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Cullum&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gragg&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Kenney&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Nagy&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Schreiber

Bai&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Davis&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Greenbaum Kincaid&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Ng&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Smith

Barlow&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Demmel&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gu&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Kuo&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Nichols&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Starke

Benzi&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Dubrulle&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gutknecht Laub&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; OLeary&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Stewart

Berry&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Duff&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hammarling LeBorne&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Ong&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Strakos

Bjorck&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Edelman&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hansen&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Liu&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Overton&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Szyld

Bjorstad&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Eisenstat&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Harrod&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Luk&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Paige&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; TChan

Bojanczyk Elden&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; He&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Marek&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Pan&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tang

Boley&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Ernst&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heath&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Mathias&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Park&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tong

Boman&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Fierro&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Henrici&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Meyer&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Plemmons&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; VanDooren

Borges&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Fischer&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hochbruck Modersitzki Pothen&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; VanHuffel

VanLoan&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Varah&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Varga&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Warner&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Widlund&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Wilkinson

Wold&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Young&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Zha&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; name&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; prcm&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; xy

and name shows the participants in the order they were added to the list:

Figure 5: [Left] The coauthor matrix from the meeting (created with spy(A), [Right] The coauthor circle from the meeting.

name

<table width="675">
<tbody>
<tr>
<td width="675">name =

Golub

Wilkinson

TChan

He

Varah

Kenney

Ashby ..

..
</td>
</tr>
</tbody>
</table>
size(A)

ans =

104&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 104

Matrix <em>A </em>is 104-by-104 and symmetric. Elements <em>A<sub>i,j </sub></em>and <em>A<sub>j,i </sub></em>are both equal to one if the people associated with indices <em>i </em>and <em>j </em>are coauthors and equal to zero otherwise. Matrix A is sparse, since most of the attendees are not coauthors and, thus, their corresponding entries have value 0. In order to check the matrix sparsity – i.e., the fraction of nonzero entries over the total number of elements – we can use the following command:

format short sparsity = nnz(A)/prod(size(A))

sparsity = 0.0486

As we can observe, only roughly 5% of the entries of matrix A are different from 0 or, in other words, only 5% of all the possible pairs of attendees actually identify coauthors. In the left panel of Figure 5, we show a graphical representation of matrix A by means of a spy plot. The latter shows the location of the non-zeros, with Gene Golub in the first row/column, followed by the other authors in the order in which they appeared on Trefethen’s flip chart.

<h2>2.1. Most Prolific Author</h2>
As the adjacency matrix is loaded from the archive, the most prolific coauthor is already in the first column. It was not a surprise to the conference participants that the most prolific coauthor is Gene Golub, one of the organizers.

Figure 6: [Left] The reordered coauthor matrix <em>PAP<sup>T </sup></em>from the meeting, [Right] The reordered coauthor circle.

m = find(sum(A) == max(sum(A))) name(m,:)

m = 1 ans = Golub

<h2>2.2. Circular plot of all the Authors</h2>
In the right panel of Figure 5, we created a circular plot with Golub in the center, the other authors around the circumference, and edges connecting the coauthors. If we place the authors around the circumference in the order we retrieve them from the chart, the edges would cross the circle pretty much randomly, as shown in Figure 5.

drawit; snapnow

<h2>2.3. Reorder the Authors</h2>
We want to rearrange the authors so that the coauthor connections are as close as possible to the circumference of the circle. This corresponds to a symmetric permutation of matrix <em>A</em>, aimed at minimizing, or at least reducing, its bandwidth. In 1969, Elizabeth Cuthill and John McKee described a heuristic for reordering the rows and columns of a matrix to reduce its bandwidth, now known as the <em>Reverse Cuthill McKee </em>ordering.

<table width="675">
<tbody>
<tr>
<td width="675">r = symrcm(A(2:end,2:end)); prcm = [1 r+1];

spy(A(prcm,prcm))

title(’Coauthor matrix with reduced bandwidth’); drawitrcm; snapnow
</td>
</tr>
</tbody>
</table>
Figure 6 shows the impact of the reordering <em>P </em>on both matrix <em>PAP<sup>T </sup></em>and on the circular plot.

<strong>Solve the following problems [85 points]:</strong>

<h2>Preliminary: Read “A First Course on Numerical Methods”</h2>
Read chapter 8 and section 5.7 on <em>Permutations and ordering strategies, pp. 122-127 </em>from the textbook [1], in order to gain a better understanding of the topic summarized above.

<h2>1. Theoretical questions [15 points]</h2>
<ul>
<li>What are an eigenvector, an eigenvalue and an eigenbasis?</li>
<li>What assumptions should be made to guarantee convergence of the power method?</li>
<li>What is the shift and invert approach?</li>
<li>What is the difference in cost of a single iteration of the power method, compared to the inverse iteration?</li>
<li>What is a Rayleigh quotient and how can it be used for eigenvalue computations?</li>
</ul>
<h2>2. Connectivity matrix and subcliques [5 points]</h2>
The connectivity matrix for the ETH500 data set (ETH500.mat) has various small, almost entirely nonzero, submatrices that produce dense patches near the diagonal of the spy plot. You can use the zoom button to find their indices. The first submatrix has, e.g., indices around 80. Mathematically, a graph where all nodes are connected to each other is known as a clique. Identify the organizations within the ETH community that are responsible for these near cliques.

<h2>3. Connectivity matrix and disjoint subgraphs [10 points]</h2>
Figure 7: Another tiny Web.

Figure 7 reports the graph of a tiny six-node subset of the Web. Unlike the example reported in Figure 1, in this case there are two disjoint subgraphs.

<ol>
<li>What is the connectivity matrix G? Which are its entries?</li>
<li>What are the PageRanks if the hyperlink transition probability <em>p </em>assumes the default value of 0<em>.</em>85?</li>
<li>Describe what happens with this example to both the definition of PageRank and the computation done by pagerank in the limit <em>p </em>→ 1.</li>
</ol>
<h2>4. PageRanks by solving a sparse linear system [25 points]</h2>
The function pagerank(U,G) computes PageRanks by solving a sparse linear system. It then plots a bar graph and prints the dominant URLs.

<ol>
<li>Create pagerank1.m by modifying pagerank.m to use the power method instead of solving the sparse linear system. The key statements are</li>
</ol>
<table width="639">
<tbody>
<tr>
<td width="639">G = p*G*D z = ((1-p)*(c˜=0) + (c==0))/n; while termination_test

x = G*x + e*(z*x)

end
</td>
</tr>
</tbody>
</table>
What is an appropriate test for terminating the power iteration?

<ol start="2">
<li>Create pagerank2.m by modifying pagerank.m to use the inverse iteration. The key statements are</li>
</ol>
while termination_test

x = (alpha*I – A)\x x = x/norm(x,1)

end

Use your functions pagerank1.m and pagerank2.m (set <em>α </em>= 0<em>.</em>99) to compute the PageRanks of the six-node example presented in Figure 1. Make sure you get the same result from each of your three functions.

<ol start="3">
<li>We now want to analyse the impact of <em>α </em>on the inverse iteration. Using the ETH500 example, set <em>α </em>equal to 0<em>.</em>8<em>,</em>0<em>.</em>9<em>,</em>0<em>.</em>95 and 1. Comment on the different number of iterations the four cases take until convergence.</li>
</ol>
Analyse your results and explain what you observe.

<em>Hint: </em>Check your solution <em>x </em>for all 4 cases. Are they always the same?

<ol start="4">
<li>Use your functions pagerank1.m and pagerank2.m (set <em>α </em>= 0<em>.</em>99) to compute the PageRanks of three selected graphs (web1.mat, web2.mat and web3.mat). Report on the convergence of the two methods for these subgraphs and summarize the advantages and disadvantages of the power method implemented in pagerank1.m against the inverse iteration in pagerank2.m.</li>
</ol>
<h2>5. The Reverse Cuthill–McKee Ordering [5 points]</h2>
Load matrix ”<em>A </em>SymPosDef.mat” from the dataset. You can reorder (permute) the matrix using “Reverse Cuthill McKee Ordering” via the Matlab function symrcm(), see Matlab documentation for more information. Visualize both the original and Reverse Cuthill McKee permuted matrix and comment on what you observe. Compute the Cholesky factor of the original matrix and the permuted matrix. Visualize the Cholesky factors and comment on the number of nonzeros.

<h2>6. Sparse Matrix Factorization [10 points]</h2>
Let <em>A </em>∈ R<em><sup>n</sup></em><sup>×<em>n </em></sup>be symmetric and positive definite, with entries <em>A<sub>ij </sub></em>defined as follows:

<em>A<sub>ij </sub></em>= <em>n </em>+ <em>i </em>− 1<em>,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>if <em>i </em>= <em>j&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(14)

<sup></sup>0<em>,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>otherwise

Please note that the increasingly larger values on the diagonal are necessary to ensure the positive definiteness of matrix A. Answer the following questions:

<ol>
<li>Construct matrix <em>A </em>for the case <em>n </em>= 10 and explicitly write down its entries. How many non-zero elements does it have?</li>
<li>We now want to derive a general formula to compute the number of non-zero entries. Show that, for a given matrix <em>A </em>∈ R<em><sup>n</sup></em><sup>×<em>n </em></sup>with this structure, the number of non-zero elements is 5<em>n </em>− 6.</li>
<li>Write a function Aconstruct(), which takes as input <em>n </em>and returns, as output, the matrix <em>A </em>defined in Eq. 14 and its number of non-zero elements <em>nz</em>. Test your function in a script ex2c.m for <em>n </em>= 10 and compare your results with those you obtained in point (a). Furthermore, within the same script, visualise the non-zero structure of matrix <em>A </em>by using the command spy().</li>
<li>Using again the spy() command, visualize side by side the original matrix <em>A </em>and the result of the Cholesky factorization (chol() in Matlab).</li>
<li>Explain why, for <em>n </em>= 100<em>,</em>000, using chol() to solve <em>Ax </em>= <em>b </em>for a given right-hand-side vector <em>b </em>would be problematic. Are there ways to mitigate this issue?</li>
</ol>
<h2>7. Degree Centrality [5 points]</h2>
In graph theory and network analysis, centrality refers to indicators which identify the most important vertices within a graph. Applications include identifying the most influential person(s) in a social network, key infrastructure nodes in the Internet or urban networks, and super spreaders of disease. Here we are interested in the Degree centrality, which is conceptually simple. It is defined as the number of links incident upon a node (i.e., the number of vertices that a node has). The degree centrality of a vertex <em>v</em>, for a given graph <em>G </em>:= (<em>V,E</em>) with |<em>V </em>| vertices and |<em>E</em>| edges, is defined as the numbers of edges of vertex <em>v</em>.

Compute the degree centrality for the top 5 authors. Include them in an ordered list, and show the authors, the their coauthors and the degree centrality.

<h2>8. The Connectivity of the Coauthors [5 points]</h2>
How many coauthors have the authors in common? Think about a general procedure that allows you to compute the list of common coauthors of two authors and express it in matrix notation. Use the formula you derived to compute the common coauthors of the pairs (Golub, Moler), (Golub, Saunders), and (TChan, Demmel). Who are these common coauthors? Report their names.

<h2>9. PageRank of the Coauthor Graph [5 points]</h2>
Compute the PageRank value (e.g., by using a modified version of pagerank.m from Project 1) for all authors and provide a graph of all authors in descending order according to the PageRank. Include your script in the submission.

<h1>Quality of the code and of the report [15 Points]</h1>
The highest possible score of each project is 85 points and up to 15 additional points can be awarded based on the quality of your report and code (maximum possible grade: 100 points). Your report should be a coherent document, structured according to the template provided on iCorsi. If there are theoretical questions, provide a complete and detailed answer. All figures must have a caption and must be of sufficient quality (include them either as .eps or .pdf). If you made a particular choice in your implementation that might be out of the ordinary, clearly explain it in the report. The code you submit must be self-contained and executable, and must include the set-up for all the results that you obtained and listed in your report. It has to be readable and, if particularly complicated, well-commented.

<h1>Additional notes and submission details</h1>
Summarize your results and experiments for all exercises by writing an extended LaTeX report, by using the template provided on iCorsi (<a href="https://www.icorsi.ch/course/view.php?id=16926">https://www.icorsi.ch/course/view.php?id=16926</a><a href="https://www.icorsi.ch/course/view.php?id=16926">)</a>. Submit your gzipped archive file (tar, zip, etc.) – named projectnumberlastnamefirstname.zip/tgz – on iCorsi (see <em>[NC 2023] Project 1 – Submission PageRank Algorithm</em>) before the deadline. Submission by email or through any other channel will not be considered. Late submissions will not be graded and will result in a score of 0 points for that project. You are allowed to discuss all questions with anyone you like, but: (i) your submission must list anyone you discussed problems with and (ii) you must write up your submission independently. Please remember that plagiarism will result in a harsh penalization for all involved parties.

<h1>In-class assistance</h1>
If you experience difficulties in solving the problems above, please join us in class either on Tuesdays 15:30-17:00 or on Wednesdays 13:30-15:00 in room C1.03.

<h1>References</h1>
<ul>
<li>The power method and variants, Chapter 8: Eigenvalues and Singular Values, SIAM Book “A First Course on Numerical Methods”, C. Greif, U. Ascher, pp. 219-229.</li>
<li>Power iteration, <a href="https://en.wikipedia.org/wiki/Power_iteration">http://en.wikipedia.org/wiki/Power_iteration</a></li>
<li>Inverse iteration, <a href="https://en.wikipedia.org/wiki/Inverse_iteration">http://en.wikipedia.org/wiki/Inverse_iteration</a></li>
</ul>
<a href="#_ftnref1" name="_ftn1">[1]</a> The first part is originally based on a SIAM book chapter from <em>Numerical Computing with Matlab </em>by Cleve B. Moler.

<a href="#_ftnref2" name="_ftn2">[2]</a> The second part is originally based on a blog by Cleve B. Moler, who wrote a fantastic blog post about the Lake Arrowhead graph, and John Gilbert, who initially created the coauthor graph from the 1993 Householder Meeting. You can find more information at <a href="http://blogs.mathworks.com/cleve/2013/06/10/lake-arrowhead-coauthor-graph/">http:</a>

<a href="http://blogs.mathworks.com/cleve/2013/06/10/lake-arrowhead-coauthor-graph/">//blogs.mathworks.com/cleve/2013/06/10/lake-arrowhead-coauthor-graph/</a><a href="http://blogs.mathworks.com/cleve/2013/06/10/lake-arrowhead-coauthor-graph/">.</a>

<a href="#_ftnref3" name="_ftn3">[3]</a> see ”Estimating search engine index size variability” by van den Bosch et al., Scientometrics, <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4833824/">https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4833824/</a>

<a href="#_ftnref4" name="_ftn4">[4]</a> <a href="https://en.wikipedia.org/wiki/Gene_H._Golub">http://en.wikipedia.org/wiki/Gene_H._Golub</a>
