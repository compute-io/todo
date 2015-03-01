Update
======


### General

1. where applicable, if a function can accept non-numeric arrays (e.g., when using accessors), then the fcn desc should __not__ stipulate numeric arrays
	-	descriptions are present in
		* 	`package.json`
		*	`README.md` (multiple places)
		*	`lib/index.js` (possibly multiple places)
2. 



### README

1. update mocha link in tests#unit section: http://mochajs.org
2. command for viewing an HTML version of the coverage report should be
	``` bash
	$ make view-cov
	in usage section, remove the line "To use the module"
4. API documentation/use should follow precedent established in later modules.
	- 	e.g., compare [compute-sum](https://github.com/compute-io/sum) with [compute-prod](https://github.com/compute-io/prod)
	-	function options should be detailed and documented
		* e.g., function accessors where applicable
5. `move `---` from above the copyright section to above the license section
6. example in examples section should begin by using `require` to load the module (i.e., include the `require` statement)
7. 


### Dotfiles

Every repository should include the following dotfiles...

1. `.gitattributes`
2. `.gitignore`
3. `.editorconfig`
4. `.jshintrc`
5. `.jshintignore`
6. `.npmignore`
7. `.travis.yml`

When updating modules, you are encouraged to simply replace any existing dotfile of the same name with a copy its corresponding file in the `update` directory of this repository. These dotfiles are the most recent iteration.


### Makefile

The `Makefile` included in the `update` directory should replace any existing file of the same name.


### package.json

1. all modules should use Chai `2.x.x` and Mocha `2.x.x`. Simply bump the major version from `1` to `2`.
2. verify keywords
3. update module description according to general task #1 above.
4. include `jshint` and `jshint-stylish` as `devDependencies`
	``` javascript
	...,
    "jshint": "2.x.x",
    "jshint-stylish": "^1.0.0",
	...
	```
5.



### lib/index.js

1. remove immediately invoked function wrapper, as not necessary
2. use [validate.io](https://github.com/validate-io) validators
	- 	see more recent modules for an example; e.g., [nanquantiles](https://github.com/compute-io/nanquantiles)
3. where applicable, support accessor option
	-	see more recent modules for examples; e.g., [prod](https://gitub.com/compute-io/prod) and [nanmedian](https://github.com/compute-io/nanmedian)
4. 


### examples/index.js

1. insert `'use strict'` at the top of the file
2. where possible, use compute-io modules (include as devDepedencies)
	e.g., when computing the sum, min, max, mean, etc
3.


### test/test.js

1. move `'use strict'` from inside the `describe` block to the top of file
2. above the `'use strict'` statement declare the global variables (for jshint)
	``` javascript
	/* global require, describe, it */
	```
	- 	Note: if other globals are used, e.g., `beforeEach`, `after`, etc, these should also be included. Check the lint errors.
3. 
