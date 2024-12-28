# Identifiers
* Bare identifiers can now be used as values in Arguments and Properties, and are interpreted as string values.

# Whitespace
* More places allow whitespace (node-spaces, specifically) now
  * Around `=` for props (`x = 1`)

* Slashdash (`/-`) -compatible locations adjusted to be more clear and intuitive. They can now be used in exactly three different places: before nodes, before entire entries, or before entire child blocks.
  * ordering of slashdashed elements has been restricted: slashdashed child block cannot go before an entry (including slashdashed entries)
