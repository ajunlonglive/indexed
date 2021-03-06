Indexed
------
*for educational purposes ONLY ...*

[![Build Status](https://travis-ci.org/krakjoe/indexed.svg)](https://travis-ci.org/krakjoe/indexed)

This extension implements the following abstract:

	final class Indexed implements ArrayAccess, Countable {
		/* for ArrayAccess */
		public function offsetGet(int $index);
		public function offsetSet(int $index, $value);
		public function offsetExists(int $index) : bool;

		public function offsetUnset(int $index);
		/* for Countable */
		public function count() : int;

		public function __construct(int $size, array $data = []);
		public function resize(int $size);
		public function flip() : Indexed;
	}

This touches upon all of the following Zend subjects:

 - custom zend objects
 - implementing internal interfaces
 - paramters, optional parameters, return types
 - casting objects
 - interfacing with garbage collector
 - dealing with reference counting/copying
 - implementing cloning
 - implementing iteration
 - testing

[Here is a screencast discussing the extension, thanks to Edd Mann from Three Devs and a Maybe](https://www.youtube.com/watch?v=AloIn2t7bWc)
