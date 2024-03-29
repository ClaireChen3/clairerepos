---
keywords: fastai
title: Review Guide 
toc: true 
badges: true
comments: true 
categories: [week 24] 
description: 
nb_path: _notebooks/2023-02-27-Review_Guide.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2023-02-27-Review_Guide.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Row-1:">Row 1:<a class="anchor-link" href="#Row-1:"> </a></h3><p>Video:</p>
<ul>
<li>input</li>
<li>program functionality</li>
<li>Output</li>
</ul>
<p>Written:</p>
<ul>
<li>describes the overall purpose of the program.</li>
<li>describes what functionality of the program is demonstrated in the video.</li>
<li>describes the input and output of the program demonstrated in the video.
<br><br></li>
</ul>
<p>My Response:</p>
<ul>
<li>This program’s purpose is to help women find remedies to their period symptoms and build a community where women can share what remedies work for them and help others</li>
<li>This program’s function is to provide a comment section where people can input the symptom they are addressing as well as the remedy for that symptom and check off the symptoms they experience in the checkbox to find remedies and products that can help</li>
<li>In the video, the user imputed the symptom they were addressing, cramps, and a remedy that worked for them which was tylenol. When the user clicked ‘post’ and ‘see all comments’, their comment was there even when the page was refreshed, the user’s comment was also saved into the database. The input was the symptom she imputed which was cramp, as well as the comment she imputed, which was tylenol, and the output was the same thing but displayed in the comments table. The comment is then stored in the database as a list</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Row-2:">Row 2:<a class="anchor-link" href="#Row-2:"> </a></h3><ul>
<li>one code segment that shows the data in this same list being used as part of fulfilling the program’s purpose.</li>
<li>one code segment that identifies the name of the variable representing the list being used in this response.</li>
<li>describes what the data contained in this list is representing in the program.
<br></li>
</ul>
<p>My Response:
The data contained in ‘myObj’ is the symptom and comment that is being added into the comment section to give other people advice on helping ease their period symptoms</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="n">function</span> <span class="n">addData</span><span class="p">(){</span>
    <span class="k">if</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;symptoms&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="o">&amp;&amp;</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;comment-box&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">){</span>
      <span class="n">myObj</span> <span class="o">=</span> <span class="p">{</span> <span class="s2">&quot;symptom&quot;</span><span class="p">:</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;symptoms&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">,</span> <span class="s2">&quot;comment&quot;</span><span class="p">:</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;comment-box&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">};</span>
      <span class="o">//</span><span class="n">alert</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;symptoms&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
      <span class="o">//</span><span class="n">alert</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;comment-box&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
      <span class="n">add_row</span><span class="p">(</span><span class="n">myObj</span><span class="p">);</span>
    <span class="p">}</span>
  <span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Row-3:">Row 3:<a class="anchor-link" href="#Row-3:"> </a></h3><ul>
<li>includes a program code segment that shows a list being used to manage complexity in the program.</li>
<li>explains how the named, selected list manages complexity in the program code by explaining why the program code could not be written, or how it would be written differently, without using this list.
<br></li>
</ul>
<p>My Response:</p>
<ul>
<li>This list 'myObj' manages complexity and the program code could not be written without it because getting the value of the symptom and the comment is needed to save them both in to the database. You could write two separate functions to add symptom and comment into a database, but it wouldn't be as concise, might lead to more errors in the code, and the inputs might not be stored together in the database which could also be confusing.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="n">function</span> <span class="n">addData</span><span class="p">(){</span>
    <span class="k">if</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;symptoms&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="o">&amp;&amp;</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;comment-box&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">){</span>
      <span class="n">myObj</span> <span class="o">=</span> <span class="p">{</span> <span class="s2">&quot;symptom&quot;</span><span class="p">:</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;symptoms&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">,</span> <span class="s2">&quot;comment&quot;</span><span class="p">:</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;comment-box&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">};</span>
      <span class="o">//</span><span class="n">alert</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;symptoms&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
      <span class="o">//</span><span class="n">alert</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;comment-box&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
      <span class="n">add_row</span><span class="p">(</span><span class="n">myObj</span><span class="p">);</span>
    <span class="p">}</span>
  <span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Row-4:">Row 4:<a class="anchor-link" href="#Row-4:"> </a></h3><ul>
