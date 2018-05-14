### Kotlin at SPS Commerce
<img src="https://avatars0.githubusercontent.com/u/1446536?s=400&v=4" style="border:none; box-shadow: 0 0 0px rgba(0, 0, 0, 0);background:rgba(255, 255, 255, 0);"/>
#### Ben Lipson
---
### Intro
<div class="fragment">
    <img src="https://algeria20.com/wp-content/uploads/2017/11/jet.png" style="border:none; box-shadow: 0 0 0px rgba(0, 0, 0, 0);background:rgba(255, 255, 255, 0);">
    <ul>
        <li class="fragment">Statically typed</li>
        <li class="fragment">Type inference</li>
        <li class="fragment">Runs on the JVM</li>
        <li class="fragment">Interoperable with Java</li>
        <li class="fragment">Java-compatible bytecode or ES5</li>
    </ul>
</div>
---
### Why?
<ul style="margin-left: 0%">
    <li class="fragment">Easy</li>
    <li class="fragment">Costs nothing</li>
    <li class="fragment">Flexible</li>
    <li class="fragment">Popular</li>
    <li class="fragment">Like Java, but better</li>
</ul>
---
### Concise
<pre class="fragment" style="display:inline-block; width: auto"><code data-trim data-noescape>
data class Company(val uid: Int, val name: String)
</code></pre>
<pre class="fragment" style="display:inline-block; width: auto"><code data-trim data-noescape>
val positiveNumbers = list.filter { it > 0 }
</code></pre>
<pre class="fragment" style="display:inline-block; width: auto"><code data-trim data-noescape>
object ThisIsASingleton {
    val companyName: String = "SPS Commerce"
}
</code></pre>
---
### Safe
<pre class="fragment" style="display:inline-block; width: auto"><code data-trim data-noescape>
var output: String
output = null   // Compilation error
</code></pre>
<pre class="fragment" style="display:inline-block; width: auto"><code data-trim data-noescape>
val name: String? = null    // Nullable type
println(name.length())      // Compilation error
</code></pre>
<pre class="fragment" style="display:inline-block; width: auto"><code data-trim data-noescape>
fun calculateTotal(obj: Any) {
    if (obj is Company) {
        return obj.name
    }
}
</code></pre>
---
# Live Demo
---
### Cons
<ul style="margin-left: 0%; font-size: 75%;">
    <li class="fragment">Bilingualism</li>
    <ul>
        <li class="fragment">Syntactically  more similar than most Java libraries (Vavr, Lombok, Camel, etc...)</li>
        <li class="fragment">Conversion Tool</li>
    </ul>
    <li class="fragment">Reflection</li>
    <ul>
        <li class="fragment">JDBI and annotations</li>
        <li class="fragment">Workarounds</li>
    </ul>
    <li class="fragment">Conversion Tool Code Style</li>
    <ul>
        <li class="fragment">Conversion Tool Shouldn't Be Your Only Tool</li>
    </ul>
    <li class="fragment">Inaccurate Code Coverage Reports With Inline Functions</li>
    <ul>
        <li class="fragment">Code Coverage Shouldn't Be Required</li>
    </ul>
</ul>
