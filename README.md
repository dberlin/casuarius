# casuarius
This is a Rust implementation of the Cassowary constraint solving algorithm
([Badros et. al 2001](https://constraints.cs.washington.edu/solvers/cassowary-tochi.pdf)).
It is a fork of [Dylan Ede's implementation](https://github.com/dylanede/cassowary-rs),
which is based heavily on the implementation for C++ at
[nucleic/kiwi](https://github.com/nucleic/kiwi). However, this implementation does
differ in from all others in some details.

Cassowary is designed for solving constraints to lay out user interfaces.
Constraints typically take the form "this button must line up with this
text box", or "this box should try to be 3 times the size of this other box".
Its most popular incarnation by far is in Apple's Autolayout
system for Mac OS X and iOS user interfaces. UI libraries using the Cassowary
algorithm manage to achieve a much more natural approach to specifying UI
layouts than traditional approaches like those found in HTML.

This library is a low level interface to the solving algorithm, though it
tries to be as convenient as possible. As a result it does not have any
intrinsic knowledge of common user interface conventions like rectangular
regions or even two dimensions. These abstractions belong in a higher level
crate.

## License

Licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT)

at your option.
