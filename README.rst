
Installation & Usage
====================
This is a standalone version of refract - it can be installed with NPM:

.. code-block:: 
	
	npm install refract

And used just as a regular JavaScript library:

.. code-block:: javascript

	import refract, {render, Component} from 'refract';
	
Due to its nature, refract can consume JSX - just don't forget to hook up the Babel together with React preset:

.. code-block:: javascript

	/** @jsx refract.createElement */
	render(<div>Hello World!</div>, document.getElementById('root'));
	
Notice that `@jsx` pragma comment - without it Babel will fail to tie proper element factory function. Check :code:`example` folder for a bigger snippet.

License
=======
refract is licensed under the MIT License, what allows you to use it for basically anything absolutely for free. It would be great if somebody will find it useful.
