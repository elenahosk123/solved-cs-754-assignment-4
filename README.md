Download Link: https://assignmentchef.com/product/solved-cs-754-assignment-4
<br>
Advanced Image Processing




<ol>

 <li>Consider a signal f = f1 + f2 + η where f1 is a sparse linear combination of cosine waves with integer frequencies (i.e. sparse in DCT basis) and f2 is a signal consisting of a small number of spikes. η represents noise from N(0, σ<sup>2</sup>) where σ = 0.01× average value of f1 + f2. Consider that f is a 1D discrete signal with 256 elements. Your job is to implement any technique of your choice to separate f into f1 and f2. That is, you are given only f (which is noisy) and you want to estimate f1 and f2. Experimentally study the quality of the estimation of both components (in terms of relative reconstruction error for both f1 and f2) with (a) varying σ and fixed s, and (b) varying sparsity level s with fixed σ. You may assume for simplicity that s is same for both. Include all relevant plots in your report, and mention which technique you used. Comment on these results.</li>

</ol>

Now suppose that the magnitude of f2 was k times that of f1. Study the effect of varying k on the RMSE of both signals, on the same algorithm. Again, include the relevant plot and comments in your report. You may use any ready-made CS solver – examples are your own implementation of ISTA, OMP or solvers such as L1 LS, SPGL1, YALL1, L1-MAGIC (MATLAB codes for all are freely downloadable from the web). In all cases, state how you picked the relevant parameters for the solver or algorithm. [20 points]

<ol start="2">

 <li>We have studied two greedy algorithms for compressive recovery in class – MP and OMP. Your task is to do a google search and find out a research paper that proposes a greedy algorithm for CS recovery that is different from OMP and MP. Write down the algorithm in your report in the form of a simple pseudo-code. State the key theorem from the paper which presents performance bounds for the algorithm, and explain the meaning of the terms involved. If there are multiple theorems, pick the one that states the strongest result. [20 points]</li>

 <li>Consider that you learned a dictionary D to sparsely represent a certain class S of images – say handwritten alphabet or digit images. How will you convert D to another dictionary which will sparsely represent the following classes of images? Note that you are not allowed to learn the dictionary all over again, as it is time-consuming.</li>

</ol>

<ul>

 <li>Class S1 which consists of images obtained by applying a known derivative filter to the images in S.</li>

 <li>Class S2 which consists of images obtained by rotating a subset of the images in class S by a known fixed angle α, and the other subset by another known fixed angle /3.</li>

 <li>Class S3 which consists of images obtained by applying an intensity transformation Ii new(x, y) = α(Ii <sub>old</sub><sub>(</sub><sub>x,</sub> y))2 + /3(Ii <sub>old</sub><sub>(</sub><sub>x,</sub> y)) + ‘y to the images in S, where α, /3, ‘y are known.</li>

</ul>




<ul>

 <li>Class S4 which consists of images obtained by applying a known blur kernel to the images in S.</li>

 <li>Class S5 which consists of images obtained by applying a blur kernel which is known to be a linear combination of blur kernels belonging to a known set B, to the images in S. [4+4+4+4+4=20 points]</li>

</ul>

<ol start="4">

 <li>How will you solve for the minimum of the following objective functions: (1) J(A<strong><sub>r</sub></strong>) = IA − A<strong>r</strong>I2 <sub>F</sub> , where A is a known m x n matrix of rank greater than r, and A<strong><sub>r</sub></strong> is a rank-r matrix, where r &lt; m, r &lt; n. (2) J(R) = IA − RBI2 <sub>F</sub> , where A E R<sup>n×m</sup>,B E R<sup>n×m</sup>,R E R<sup>n×n</sup>,m &gt; n and R is constrained to be Note that A and B are both known.</li>

</ol>

In both cases, explain briefly any one situation in image processing where the solution to such an optimization problem is required. [5+5+5+5=20 points]

<ol start="5">

 <li>Read the paper ‘A Signal Processing Perspective on Hyperspectral Unmixing’, a copy of which is placed in the homework folder. Answer the following questions:</li>

</ol>

<ul>

 <li>What is hyperspectral unmixing? You may use an equation to support your answer with symbol meanings carefully explained.</li>

 <li>In equation 40 of the paper, explain how non-negative matrix factorization is used for hyperspectral</li>

 <li>Explain the improvement to non-negative matrix factorization proposed in equation 41 of the paper. (You may explain any two forms each for g and h.) [6+6+8=20 points]</li>

</ul>