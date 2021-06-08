<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# isProbability

> Test if a numeric value is a probability.

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-assert-is-probability
```

</section>

<section class="usage">

## Usage

```javascript
var isProbability = require( '@stdlib/math-base-assert-is-probability' );
```

#### isProbability( x )

Tests if a `numeric` value is a probability.

```javascript
var bool = isProbability( 0.5 );
// returns true

bool = isProbability( 3.14 );
// returns false

bool = isProbability( NaN );
// returns false
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var randu = require( '@stdlib/random-base-randu' );
var isProbability = require( '@stdlib/math-base-assert-is-probability' );

var bool;
var x;
var i;

for ( i = 0; i < 100; i++ ) {
    x = ( randu()*2.0 ) - 1.0;
    bool = isProbability( x );
    console.log( '%d is %s', x, ( bool ) ? 'a probability' : 'not a probability' );
}
```

</section>

<!-- /.examples -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-assert-is-probability/main/LICENSE

</section>

<!-- /.links -->
