# KDL Changelog

# String
* All literal whitespace following a `\` in a string is now discarded.

* Multiline string escape rules have been tweaked significantly.
  * Multi-line strings must now use `"""` as delimeters. The opening delimiter must be immediately followed by a newline, and the closing delimiter must be on its own line, prefixed by optional whitespace.
  * Multi-line strings are now automatically dedented, according to the common  whitespace matching the whitespace prefix of the closing line.
  * Multi-line strings' literal Newline sequences are now normalized to single `LF`s.
  * Multiline strings, both Raw and Quoted, must now use `"""` instead of a single `"`. Using `"""` for a single-line string is a syntax error.
  * Grammar has been fixed to disallow raw strings like `#"""#`, which are now properly treated as invalid multi-line raw strings (instead of the equivalent of `"\""`).
  * One or two consecutive double-quotes are now allowed in the bodies of multi-line quoted strings, without needing to be escaped

# Identifiers
* Bare identifiers can now be used as values in Arguments and Properties, and are interpreted as string values.
* `.1`, `+.1` etc are no longer valid identifiers, to prevent confusion and conflicts with numbers.

# Whitespace
* `node-space` is now allowed as whitespace after a `slashdash`, meaning line continuations will work now.
* More places allow whitespace (node-spaces, specifically) now
  * Inside `(foo)` annotations `( foo )` would be legal `( f oo )` would not be, since it has two identifiers
  * Between annotations and the thing they're annotating `(blah) node (thing) 1 y= (who) 2`
  * Around `=` for props (`x = 1`)

* Slashdash (`/-`) -compatible locations adjusted to be more clear andintuitive. They can now be used in exactly three different places: before nodes, before entire entries, or before entire child blocks.
  * ordering of slashdashed elements has been restricted: slashdashed child block cannot go before an entry (including slashdashed entries)
