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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# String Manipulation

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> String manipulation functions.

<section class="installation">

## Installation

```bash
npm install @dramaorg/magni-explicabo
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var string = require( '@dramaorg/magni-explicabo' );
```

#### string

Namespace containing string manipulation functions.

```javascript
var str = string;
// returns {...}
```

The namespace exposes the following string manipulation functions:

<!-- <toc pattern="*"> -->

<div class="namespace-toc">

-   <span class="signature">[`acronym( str[, options] )`][@dramaorg/magni-explicabo/acronym]</span><span class="delimiter">: </span><span class="description">generate an acronym for a given string.</span>
-   <span class="signature">[`base`][@dramaorg/magni-explicabo/base]</span><span class="delimiter">: </span><span class="description">base (i.e., lower-level) string functions.</span>
-   <span class="signature">[`camelcase( str )`][@dramaorg/magni-explicabo/camelcase]</span><span class="delimiter">: </span><span class="description">convert a string to camel case.</span>
-   <span class="signature">[`capitalize( str )`][@dramaorg/magni-explicabo/capitalize]</span><span class="delimiter">: </span><span class="description">capitalize the first character in a string.</span>
-   <span class="signature">[`codePointAt( string, position[, backward] )`][@dramaorg/magni-explicabo/code-point-at]</span><span class="delimiter">: </span><span class="description">return a Unicode code point from a string at a specified position.</span>
-   <span class="signature">[`constantcase( str )`][@dramaorg/magni-explicabo/constantcase]</span><span class="delimiter">: </span><span class="description">convert a string to constant case.</span>
-   <span class="signature">[`dotcase( str )`][@dramaorg/magni-explicabo/dotcase]</span><span class="delimiter">: </span><span class="description">convert a string to dot case.</span>
-   <span class="signature">[`endsWith( str, search[, len] )`][@dramaorg/magni-explicabo/ends-with]</span><span class="delimiter">: </span><span class="description">test if a string ends with the characters of another string.</span>
-   <span class="signature">[`first( str[, n][, options] )`][@dramaorg/magni-explicabo/first]</span><span class="delimiter">: </span><span class="description">return the first character(s) of a string.</span>
-   <span class="signature">[`forEach( str, [options,] clbk[, thisArg ] )`][@dramaorg/magni-explicabo/for-each]</span><span class="delimiter">: </span><span class="description">invokes a function for each character in a string.</span>
-   <span class="signature">[`format( str, ...args )`][@dramaorg/magni-explicabo/format]</span><span class="delimiter">: </span><span class="description">insert supplied variable values into a format string.</span>
-   <span class="signature">[`fromCodePoint( pt1[, pt2[, pt3[, ...]]] )`][@dramaorg/magni-explicabo/from-code-point]</span><span class="delimiter">: </span><span class="description">create a string from a sequence of Unicode code points.</span>
-   <span class="signature">[`headercase( str )`][@dramaorg/magni-explicabo/headercase]</span><span class="delimiter">: </span><span class="description">convert a string to HTTP header case.</span>
-   <span class="signature">[`kebabcase( str )`][@dramaorg/magni-explicabo/kebabcase]</span><span class="delimiter">: </span><span class="description">convert a string to kebab case.</span>
-   <span class="signature">[`last( str[, n][, options] )`][@dramaorg/magni-explicabo/last]</span><span class="delimiter">: </span><span class="description">return the last character(s) of a string.</span>
-   <span class="signature">[`lpad( str, len[, pad] )`][@dramaorg/magni-explicabo/left-pad]</span><span class="delimiter">: </span><span class="description">left pad a string.</span>
-   <span class="signature">[`ltrimN( str, n[, chars] )`][@dramaorg/magni-explicabo/left-trim-n]</span><span class="delimiter">: </span><span class="description">trim `n` characters from the end of a string.</span>
-   <span class="signature">[`ltrim( str )`][@dramaorg/magni-explicabo/left-trim]</span><span class="delimiter">: </span><span class="description">trim whitespace characters from the beginning of a string.</span>
-   <span class="signature">[`lowercase( str )`][@dramaorg/magni-explicabo/lowercase]</span><span class="delimiter">: </span><span class="description">convert a string to lowercase.</span>
-   <span class="signature">[`nextCodePointIndex( string[, fromIndex] )`][@dramaorg/magni-explicabo/next-code-point-index]</span><span class="delimiter">: </span><span class="description">return the position of the next Unicode code point in a string after a specified position.</span>
-   <span class="signature">[`nextGraphemeClusterBreak( string[, fromIndex] )`][@dramaorg/magni-explicabo/next-grapheme-cluster-break]</span><span class="delimiter">: </span><span class="description">return the next extended grapheme cluster break in a string after a specified position.</span>
-   <span class="signature">[`numGraphemeClusters( str )`][@dramaorg/magni-explicabo/num-grapheme-clusters]</span><span class="delimiter">: </span><span class="description">return the number of grapheme clusters in a string.</span>
-   <span class="signature">[`num2words( value[, options] )`][@dramaorg/magni-explicabo/num2words]</span><span class="delimiter">: </span><span class="description">convert a number to a word representation.</span>
-   <span class="signature">[`pad( str, len[, options] )`][@dramaorg/magni-explicabo/pad]</span><span class="delimiter">: </span><span class="description">pad a string.</span>
-   <span class="signature">[`pascalcase( str )`][@dramaorg/magni-explicabo/pascalcase]</span><span class="delimiter">: </span><span class="description">convert a string to Pascal case.</span>
-   <span class="signature">[`percentEncode( str )`][@dramaorg/magni-explicabo/percent-encode]</span><span class="delimiter">: </span><span class="description">percent-encode a UTF-16 encoded string according to RFC 3986.</span>
-   <span class="signature">[`prevGraphemeClusterBreak( string[, fromIndex] )`][@dramaorg/magni-explicabo/prev-grapheme-cluster-break]</span><span class="delimiter">: </span><span class="description">return the previous extended grapheme cluster break in a string before a specified position.</span>
-   <span class="signature">[`removeFirst( str[, n][, options] )`][@dramaorg/magni-explicabo/remove-first]</span><span class="delimiter">: </span><span class="description">remove the first character(s) of a string.</span>
-   <span class="signature">[`removeLast( str[, n][, options] )`][@dramaorg/magni-explicabo/remove-last]</span><span class="delimiter">: </span><span class="description">remove the last character(s) of a string.</span>
-   <span class="signature">[`removePunctuation( str )`][@dramaorg/magni-explicabo/remove-punctuation]</span><span class="delimiter">: </span><span class="description">remove punctuation characters from a string.</span>
-   <span class="signature">[`removeUTF8BOM( str )`][@dramaorg/magni-explicabo/remove-utf8-bom]</span><span class="delimiter">: </span><span class="description">remove a UTF-8 byte order mark (BOM) from the beginning of a string.</span>
-   <span class="signature">[`removeWords( str, words[, ignoreCase] )`][@dramaorg/magni-explicabo/remove-words]</span><span class="delimiter">: </span><span class="description">remove a list of words from a string.</span>
-   <span class="signature">[`repeat( str, n )`][@dramaorg/magni-explicabo/repeat]</span><span class="delimiter">: </span><span class="description">repeat a string a specified number of times and return the concatenated result.</span>
-   <span class="signature">[`replaceBefore( str, search, replacement )`][@dramaorg/magni-explicabo/replace-before]</span><span class="delimiter">: </span><span class="description">replace the substring before the first occurrence of a specified search string.</span>
-   <span class="signature">[`replace( str, search, newval )`][@dramaorg/magni-explicabo/replace]</span><span class="delimiter">: </span><span class="description">replace search occurrences with a replacement string.</span>
-   <span class="signature">[`reverse( str[, options] )`][@dramaorg/magni-explicabo/reverse]</span><span class="delimiter">: </span><span class="description">reverse a string.</span>
-   <span class="signature">[`rpad( str, len[, pad] )`][@dramaorg/magni-explicabo/right-pad]</span><span class="delimiter">: </span><span class="description">right pad a string.</span>
-   <span class="signature">[`rtrimN( str, n[, chars] )`][@dramaorg/magni-explicabo/right-trim-n]</span><span class="delimiter">: </span><span class="description">trim `n` characters from the end of a string.</span>
-   <span class="signature">[`rtrim( str )`][@dramaorg/magni-explicabo/right-trim]</span><span class="delimiter">: </span><span class="description">trim whitespace characters from the end of a string.</span>
-   <span class="signature">[`snakecase( str )`][@dramaorg/magni-explicabo/snakecase]</span><span class="delimiter">: </span><span class="description">convert a string to snake case.</span>
-   <span class="signature">[`splitGraphemeClusters( str )`][@dramaorg/magni-explicabo/split-grapheme-clusters]</span><span class="delimiter">: </span><span class="description">split a string by its grapheme cluster breaks.</span>
-   <span class="signature">[`startcase( str )`][@dramaorg/magni-explicabo/startcase]</span><span class="delimiter">: </span><span class="description">capitalize the first letter of each word in a string.</span>
-   <span class="signature">[`startsWith( str, search[, position] )`][@dramaorg/magni-explicabo/starts-with]</span><span class="delimiter">: </span><span class="description">test if a string starts with the characters of another string.</span>
-   <span class="signature">[`substringAfterLast( str, search[, fromIndex] )`][@dramaorg/magni-explicabo/substring-after-last]</span><span class="delimiter">: </span><span class="description">return the part of a string after the last occurrence of a specified substring.</span>
-   <span class="signature">[`substringAfter( str, search[, fromIndex] )`][@dramaorg/magni-explicabo/substring-after]</span><span class="delimiter">: </span><span class="description">return the part of a string after a specified substring.</span>
-   <span class="signature">[`substringBeforeLast( str, search )`][@dramaorg/magni-explicabo/substring-before-last]</span><span class="delimiter">: </span><span class="description">return the part of a string before the last occurrence of a specified substring.</span>
-   <span class="signature">[`substringBefore( str, search )`][@dramaorg/magni-explicabo/substring-before]</span><span class="delimiter">: </span><span class="description">return the part of a string before a specified substring.</span>
-   <span class="signature">[`graphemeClusters2iteratorRight( src[, mapFcn[, thisArg]] )`][@dramaorg/magni-explicabo/to-grapheme-cluster-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator which iterates from right to left over grapheme clusters.</span>
-   <span class="signature">[`graphemeClusters2iterator( src[, mapFcn[, thisArg]] )`][@dramaorg/magni-explicabo/to-grapheme-cluster-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator which iterates over grapheme clusters.</span>
-   <span class="signature">[`toWellFormed( str )`][@dramaorg/magni-explicabo/to-well-formed]</span><span class="delimiter">: </span><span class="description">create a new well-formed string.</span>
-   <span class="signature">[`trim( str )`][@dramaorg/magni-explicabo/trim]</span><span class="delimiter">: </span><span class="description">trim whitespace characters from the beginning and end of a string.</span>
-   <span class="signature">[`truncateMiddle( str, len[, seq] )`][@dramaorg/magni-explicabo/truncate-middle]</span><span class="delimiter">: </span><span class="description">truncate a string in the middle to a specified length.</span>
-   <span class="signature">[`truncate( str, len[, ending] )`][@dramaorg/magni-explicabo/truncate]</span><span class="delimiter">: </span><span class="description">truncate a string to a specified length.</span>
-   <span class="signature">[`uncapitalize( str )`][@dramaorg/magni-explicabo/uncapitalize]</span><span class="delimiter">: </span><span class="description">uncapitalize the first character of a string.</span>
-   <span class="signature">[`uppercase( str )`][@dramaorg/magni-explicabo/uppercase]</span><span class="delimiter">: </span><span class="description">convert a string to uppercase.</span>
-   <span class="signature">[`utf16ToUTF8Array( str )`][@dramaorg/magni-explicabo/utf16-to-utf8-array]</span><span class="delimiter">: </span><span class="description">convert a UTF-16 encoded string to an array of integers using UTF-8 encoding.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var getKeys = require( '@stdlib/utils/keys' );
var string = require( '@dramaorg/magni-explicabo' );

console.log( getKeys( string ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@dramaorg/magni-explicabo.svg
[npm-url]: https://npmjs.org/package/@dramaorg/magni-explicabo

[test-image]: https://github.com/dramaorg/magni-explicabo/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/dramaorg/magni-explicabo/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/dramaorg/magni-explicabo/main.svg
[coverage-url]: https://codecov.io/github/dramaorg/magni-explicabo?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/dramaorg/magni-explicabo.svg
[dependencies-url]: https://david-dm.org/dramaorg/magni-explicabo/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/dramaorg/magni-explicabo/tree/deno
[deno-readme]: https://github.com/dramaorg/magni-explicabo/blob/deno/README.md
[umd-url]: https://github.com/dramaorg/magni-explicabo/tree/umd
[umd-readme]: https://github.com/dramaorg/magni-explicabo/blob/umd/README.md
[esm-url]: https://github.com/dramaorg/magni-explicabo/tree/esm
[esm-readme]: https://github.com/dramaorg/magni-explicabo/blob/esm/README.md
[branches-url]: https://github.com/dramaorg/magni-explicabo/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/dramaorg/magni-explicabo/main/LICENSE

<!-- <toc-links> -->

[@dramaorg/magni-explicabo/acronym]: https://github.com/dramaorg/magni-explicabo/tree/main/acronym

[@dramaorg/magni-explicabo/base]: https://github.com/dramaorg/magni-explicabo/tree/main/base

[@dramaorg/magni-explicabo/camelcase]: https://github.com/dramaorg/magni-explicabo/tree/main/camelcase

[@dramaorg/magni-explicabo/capitalize]: https://github.com/dramaorg/magni-explicabo/tree/main/capitalize

[@dramaorg/magni-explicabo/code-point-at]: https://github.com/dramaorg/magni-explicabo/tree/main/code-point-at

[@dramaorg/magni-explicabo/constantcase]: https://github.com/dramaorg/magni-explicabo/tree/main/constantcase

[@dramaorg/magni-explicabo/dotcase]: https://github.com/dramaorg/magni-explicabo/tree/main/dotcase

[@dramaorg/magni-explicabo/ends-with]: https://github.com/dramaorg/magni-explicabo/tree/main/ends-with

[@dramaorg/magni-explicabo/first]: https://github.com/dramaorg/magni-explicabo/tree/main/first

[@dramaorg/magni-explicabo/for-each]: https://github.com/dramaorg/magni-explicabo/tree/main/for-each

[@dramaorg/magni-explicabo/format]: https://github.com/dramaorg/magni-explicabo/tree/main/format

[@dramaorg/magni-explicabo/from-code-point]: https://github.com/dramaorg/magni-explicabo/tree/main/from-code-point

[@dramaorg/magni-explicabo/headercase]: https://github.com/dramaorg/magni-explicabo/tree/main/headercase

[@dramaorg/magni-explicabo/kebabcase]: https://github.com/dramaorg/magni-explicabo/tree/main/kebabcase

[@dramaorg/magni-explicabo/last]: https://github.com/dramaorg/magni-explicabo/tree/main/last

[@dramaorg/magni-explicabo/left-pad]: https://github.com/dramaorg/magni-explicabo/tree/main/left-pad

[@dramaorg/magni-explicabo/left-trim-n]: https://github.com/dramaorg/magni-explicabo/tree/main/left-trim-n

[@dramaorg/magni-explicabo/left-trim]: https://github.com/dramaorg/magni-explicabo/tree/main/left-trim

[@dramaorg/magni-explicabo/lowercase]: https://github.com/dramaorg/magni-explicabo/tree/main/lowercase

[@dramaorg/magni-explicabo/next-code-point-index]: https://github.com/dramaorg/magni-explicabo/tree/main/next-code-point-index

[@dramaorg/magni-explicabo/next-grapheme-cluster-break]: https://github.com/dramaorg/magni-explicabo/tree/main/next-grapheme-cluster-break

[@dramaorg/magni-explicabo/num-grapheme-clusters]: https://github.com/dramaorg/magni-explicabo/tree/main/num-grapheme-clusters

[@dramaorg/magni-explicabo/num2words]: https://github.com/dramaorg/magni-explicabo/tree/main/num2words

[@dramaorg/magni-explicabo/pad]: https://github.com/dramaorg/magni-explicabo/tree/main/pad

[@dramaorg/magni-explicabo/pascalcase]: https://github.com/dramaorg/magni-explicabo/tree/main/pascalcase

[@dramaorg/magni-explicabo/percent-encode]: https://github.com/dramaorg/magni-explicabo/tree/main/percent-encode

[@dramaorg/magni-explicabo/prev-grapheme-cluster-break]: https://github.com/dramaorg/magni-explicabo/tree/main/prev-grapheme-cluster-break

[@dramaorg/magni-explicabo/remove-first]: https://github.com/dramaorg/magni-explicabo/tree/main/remove-first

[@dramaorg/magni-explicabo/remove-last]: https://github.com/dramaorg/magni-explicabo/tree/main/remove-last

[@dramaorg/magni-explicabo/remove-punctuation]: https://github.com/dramaorg/magni-explicabo/tree/main/remove-punctuation

[@dramaorg/magni-explicabo/remove-utf8-bom]: https://github.com/dramaorg/magni-explicabo/tree/main/remove-utf8-bom

[@dramaorg/magni-explicabo/remove-words]: https://github.com/dramaorg/magni-explicabo/tree/main/remove-words

[@dramaorg/magni-explicabo/repeat]: https://github.com/dramaorg/magni-explicabo/tree/main/repeat

[@dramaorg/magni-explicabo/replace-before]: https://github.com/dramaorg/magni-explicabo/tree/main/replace-before

[@dramaorg/magni-explicabo/replace]: https://github.com/dramaorg/magni-explicabo/tree/main/replace

[@dramaorg/magni-explicabo/reverse]: https://github.com/dramaorg/magni-explicabo/tree/main/reverse

[@dramaorg/magni-explicabo/right-pad]: https://github.com/dramaorg/magni-explicabo/tree/main/right-pad

[@dramaorg/magni-explicabo/right-trim-n]: https://github.com/dramaorg/magni-explicabo/tree/main/right-trim-n

[@dramaorg/magni-explicabo/right-trim]: https://github.com/dramaorg/magni-explicabo/tree/main/right-trim

[@dramaorg/magni-explicabo/snakecase]: https://github.com/dramaorg/magni-explicabo/tree/main/snakecase

[@dramaorg/magni-explicabo/split-grapheme-clusters]: https://github.com/dramaorg/magni-explicabo/tree/main/split-grapheme-clusters

[@dramaorg/magni-explicabo/startcase]: https://github.com/dramaorg/magni-explicabo/tree/main/startcase

[@dramaorg/magni-explicabo/starts-with]: https://github.com/dramaorg/magni-explicabo/tree/main/starts-with

[@dramaorg/magni-explicabo/substring-after-last]: https://github.com/dramaorg/magni-explicabo/tree/main/substring-after-last

[@dramaorg/magni-explicabo/substring-after]: https://github.com/dramaorg/magni-explicabo/tree/main/substring-after

[@dramaorg/magni-explicabo/substring-before-last]: https://github.com/dramaorg/magni-explicabo/tree/main/substring-before-last

[@dramaorg/magni-explicabo/substring-before]: https://github.com/dramaorg/magni-explicabo/tree/main/substring-before

[@dramaorg/magni-explicabo/to-grapheme-cluster-iterator-right]: https://github.com/dramaorg/magni-explicabo/tree/main/to-grapheme-cluster-iterator-right

[@dramaorg/magni-explicabo/to-grapheme-cluster-iterator]: https://github.com/dramaorg/magni-explicabo/tree/main/to-grapheme-cluster-iterator

[@dramaorg/magni-explicabo/to-well-formed]: https://github.com/dramaorg/magni-explicabo/tree/main/to-well-formed

[@dramaorg/magni-explicabo/trim]: https://github.com/dramaorg/magni-explicabo/tree/main/trim

[@dramaorg/magni-explicabo/truncate-middle]: https://github.com/dramaorg/magni-explicabo/tree/main/truncate-middle

[@dramaorg/magni-explicabo/truncate]: https://github.com/dramaorg/magni-explicabo/tree/main/truncate

[@dramaorg/magni-explicabo/uncapitalize]: https://github.com/dramaorg/magni-explicabo/tree/main/uncapitalize

[@dramaorg/magni-explicabo/uppercase]: https://github.com/dramaorg/magni-explicabo/tree/main/uppercase

[@dramaorg/magni-explicabo/utf16-to-utf8-array]: https://github.com/dramaorg/magni-explicabo/tree/main/utf16-to-utf8-array

<!-- </toc-links> -->

</section>

<!-- /.links -->
