<h1>About</h1>
<p>
	Being able able to make asynchronous requests and inlining any processing in the form of map, each and reduce is very powerfull. Don't really need to wait for JavaScript generators to take advantage of clean asynchronous programming. 
</p>
<p>
	Time to take a lesson from C#.
</p>

<h3>Example Usage</h3>
<code>
	var dfd = $.Deferred();
  
	_(dfd).map(function(v) {
		console.log("Value: ", v);
	});

	console.log("Now resolving deferred collection.");
	dfd.resolve([1,2,3,4]);


	//Example output:
	> Now resolving deferred collection.
	> Value: 1
	> Value: 2
	> Value: 3
	> Value: 4
</code>

<h3>Road Map</h3>
<p>
	Lots of thing I'd like to do. I think Underscore.js is becoming the practical JS developer utility that it should have been long time ago. The thing its weak on is in the department of Deferreds which jQuery has done well in.
</p>

<ul>
	<li>Get rid of jQuery dependency and use underscore.deferred.js</li>
	<li>Some task.js integration. Who needs to wait for generators.</li>
	<li>Specialized map, each, and reduce methods that can deal with arrays of deferreds.</li>
	<li>Anything else?</li>
</ul>