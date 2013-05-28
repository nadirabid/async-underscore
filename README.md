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
</code>