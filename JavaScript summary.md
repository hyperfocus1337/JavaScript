<h2 id="javascript-summary">JavaScript summary</h2>
<p><strong>Syntax parsers</strong><br>
Testing</p>
<p><strong>Single threaded</strong><br>
One set of instructions is executed every single time. It has only one call stack. Web API requests are asynchronous.</p>
<p><strong>Hoisting</strong><br>
The behavior of moving the variables (only var) and functions to the top of their respective environment (during compilation). Use let or const keyword to prevent hoisting.</p>
<p><strong>Lexical environment</strong><br>
Used so compiler can understand where to put things/what actions to undertake.</p>
<p><strong>Lexical scope</strong><br>
In JavaScript our lexical scope (available data + variables where the function was defined) determines our available variables. Not where the function is called (dynamic scope).</p>
<p><strong>IIFE pattern</strong></p>
<p><strong>Execution context</strong><br>
Execution context tells you which lexical environment is running. Each execution context has it’s own variable environment.</p>
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

