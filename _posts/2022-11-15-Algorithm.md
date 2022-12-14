---
keywords: fastai
title: Algorithms
toc: true 
badges: true
comments: true 
categories: [markdown, week 8]
nb_path: _notebooks/2022-11-15-Algorithm.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-11-15-Algorithm.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="A-little-review-on-Algorithms:">A little review on Algorithms:<a class="anchor-link" href="#A-little-review-on-Algorithms:"> </a></h4><p>what are the three components of an algorithm?</p>
<ul>
<li>sel<strong>__</strong></li>
<li>seq<strong>__</strong></li>
<li>it<strong>___</strong></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Today we will be looking at algorithms from another standpoint.
<br>Q: How many ways are there to peel a banana? Is the result the same?</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Main-Idea-1:">Main Idea 1:<a class="anchor-link" href="#Main-Idea-1:"> </a></h3><h4 id="Algorithms-can-be-written-in-different-ways-and-still-do-the-same-thing">Algorithms can be written in different ways and still do the same thing<a class="anchor-link" href="#Algorithms-can-be-written-in-different-ways-and-still-do-the-same-thing"> </a></h4><ul>
<li>However, Algorithms that look similar might not always have the same result</li>
<li>Different algorithms can be used to solve the same problem</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Examples!">Examples!<a class="anchor-link" href="#Examples!"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The goal with the two algorithms below is to show "Wow! Good job!" when you get an A and show "Nice!" when you get a B or C (pass), if you don't pass (lower than 70) it will show "Do Better"</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What Grade Did You Get?&quot;</span><span class="p">)</span>
<span class="n">grade</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter Grade:&quot;</span><span class="p">))</span>
<span class="k">if</span> <span class="n">grade</span> <span class="o">&gt;=</span> <span class="mi">90</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Wow! Good job!&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="mi">70</span> <span class="o">&lt;=</span> <span class="n">grade</span> <span class="o">&lt;</span> <span class="mi">90</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Nice!&quot;</span><span class="p">)</span>
<span class="k">elif</span> <span class="n">grade</span> <span class="o">&lt;</span> <span class="mi">70</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Do Better&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>What Grade Did You Get?
Nice!
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>yay! it worked! Lets look at the next one. Do you notice any differences? Do you think this algorithm will still achieve the same goal? If not, what is the flaw?</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What Grade Did You Get?&quot;</span><span class="p">)</span>
<span class="n">grade</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter Grade:&quot;</span><span class="p">))</span>
<span class="k">if</span> <span class="n">grade</span> <span class="o">&gt;=</span> <span class="mi">90</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Wow! Good job!&quot;</span><span class="p">)</span>
<span class="k">elif</span> <span class="mi">70</span> <span class="o">&lt;</span> <span class="n">grade</span> <span class="o">&lt;</span> <span class="mi">90</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Nice!&quot;</span><span class="p">)</span>
<span class="k">elif</span> <span class="n">grade</span> <span class="o">&lt;</span> <span class="mi">70</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Do Better&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>What Grade Did You Get?
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="So,-why-is-this-important?-Why-are-we-even-doing-this?">So, why is this important? Why are we even doing this?<a class="anchor-link" href="#So,-why-is-this-important?-Why-are-we-even-doing-this?"> </a></h4><p>when 2 algorithms look extremely similar, it is easy to assume they do the same thing. However, that is not the case and we have learn how to notice small differences in code and pretty much debug.
<br>- just know that codes that look similar don't always produce the same things:)</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Real-life-situation-(Storytime)">Real-life situation (Storytime)<a class="anchor-link" href="#Real-life-situation-(Storytime)"> </a></h4><p>Tommy and Billy are working on solving the same issue with an algorithm<br>
Tommy creates a functioning code and yells "I did it!"<br>
He looks over at his friend Billy which is having a bit of trouble and he offers help<br>
However, Billy's code looks basically the same! which confuses them<br>
Then they remeber that they were taught that algorithms that look similar don't always have the same results and they collaborate to do further investigation:)</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, without running, investigate the algorithm below. This one looks different. Do you thing it will still achieve the same goal as above?</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What Grade Did You Get?&quot;</span><span class="p">)</span>
<span class="n">grade</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter Grade:&quot;</span><span class="p">))</span>
<span class="n">A</span> <span class="o">=</span> <span class="n">grade</span> <span class="o">&gt;=</span> <span class="mi">90</span>
<span class="n">B</span> <span class="o">=</span> <span class="mi">70</span> <span class="o">&lt;=</span> <span class="n">grade</span> <span class="o">&lt;</span> <span class="mi">90</span>
<span class="n">C</span> <span class="o">=</span> <span class="n">grade</span> <span class="o">&lt;</span> <span class="mi">70</span>
<span class="k">if</span> <span class="n">A</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Wow! Good job!&quot;</span><span class="p">)</span>
<span class="k">elif</span> <span class="n">B</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Nice!&quot;</span><span class="p">)</span>
<span class="k">elif</span> <span class="n">C</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Do Better&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>What Grade Did You Get?
Do Better
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Why is this important?<br>
When collaborating or working on group projects, two people might come up with two different ways to solve a problem, and that happens a lot.</p>
<ul>
<li>know that same goal can be achieved in many ways (the possibilities are endless)</li>
<li>make notes in you code! (explain how it works to others or you future self)</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Hacks:">Hacks:<a class="anchor-link" href="#Hacks:"> </a></h4><p>Make your own version of this!
<br>requirements:</p>
<ul>
<li>main goal of algorithm </li>
<li>main/base algorithm (ideal algorithm)</li>
<li>an algorithm that visual looks like the first one but is flawed, has a different result, or both<ul>
<li>explain the flaw either in notes of your code or in a markdown</li>
</ul>
</li>
<li>an algorithm that looks very different from first algorithm but has some result/ solves the same problem<ul>
<li>explanation/ comparison of this algorithm with the first one</li>
</ul>
</li>
</ul>
<p><br>The Algorithms don't have to be super complicated! But it should be complex enough to show a good understanding of this lesson as well as previous ones</p>
<p><br>Scoring Rubric:</p>
<ul>
<li>0.05 for an interesting goal</li>
<li>0.05 for a well completed main algorithm</li>
<li>0.05 for algorithm that looks the same but is different</li>
<li>0.05 for algorithm that looks different but is the same</li>
<li>0.05 for explanation of both algorithms above</li>
<li>total: 0.25 <br></li>
</ul>
<h4 id="Extra-things-to-add-to-notes:)">Extra things to add to notes:)<a class="anchor-link" href="#Extra-things-to-add-to-notes:)"> </a></h4><p><br></p>
<ul>
<li>why having this understanding of algorithms is important to you as a coder</li>
</ul>

</div>
</div>
</div>
</div>
 

