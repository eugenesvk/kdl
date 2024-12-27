# Identifiers
* Bare identifiers can now be used as values in Arguments and Properties, and are interpreted as string values.

# Whitespace
* `node-space` is now allowed as whitespace after a `slashdash`, meaning line continuations will work now.
* More places allow whitespace (node-spaces, specifically) now
  * Inside `(foo)` annotations `( foo )` would be legal `( f oo )` would not be, since it has two identifiers
  * Between annotations and the thing they're annotating `(blah) node (thing) 1 y= (who) 2`
  * Around `=` for props (`x = 1`)

* Slashdash (`/-`) -compatible locations adjusted to be more clear and intuitive. They can now be used in exactly three different places: before nodes, before entire entries, or before entire child blocks.
  * ordering of slashdashed elements has been restricted: slashdashed child block cannot go before an entry (including slashdashed entries)
