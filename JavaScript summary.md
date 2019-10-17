<h1 id="javascript-summary">JavaScript summary</h1>
<p>These are my notes from learning the JavaScript language. I have used several resources to learn the language, the notes are inspired from all these resources. I have used two Udemy courses, a book, online resources and two learning environments.</p>
<p>The Udemy courses:<br>
<a href="https://www.udemy.com/course/understand-javascript/">JavaScript: Understanding the Weird Parts</a><br>
<a href="https://www.udemy.com/course/advanced-javascript-concepts/">Advanced JavaScript Concepts</a></p>
<p>Text resources:<br>
<a href="https://eloquentjavascript.net/Eloquent_JavaScript.pdf">Eloquent Javascript</a><br>
<a href="https://developer.mozilla.org/en/docs/Web/JavaScript">MDN JavaScript docs</a></p>
<p>The learning environments:<br>
<a href="https://learn.freecodecamp.org/">FreeCodeCamp</a><br>
<a href="https://www.codecademy.com/learn/introduction-to-javascript">CodeCademy</a></p>
<h2 id="language-characteristics">Language characteristics</h2>
<p><strong>Syntax parsers</strong><br>
A program that reads your code and determines what it does and if it’s grammar is valid.</p>
<p><strong>Single threaded</strong><br>
One set of instructions is executed every single time. It has only one call stack. Web API requests are asynchronous.</p>
<p><strong>Deterministic</strong><br>
Whatever we put into the parameters it always returns the same values.</p>
<h2 id="scope">Scope</h2>
<p><strong>Scope chain</strong><br>
Scope chain <a href="https://repl.it/@aneagoie/Scope-Chain">example</a>. Scope leakage <a href="https://repl.it/@aneagoie/JS-is-Weird">example</a>.</p>
<p><strong>Function scope vs block scope</strong><br>
Block scoping means declaring a variable not just inside a function, but around any curly brackets.</p>
<h2 id="lexical">Lexical</h2>
<p><strong>Hoisting</strong><br>
The behavior of moving the variables (only var) and functions to the top of their respective environment (during compilation). Use let or const keyword to prevent hoisting. Hoisting <a href="https://repl.it/@aneagoie/hoisting-exe">example</a>.</p>
<p><strong>Lexical environment</strong><br>
Where you write something. Used so compiler can understand where to put things/what actions to undertake.</p>
<p><strong>Lexical scope</strong><br>
In JavaScript our lexical scope (available data + variables where the function was defined) determines our available variables. Not where the function is called (dynamic scope).</p>
<p><strong>IIFE pattern</strong><br>
Explained in this Udemy lesson.</p>
<p><strong>Execution context</strong><br>
Execution context tells you which lexical environment is running. There are lots of lexical environments. Which one is currently running is managed via execution contexts. It can contain things beyond what you’ve written in your code. Each execution context has it’s own variable environment.</p>
<p><strong>Variable environment</strong><br>
Each execution context has it’s own variable environment. <a href="https://repl.it/@aneagoie/Variable-Environment">Example</a>.</p>
<p>Types of execution context:</p>
<ul>
<li>Global</li>
<li>Local</li>
</ul>
<p>Global execution context:</p>
<ul>
<li>this</li>
<li>arguments</li>
<li>window</li>
</ul>
<h2 id="syntax">Syntax</h2>
<p><strong>Variables</strong></p>
<p><strong>Operators</strong></p>
<p><strong>Functions</strong></p>
<p><strong>Modules</strong><br>
Exporting modules.</p>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">function</span> <span class="token function">function1</span><span class="token punctuation">(</span>p1<span class="token punctuation">,</span> p2<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"function 1"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>

<span class="token keyword">function</span> <span class="token function">function1</span><span class="token punctuation">(</span>p1<span class="token punctuation">,</span> p2<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"function 1"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>

<span class="token keyword">export</span> <span class="token punctuation">{</span> function1<span class="token punctuation">,</span> function2<span class="token punctuation">}</span><span class="token punctuation">;</span>
</code></pre>

