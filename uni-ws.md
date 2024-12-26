.         0009..000D    ; White_Space # Cc   [5] <control-0009>..<control-000D>
# . ␠  ␤
.   +     0009          ; White_Space # Cc       <control-0009>
.      +  000A          ; White_Space # Cc       <control-001A>
.      +  000B          ; White_Space # Cc       <control-000B>
.      +  000C          ; White_Space # Cc       <control-000C>
.      +  000D          ; White_Space # Cc       <control-000D>
.   +     0020          ; White_Space # Zs       SPACE
.      +  0085          ; White_Space # Cc       <control-0085>
.   +     00A0          ; White_Space # Zs       NO-BREAK SPACE
.   +     1680          ; White_Space # Zs       OGHAM SPACE MARK
.   +     2000..200A    ; White_Space # Zs  [11] EN QUAD..HAIR SPACE
.      +  2028          ; White_Space # Zl       LINE SEPARATOR
.      +  2029          ; White_Space # Zp       PARAGRAPH SEPARATOR
.   +     202F          ; White_Space # Zs       NARROW NO-BREAK SPACE
.   +     205F          ; White_Space # Zs       MEDIUM MATHEMATICAL SPACE
.   +     3000          ; White_Space # Zs       IDEOGRAPHIC SPACE
25 18  7  25 ∑

∑ 7  7
| + | LF      | Line Feed       | `U+000A`  |
| + | CR      | Carriage Return | `U+000D`  |
| + | NEL     | Next Line       | `U+0085`  |
| + | VT      | Vertical tab    | `U+000B`  |
| + | FF      | Form Feed       | `U+000C`  |
| + | LS      | Line Separator  | `U+2028`  |
| + | PS      | Paragraph Separator | `U+2029` |

∑ 18  18
| + | Character Tabulation | `U+0009`  |
| + | Space                | `U+0020`  |
| + | No-Break Space       | `U+00A0`  |
| + | Ogham Space Mark     | `U+1680`  |
| + | En Quad              | `U+2000`  |
| + | Em Quad              | `U+2001`  |
| + | En Space             | `U+2002`  |
| + | Em Space             | `U+2003`  |
| + | Three-Per-Em Space   | `U+2004`  |
| + | Four-Per-Em Space    | `U+2005`  |
| + | Six-Per-Em Space     | `U+2006`  |
| + | Figure Space         | `U+2007`  |
| + | Punctuation Space    | `U+2008`  |
| + | Thin Space           | `U+2009`  |
| + | Hair Space           | `U+200A`  |
| + | Narrow No-Break Space| `U+202F`  |
| + | Medium Mathematical Space | `U+205F`  |
| + | Ideographic Space    | `U+3000`  |


(repeats White_Space)
0009..000D    ; Pattern_White_Space # Cc   [5] <control-0009>..<control-000D>
0020          ; Pattern_White_Space # Zs       SPACE
0085          ; Pattern_White_Space # Cc       <control-0085>
200E..200F    ; Pattern_White_Space # Cf   [2] LEFT-TO-RIGHT MARK..RIGHT-TO-LEFT MARK
2028          ; Pattern_White_Space # Zl       LINE SEPARATOR
2029          ; Pattern_White_Space # Zp       PARAGRAPH SEPARATOR
# Total code points: 11
