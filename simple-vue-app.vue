/* Create a Vue app running on a Web Page
The whole Vue library is based on Vue instances, which are mediators
between your View and your data. 
So we need to create a new Vue instance to start our app */


/* The Vue constructor is called with the new keyword to create a new instance.
It has one argument--the option object. It can have multiple attributes (called options) 
For now we are only using two of them: el and data.
el: mounts the Vue Instance on our web page using a CSS selector.
data: we initialise some data with a message property "some text etc"
We can alternatively use the $mount method of the Vue instance instead of the 
el option e.g.
	var app = New Vue({
		data () {
			return { message: 'Hello Vue.js!',}
		}.
	})
	// add the instance to the page
	app.$mount('#root')
*/
	
// New Vue instance
var app = new Vue()
	// CSS selector of the root DOM element
	el: '#root',
	// Some data
	data () {
		return {
			message: 'Hello Vue.js!',
		}
	},
})

<html>
<!-- From Vue.js 2 Web Project Development -->
<head>
	<meta charset="utf-8">
	<title>Vue Project Guide setup</title>
<head>
<body>

<!-- Include the library in the page -->
<script src="https://unpkg.com/vue/dist/vue.js"></script>

	<!-- Some HTML --> 
	<div id="root">
		<p>Is this an Hello world ?</p>
	</div>

	<!-- Some JavaScript --> 
	<script>
		console.log('Yes! We are using Vue version', Vue.version)
	</script>

</body>
</html>
