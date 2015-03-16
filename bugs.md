Bugs
====

- [ ] [range](https://github.com/compute-io/range)
	-	if empty input `array`, should return `null`.
- [x] [median](https://github.com/compute-io/median)
	-	if empty input `array`, should return `null`.
- [ ] [quantiles](https://github.com/compute-io/quantiles)
	-	if empty input `array`, should return `null`.
- [ ] [incrspace](https://github.com/compute-io/incrspace)
	-	increment allowed to be 0!!! allows for infinite length. May want to check also that len is not infinite in the event of a small enough incr. Should top out at maximum array length. Throw error: maximum array length exceeded.
- [ ] [lcm](https://github.com/compute-io/lcm)
	-	README calls `gcd` rather than `lcm` in #usage
- [ ] [unique](https://github.com/compute-io/unique)
	-	should return a reference to the input `array`
	-	should provide `copy` option
	-	should provide an accessor option (for accessing numeric values)
- [ ] [linspace](https://github.com/compute-io/linspace)
	-	when number of elements equals 1, returns the upper bound
	-	handle 0 element case

 