<li>a code segment showing a student-developed procedure with at least one parameter that has an effect on the functionality of the procedure.</li>
<li>one code segment showing where the student-developed procedure is being called.</li>
<li>describes what the identified procedure does and how it contributes to the overall functionality of the program.
<br></li>
</ul>
<p>My Response:</p>
<ul>
<li><p>The first function "fHide" hides all the hyperlinks when you first click on the page by using a for loop to go through all the hyperlinks and changing their visibility to hidden.</p>
</li>
<li><p>Then the second function "fDisplay" also uses a for loop that goes through the checklist and looks for the ones that are checked. If it is checked, then it will change the visibility from hidden to not hidden, but if it is not checked, it will remain hidden.</p>
</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="o">//</span> <span class="n">this</span> <span class="n">function</span> <span class="n">hides</span> <span class="nb">all</span> <span class="n">the</span> <span class="n">links</span> <span class="n">at</span> <span class="n">first</span>
<span class="n">fHide</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">11</span><span class="p">);</span>
<span class="n">function</span> <span class="n">fHide</span><span class="p">(</span><span class="n">startIndex</span><span class="p">,</span> <span class="n">endIndex</span><span class="p">)</span> <span class="p">{</span>
  <span class="k">for</span> <span class="p">(</span><span class="n">var</span> <span class="n">i</span> <span class="o">=</span> <span class="n">startIndex</span><span class="p">;</span> <span class="n">i</span> <span class="o">&lt;=</span> <span class="n">endIndex</span><span class="p">;</span> <span class="n">i</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;s&quot;</span> <span class="o">+</span> <span class="n">i</span><span class="p">)</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;hidden&quot;</span><span class="p">;</span>
  <span class="p">}</span>
<span class="p">}</span>
<span class="o">//</span> <span class="n">when</span> <span class="n">this</span> <span class="n">function</span> <span class="ow">is</span> <span class="n">called</span><span class="p">,</span> <span class="n">it</span> <span class="n">will</span> <span class="n">display</span> <span class="n">the</span> <span class="n">remedies</span> <span class="n">to</span> <span class="n">the</span> <span class="n">symptoms</span> <span class="n">that</span> <span class="n">have</span> <span class="n">been</span> <span class="n">checked</span>
<span class="n">function</span> <span class="n">fDisplay</span><span class="p">(</span><span class="n">startIndex</span><span class="p">,</span> <span class="n">endIndex</span><span class="p">,</span> <span class="n">checkboxPrefix</span><span class="p">)</span> <span class="p">{</span>
  <span class="k">for</span> <span class="p">(</span><span class="n">var</span> <span class="n">i</span> <span class="o">=</span> <span class="n">startIndex</span><span class="p">;</span> <span class="n">i</span> <span class="o">&lt;=</span> <span class="n">endIndex</span><span class="p">;</span> <span class="n">i</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">var</span> <span class="n">checkboxId</span> <span class="o">=</span> <span class="n">checkboxPrefix</span> <span class="o">+</span> <span class="n">i</span><span class="p">;</span>
    <span class="n">var</span> <span class="n">element</span> <span class="o">=</span> <span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;s&quot;</span> <span class="o">+</span> <span class="n">i</span><span class="p">);</span>
    <span class="k">if</span> <span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="n">checkboxId</span><span class="p">)</span><span class="o">.</span><span class="n">checked</span><span class="p">)</span> <span class="p">{</span>
      <span class="n">element</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">;</span>
    <span class="p">}</span> <span class="k">else</span> <span class="p">{</span>
      <span class="n">element</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;hidden&quot;</span><span class="p">;</span>
    <span class="p">}</span>
  <span class="p">}</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Row-5:">Row 5:<a class="anchor-link" href="#Row-5:"> </a></h3><ul>
