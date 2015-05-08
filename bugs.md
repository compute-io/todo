Bugs
====

- [x] [range](https://github.com/compute-io/range)
	-	if empty input `array`, should return `null`.
- [x] [median](https://github.com/compute-io/median)
	-	if empty input `array`, should return `null`.
- [ ] [quantiles](https://github.com/compute-io/quantiles)
	-	if empty input `array`, should return `null`.
- [x] [incrspace](https://github.com/compute-io/incrspace)
	-	increment allowed to be 0!!! allows for infinite length. May want to check also that len is not infinite in the event of a small enough incr. Should top out at maximum array length. Throw error: maximum array length exceeded.
	-	reassignment of input argument while mentioning `arguments` in fcn body
- [x] [lcm](https://github.com/compute-io/lcm)
	-	README calls `gcd` rather than `lcm` in #usage
- [ ] [unique](https://github.com/compute-io/unique)
	-	should return a reference to the input `array`
	-	should provide `copy` option
	-	should provide an accessor option (for accessing numeric values)
- [ ] [linspace](https://github.com/compute-io/linspace)
	-	when number of elements equals 1, returns the upper bound
	-	handle 0 element case
- [ ] [truncmean](https://github.com/compute-io/truncmean)
	-	reassignment of input argument while mentioning `arguments` in fcn body
- [ ] [tversky-index](https://github.com/compute-io/tversky-index)
	-	reassignment of input arguments while mentioning `arguments` in fcn body
- [ ] [zip](https://github.com/compute-io/zip)
	-	should inline copying of `arguments` to `args`
- [ ] [unzip](https://github.com/compute-io/unzip)
	-	reassignment of input argument while mentioning `arguments` in fcn body
- [ ] [mean](https://github.com/compute-io/mean)
	-	is welford's algorithm [sufficient](https://github.com/JuliaLang/julia/issues/199)
	-	see [haskell](http://www.serpentine.com/blog/2014/06/10/win-bigger-statistical-fights-with-a-better-jackknife/)
	- 	also affects any other "online" algorithm
- [ ] [variance](https://github.com/compute-io/variance)
	-	see discussion above re:mean
- [ ] [msum](https://github.com/compute-io/msum)
	-	code duplication (cases 2 and 3)


 