<li>includes a program code segment of a student developed algorithm that includes sequencing, selection, and iteration</li>
<li>explains in detailed steps how the identified algorithm works in enough detail that someone else could recreate it.</li>
</ul>
<p><br></p>
<p>My Response:</p>
<ul>
<li>For my function ‘fDisplay’, I used a for loop(iteration) and set the variable i to 1 and added one to i each time it ran until i reached 12. This results in the function checking all 11 of the symptoms in my checkbox and checking them for a certain condition. I then used an if statement(selection) to check if the checkboxes were checked off or not. If the condition of it being checked came out to be true, then the visibility of the corresponding hyperlink to that symptom would become visible. If not, the corresponding hyperlink to that symptom would remain hidden.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="o">//</span> <span class="n">when</span> <span class="n">this</span> <span class="n">function</span> <span class="ow">is</span> <span class="n">called</span><span class="p">,</span> <span class="n">it</span> <span class="n">will</span> <span class="n">display</span> <span class="n">the</span> <span class="n">remedies</span> <span class="n">to</span> <span class="n">the</span> <span class="n">symptoms</span> <span class="n">that</span> <span class="n">have</span> <span class="n">been</span> <span class="n">checked</span>
<span class="n">function</span> <span class="n">fDisplay</span><span class="p">(</span><span class="n">startIndex</span><span class="p">,</span> <span class="n">endIndex</span><span class="p">,</span> <span class="n">checkboxPrefix</span><span class="p">)</span> <span class="p">{</span>
    <span class="k">for</span> <span class="p">(</span><span class="n">var</span> <span class="n">i</span> <span class="o">=</span> <span class="n">startIndex</span><span class="p">;</span> <span class="n">i</span> <span class="o">&lt;=</span> <span class="n">endIndex</span><span class="p">;</span> <span class="n">i</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
      <span class="n">var</span> <span class="n">checkboxId</span> <span class="o">=</span> <span class="n">checkboxPrefix</span> <span class="o">+</span> <span class="n">i</span><span class="p">;</span>
      <span class="n">var</span> <span class="n">element</span> <span class="o">=</span> <span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;s&quot;</span> <span class="o">+</span> <span class="n">i</span><span class="p">);</span>
      <span class="k">if</span> <span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="n">checkboxId</span><span class="p">)</span><span class="o">.</span><span class="n">checked</span><span class="p">)</span> <span class="p">{</span>
        <span class="n">element</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">;</span>
      <span class="p">}</span> <span class="k">else</span> <span class="p">{</span>
        <span class="n">element</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;hidden&quot;</span><span class="p">;</span>
      <span class="p">}</span>
    <span class="p">}</span>
  <span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Row-6:">Row 6:<a class="anchor-link" href="#Row-6:"> </a></h3><ul>
<li>describes two calls to the selected procedure identified in written response. Each call must pass a different argument(s) that causes a different segment of code in the algorithm to execute.</li>
<li>describes the condition(s) being tested by each call to the procedure.</li>
<li>identifies the result of each call.</li>
</ul>
<p><br></p>
<p>My Response:</p>
<ul>
<li><p>fHide is called at the beginning of the code so that right as you click on the page all the hyperlinks start off being invisible.
The result of this call is the hyperlinks becoming invisible</p>
</li>
<li><p>fDisplay is called when you press the ‘See Remedies to Button’ so it gives you the link to the remedy of your symptom(s) after you submit your checklist.
The conditions being tested in this call is whether or not the checkbox is checked.
The result is it outputting the hyperlinks to the remedies to the corresponding symptoms that have been checked off</p>
</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="o">&lt;</span><span class="n">button</span> <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;button&quot;</span> <span class="nb">id</span><span class="o">=</span><span class="n">rem</span> <span class="n">onclick</span> <span class="o">=</span><span class="s2">&quot;fDisplay(1, 11, &#39;chk&#39;)&quot;</span> <span class="n">style</span> <span class="o">=</span> <span class="s2">&quot;color: white&quot;</span><span class="o">&gt;&lt;</span><span class="n">font</span> <span class="n">color</span><span class="o">=</span><span class="s2">&quot;darkred&quot;</span><span class="o">&gt;</span> <span class="n">See</span> <span class="n">Remedies</span> <span class="n">To</span><span class="p">:</span><span class="o">&lt;/</span><span class="n">font</span><span class="o">&gt;&lt;/</span><span class="n">button</span><span class="o">&gt;</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>lists: database, json, api</p>

</div>
</div>
</div>
</div>
 

