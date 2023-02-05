# ASCII-ANSI Table

ASCII (American Standard Code for Information Interchange) is a 7-bit character set that contains 128 (0-127) characters.

The generic term ANSI (American National Standards Institute) is used for 8-bit character sets. They contain further characters from 128 to 255, which differ in the various ANSI character sets. There are character sets for western special characters, and for Arabic, Greek or Cyrillic characters.

The following table shows which characters are available in which (western) character set:

| Character code | Type                 | ASCII | Windows-1252 | ISO-8859-1 |
|:--------------:| -------------------- |:-----:|:------------:|:----------:|
|     0 - 31     | control characters   |  ✅   |      ✅      |     ✅     |
|    32 - 126    | printable characters |  ✅   |      ✅      |     ✅     |
|      127       | control character    |  ✅   |      ✅      |     ✅     |
|   128 - 159    | printable characters |  ❌   |      ✅      |     ❌     |
|   160 - 255    | printable characters |  ❌   |      ✅      |     ✅     |

## ASCII (0-31 & 127)

These characters are part of ASCII, Windows-1252 and ISO-8859-1. Control characters are not intended to be displayed.

The escape sequence (in column "ESC") is used e.g. in programming languages or search functions to be able to enter control characters as text.

| Name                      | Dec | Hex |  Binary  | Caret | ESC  |
| ------------------------- |:---:|:---:|:--------:|:-----:|:----:|
| Null                      |  0  | 00  | 00000000 |  ^@   | `\0` |
| Start of heading          |  1  | 01  | 00000001 |  \^A   |      |
| Start of text             |  2  | 02  | 00000010 |  \^B   |      |
| End of text               |  3  | 03  | 00000011 |  \^C   |      |
| End of transmission       |  4  | 04  | 00000100 |  \^D   |      |
| Enquiry                   |  5  | 05  | 00000101 |  \^E   |      |
| Acknowledge               |  6  | 06  | 00000110 |  \^F   |      |
| Bell                      |  7  | 07  | 00000111 |  \^G   | `\a` |
| Backspace                 |  8  | 08  | 00001000 |  \^H   | `\b` |
| Horizontal tab            |  9  | 09  | 00001001 |  \^I   | `\t` |
| Line feed                 | 10  | 0A  | 00001010 |  \^J   | `\n` |
| Vertical tab              | 11  | 0B  | 00001011 |  \^K   | `\v` |
| Form feed                 | 12  | 0C  | 00001100 |  \^L   | `\f` |
| Carriage return           | 13  | 0D  | 00001101 |  \^M   | `\r` |
| Shift out                 | 14  | 0E  | 00001110 |  \^N   |      |
| Shift in                  | 15  | 0F  | 00001111 |  \^O   |      |
| Data link escape          | 16  | 10  | 00010000 |  \^P   |      |
| Device control 1 (XON)    | 17  | 11  | 00010001 |  \^Q   |      |
| Device control 2          | 18  | 12  | 00010010 |  \^R   |      |
| Device control 3 (XOFF)   | 19  | 13  | 00010011 |  \^S   |      |
| Device control 4          | 20  | 14  | 00010100 |  \^T   |      |
| Negative acknowledge      | 21  | 15  | 00010101 |  \^U   |      |
| Synchronous idle          | 22  | 16  | 00010110 |  \^V   |      |
| End of transmission block | 23  | 17  | 00010111 |  \^W   |      |
| Cancel                    | 24  | 18  | 00011000 |  \^X   |      |
| End of medium             | 25  | 19  | 00011001 |  \^Y   |      |
| Substitute                | 26  | 1A  | 00011010 |  \^Z   |      |
| Escape                    | 27  | 1B  | 00011011 |  ^\[  | `\e` |
| File separator            | 28  | 1C  | 00011100 |  ^/   |      |
| Group separator           | 29  | 1D  | 00011101 |  ^]   |      |
| Record separator          | 30  | 1E  | 00011110 |  ^^   |      |
| Unit separator            | 31  | 1F  | 00011111 |  ^_   |      |
| Delete                    | 127 | 7F  | 00111111 |  ^?   |      |

## ASCII (32 - 126)

| Name                 | Dec | Hex |  Binary  |     |   Entity   |
| -------------------- |:---:|:---:|:--------:|:---:|:----------:|
| Space                | 32  | 20  | 00100000 |     |            |
| Exclamation mark     | 33  | 21  | 00100001 |  !  |  `&excl;`  |
| Quotation mark       | 34  | 22  | 00100010 |  "  |  `&quot;`  |
| Number sign          | 35  | 23  | 00100011 |  #  |  `&num;`   |
| Dollar sign          | 36  | 24  | 00100100 |  $  | `&dollar;` |
| Percent sign         | 37  | 25  | 00100101 |  %  | `&percnt;` |
| Ampersand            | 38  | 26  | 00100110 |  &  |  `&amp;`   |
| Apostrophe           | 39  | 27  | 00100111 |  '  |  `&apos;`  |
| Left parenthesis     | 40  | 28  | 00101000 |  (  |  `&lpar;`  |
| Right parentheses    | 41  | 29  | 00101001 |  )  |  `&rpar;`  |
| Asterisk             | 42  | 2A  | 00101010 |  *  |  `&ast;`   |
| Plus sign            | 43  | 2B  | 00101011 |  +  |  `&plus;`  |
| Comma                | 44  | 2C  | 00101100 |  ,  | `&comma;`  |
| Hyphen               | 45  | 2D  | 00101101 |  -  |            |
| Period               | 46  | 2E  | 00101110 |  .  | `&period;` |
| Slash                | 47  | 2F  | 00101111 |  /  |  `&sol;`   |
| Digit 0              | 48  | 30  | 00110000 |  0  |            |
| Digit 1              | 49  | 31  | 00110001 |  1  |            |
| Digit 2              | 50  | 32  | 00110010 |  2  |            |
| Digit 3              | 51  | 33  | 00110011 |  3  |            |
| Digit 4              | 52  | 34  | 00110100 |  4  |            |
| Digit 5              | 53  | 35  | 00110101 |  5  |            |
| Digit 6              | 54  | 36  | 00110110 |  6  |            |
| Digit 7              | 55  | 37  | 00110111 |  7  |            |
| Digit 8              | 56  | 38  | 00111000 |  8  |            |
| Digit 9              | 57  | 39  | 00111001 |  9  |            |
| Colon                | 58  | 3A  | 00111010 |  :  | `&colon,`  |
| Semicolon            | 59  | 3B  | 00111011 |  ;  |  `&semi;`  |
| Less-than            | 60  | 3C  | 00111100 |  <  |   `&lt;`   |
| Equals sign          | 61  | 3D  | 00111101 |  =  | `&quals;`  |
| Greater-than         | 62  | 3E  | 00111110 |  >  |   `&gt;`   |
| Question mark        | 63  | 3F  | 00111111 |  ?  | `&quest;`  |
| At sign              | 64  | 40  | 01000000 |  @  | `&commat;` |
| Uppercase letter A   | 65  | 41  | 01000001 |  A  |            |
| Uppercase letter B   | 66  | 42  | 01000010 |  B  |            |
| Uppercase letter C   | 67  | 43  | 01000011 |  C  |            |
| Uppercase letter D   | 68  | 44  | 01000100 |  D  |            |
| Uppercase letter E   | 69  | 45  | 01000101 |  E  |            |
| Uppercase letter F   | 70  | 46  | 01000110 |  F  |            |
| Uppercase letter G   | 71  | 47  | 01000111 |  G  |            |
| Uppercase letter H   | 72  | 48  | 01001000 |  H  |            |
| Uppercase letter I   | 73  | 49  | 01001001 |  I  |            |
| Uppercase letter J   | 74  | 4A  | 01001010 |  J  |            |
| Uppercase letter K   | 75  | 4B  | 01001011 |  K  |            |
| Uppercase letter L   | 76  | 4C  | 01001100 |  L  |            |
| Uppercase letter M   | 77  | 4D  | 01001101 |  M  |            |
| Uppercase letter N   | 78  | 4E  | 01001110 |  N  |            |
| Uppercase letter O   | 79  | 4F  | 01001111 |  O  |            |
| Uppercase letter P   | 80  | 50  | 01010000 |  P  |            |
| Uppercase letter Q   | 81  | 51  | 01010001 |  Q  |            |
| Uppercase letter R   | 82  | 52  | 01010010 |  R  |            |
| Uppercase letter S   | 83  | 53  | 01010011 |  S  |            |
| Uppercase letter T   | 84  | 54  | 01010100 |  T  |            |
| Uppercase letter U   | 85  | 55  | 01010101 |  U  |            |
| Uppercase letter V   | 86  | 56  | 01010110 |  V  |            |
| Uppercase letter W   | 87  | 57  | 01010111 |  W  |            |
| Uppercase letter X   | 88  | 58  | 01011000 |  X  |            |
| Uppercase letter Y   | 89  | 59  | 01011001 |  Y  |            |
| Uppercase letter Z   | 90  | 5A  | 01011010 |  Z  |            |
| Left square bracket  | 91  | 5B  | 01011011 | \[  | `&lbrack;` |
| Backslash            | 92  | 5C  | 01011100 |  \  |  `&bsol;`  |
| Right square bracket | 93  | 5D  | 01011101 |  ]  |  `&rsqb;`  |
| Caret                | 94  | 5E  | 01011110 |  ^  |  `&Hat;`   |
| Underscore           | 95  | 5F  | 01011111 |  _  | `&lowbar;` |
| Grave accent         | 96  | 60  | 01100000 | \`  | `&grave;`  |
| Lowercase letter a   | 97  | 61  | 01100001 |  a  |            |
| Lowercase letter b   | 98  | 62  | 01100010 |  b  |            |
| Lowercase letter c   | 99  | 63  | 01100011 |  c  |            |
| Lowercase letter d   | 100 | 64  | 01100100 |  d  |            |
| Lowercase letter e   | 101 | 65  | 01100101 |  e  |            |
| Lowercase letter f   | 102 | 66  | 01100110 |  f  |            |
| Lowercase letter g   | 103 | 67  | 01100111 |  g  |            |
| Lowercase letter h   | 104 | 68  | 01101000 |  h  |            |
| Lowercase letter i   | 105 | 69  | 01101001 |  i  |            |
| Lowercase letter j   | 106 | 6A  | 01101010 |  j  |            |
| Lowercase letter k   | 107 | 6B  | 01101011 |  k  |            |
| Lowercase letter l   | 108 | 6C  | 01101100 |  l  |            |
| Lowercase letter m   | 109 | 6D  | 01101101 |  m  |            |
| Lowercase letter n   | 110 | 6E  | 01101110 |  N  |            |
| Lowercase letter o   | 111 | 6F  | 01101111 |  o  |            |
| Lowercase letter p   | 112 | 70  | 01110000 |  p  |            |
| Lowercase letter q   | 113 | 71  | 01110001 |  q  |            |
| Lowercase letter r   | 114 | 72  | 01110010 |  r  |            |
| Lowercase letter s   | 115 | 73  | 01110011 |  s  |            |
| Lowercase letter t   | 116 | 74  | 01110100 |  t  |            |
| Lowercase letter u   | 117 | 75  | 01110101 |  u  |            |
| Lowercase letter v   | 118 | 76  | 01110110 |  v  |            |
| Lowercase letter w   | 119 | 77  | 01110111 |  w  |            |
| Lowercase letter x   | 120 | 78  | 01111000 |  x  |            |
| Lowercase letter y   | 121 | 79  | 01111001 |  y  |            |
| Lowercase letter z   | 122 | 7A  | 01111010 |  z  |            |
| Left curly brace     | 123 | 7B  | 01111011 |  {  | `&lbrace;` |
| Vertical bar         | 124 | 7C  | 01111100 | \|  |  `&vert;`  |
| Right curly brace    | 125 | 7D  | 01111101 |  }  |  `&rcub;`  |
| Tilde                | 126 | 7E  | 01111110 |  ~  |            |

## ANSI (128 - 159)

| Name                                       | Dec | Hex |  Binary  |     |   Entity   |
| ------------------------------------------ |:---:|:---:|:--------:|:---:|:----------:|
| Euro sign                                  | 128 | 80  | 10000000 |  €  |  `&euro;`  |
| (not used)                                 | 129 | 81  | 10000001 |     |            |
| Single low-9 quotation mark                | 130 | 82  | 10000010 |  ‚  | `&sbquo;`  |
| Latin small letter f with hook             | 131 | 83  | 10000011 |  ƒ  |  `&fnof;`  |
| Double low-9 quotation mark                | 132 | 84  | 10000100 |  „  | `&bdquo;`  |
| Horizontal ellipsis                        | 133 | 85  | 10000101 |  …  | `&hellip;` |
| Dagger                                     | 134 | 86  | 10000110 |  †  | `&dagger;` |
| Double dagger                              | 135 | 87  | 10000111 |  ‡  | `&Dagger;` |
| Modifier letter circumflex accent          | 136 | 88  | 10001000 |  ˆ  |  `&circ;`  |
| Permille sign                              | 137 | 89  | 10001001 |  ‰  | `&permil;` |
| Latin capital letter S with caron          | 138 | 8A  | 10001010 |  Š  | `&Scaron;` |
| Single left-pointing angle quotation mark  | 139 | 8B  | 10001011 |  ‹  | `&lsaquo;` |
| Latin capital ligature OE                  | 140 | 8C  | 10001100 |  Œ  | `&OElig;`  |
| (Not used)                                 | 141 | 8D  | 10001101 |     |            |
| Latin capital letter Z with caron          | 142 | 8E  | 10001110 |  Ž  | `&Zcaron;` |
| (Not used)                                 | 143 | 8F  | 10001111 |     |            |
| (Not used)                                 | 144 | 90  | 10010000 |     |            |
| Left single quotation mark                 | 145 | 91  | 10010001 |  ‘  | `&lsquo;`  |
| Right single quotation mark                | 146 | 92  | 10010010 |  ’  | `&rsquo;`  |
| Left double quotation mark                 | 147 | 93  | 10010011 |  “  | `&ldquo;`  |
| Right double quotation mark                | 148 | 94  | 10010100 |  ”  | `&rdquo;`  |
| Bullet                                     | 149 | 95  | 10010101 |  •  |  `&bull;`  |
| En dash                                    | 150 | 96  | 10010110 |  –  | `&ndash;`  |
| Em dash                                    | 151 | 97  | 10010111 |  —  | `&mdash;`  |
| Small tilde                                | 152 | 98  | 10011000 |  ˜  | `&tilde;`  |
| Trade mark sign                            | 153 | 99  | 10011001 |  ™  | `&trade;`  |
| Latin small letter s with caron            | 154 | 9A  | 10011010 |  š  | `&scaron;` |
| Single right-pointing angle quotation mark | 155 | 9B  | 10011011 |  ›  | `&rsaquo;` |
| Latin small ligature oe                    | 156 | 9C  | 10011100 |  œ  | `&oelig;`  |
| (Not used)                                 | 157 | 9D  | 10011101 |     |            |
| Latin small letter z with caron            | 158 | 9E  | 10011110 |  ž  | `&zcaron;` |
| Latin capital letter Y with diaresis       | 159 | 9F  | 10011111 |  Ÿ  |  `&Yuml;`  |

## ANSI (160-255)

| Name                                       | Dec | Hex |  Binary  |     |        Entity        |
| ------------------------------------------ |:---:|:---:|:--------:|:---:|:--------------------:|
| No-break space                             | 160 | A0  | 10100000 |     |       `&nbsp;`       |
| Inverted exclamation mark                  | 161 | A1  | 10100001 |  ¡  |      `&iexcl;`       |
| Cent sign                                  | 162 | A2  | 10100010 |  ¢  |       `&cent;`       |
| Pound sign                                 | 163 | A3  | 10100011 |  £  |      `&pound;`       |
| Currency sign                              | 164 | A4  | 10100100 |  ¤  |      `&curren;`      |
| Yen sign                                   | 165 | A5  | 10100101 |  ¥  |       `&yen;`        |
| Broken bar                                 | 166 | A6  | 10100110 |  ¦  |      `&brvbar;`      |
| Section sign                               | 167 | A7  | 10100111 |  §  |       `&sect;`       |
| Diaresis                                   | 168 | A8  | 10101000 |  ¨  |    `&DoubleDot;`     |
| Copyright sign                             | 169 | A9  | 10101001 |  ©  |       `&copy;`       |
| Feminine ordinal indicator                 | 170 | AA  | 10101010 |  ª  |       `&ordf;`       |
| Left-pointing double angle quotation mark  | 171 | AB  | 10101011 |  «  |      `&laquo;`       |
| Not sign                                   | 172 | AC  | 10101100 |  ¬  |       `&not;`        |
| Soft hyphen                                | 173 | AD  | 10101101 |     |       `&shy;`        |
| Registered sign                            | 174 | AE  | 10101110 |  ®  |       `&reg;`        |
| Macron                                     | 175 | AF  | 10101111 |  ¯  |       `&macr;`       |
| Degree sign                                | 176 | B0  | 10110000 |  °  |       `&deg;`        |
| Plus-minus sign                            | 177 | B1  | 10110001 |  ±  |      `&plusmn;`      |
| Superscript two                            | 178 | B2  | 10110010 |  ²  |       `&sup2;`       |
| Superscript three                          | 179 | B3  | 10110011 |  ³  |       `&sup3;`       |
| Acute accent                               | 180 | B4  | 10110100 |  ´  | `&DiacriticalAcute;` |
| Micro sign                                 | 181 | B5  | 10110101 |  µ  |      `&micro;`       |
| Pilcrow sign                               | 182 | B6  | 10110110 |  ¶  |       `&para;`       |
| Middle dot                                 | 183 | B7  | 10110111 |  ·  |    `&CenterDot;`     |
| Cedilla                                    | 184 | B8  | 10111000 |  ¸  |     `&Cedilla;`      |
| Superscript one                            | 185 | B9  | 10111001 |  ¹  |       `&sup1;`       |
| Masculine ordinal indicator                | 186 | BA  | 10111010 |  º  |       `&ordm;`       |
| Right-pointing double angle quotation mark | 187 | BB  | 10111011 |  »  |      `&raquo;`       |
| Vulgar fraction one quarter                | 188 | BC  | 10111100 |  ¼  |      `&frac14;`      |
| Vulgar fraction one half                   | 189 | BD  | 10111101 |  ½  |       `&half;`       |
| Vulgar fraction three quarters             | 190 | BE  | 10111110 |  ¾  |      `&frac34;`      |
| Inverted question mark                     | 191 | BF  | 10111111 |  ¿  |      `&iquest;`      |
| Latin capital letter A with grave          | 192 | C0  | 11000000 |  À  |      `&Agrave;`      |
| Latin capital letter A with acute          | 193 | C1  | 11000001 |  Á  |      `&Aacute;`      |
| Latin capital letter A with circumflex     | 194 | C2  | 11000010 |  Â  |      `&Acirc;`       |
| Latin capital letter A with tilde          | 195 | C3  | 11000011 |  Ã  |      `&Atilde;`      |
| Latin capital letter A with diaresis       | 196 | C4  | 11000100 |  Ä  |       `&Auml;`       |
| Latin capital letter A with ring above     | 197 | C5  | 11000101 |  Å  |      `&Aring;`       |
| Latin capital letter AE                    | 198 | C6  | 11000110 |  Æ  |      `&AElig;`       |
| Latin capital letter C with cedilla        | 199 | C7  | 11000111 |  Ç  |      `&Ccedil;`      |
| Latin capital letter E with grave          | 200 | C8  | 11001000 |  È  |      `&Egrave;`      |
| Latin capital letter E with acute          | 201 | C9  | 11001001 |  É  |      `&Eacute;`      |
| Latin capital letter E with circumflex     | 202 | CA  | 11001010 |  Ê  |      `&Ecirc;`       |
| Latin capital letter E with diaresis       | 203 | CB  | 11001011 |  Ë  |       `&Euml;`       |
| Latin capital letter I with grave          | 204 | CC  | 11001100 |  Ì  |      `&Igrave;`      |
| Latin capital letter I with acute          | 205 | CD  | 11001101 |  Í  |      `&Iacute;`      |
| Latin capital letter I with circumflex     | 206 | CE  | 11001110 |  Î  |      `&Icirc;`       |
| Latin capital letter I with diaresis       | 207 | CF  | 11001111 |  Ï  |       `&Iuml;`       |
| Latin capital letter Eth                   | 208 | D0  | 11010000 |  Ð  |       `&ETH;`        |
| Latin capital letter N with tilde          | 209 | D1  | 11010001 |  Ñ  |      `&Ntilde;`      |
| Latin capital letter O with grave          | 210 | D2  | 11010010 |  Ò  |      `&Ograve;`      |
| Latin capital letter O with acute          | 211 | D3  | 11010011 |  Ó  |      `&Oacute;`      |
| Latin capital letter O with circumflex     | 212 | D4  | 11010100 |  Ô  |      `&Ocirc;`       |
| Latin capital letter O with tilde          | 213 | D5  | 11010101 |  Õ  |      `&Otilde;`      |
| Latin capital letter O with diaresis       | 214 | D6  | 11010110 |  Ö  |       `&Ouml;`       |
| Multiplication sign                        | 215 | D7  | 11010111 |  ×  |      `&times;`       |
| Latin capital letter O with stroke         | 216 | D8  | 11011000 |  Ø  |      `&Oslash;`      |
| Latin capital letter U with grave          | 217 | D9  | 11011001 |  Ù  |      `&Ugrave;`      |
| Latin capital letter U with acute          | 218 | DA  | 11011010 |  Ú  |      `&Uacute;`      |
| Latin capital letter U with circumflex     | 219 | DB  | 11011011 |  Û  |      `&Ucirc;`       |
| Latin capital letter U with diaresis       | 220 | DC  | 11011100 |  Ü  |       `&Uuml;`       |
| Latin capital letter Y with acute          | 221 | DD  | 11011101 |  Ý  |      `&Yacute;`      |
| Latin capital letter Thorn                 | 222 | DE  | 11011110 |  Þ  |      `&THORN;`       |
| Latin small letter sharp s                 | 223 | DF  | 11011111 |  ß  |      `&szlig;`       |
| Latin small letter a with grave            | 224 | E0  | 11100000 |  à  |      `&agrave;`      |
| Latin small letter a with acute            | 225 | E1  | 11100001 |  á  |      `&aacute;`      |
| Latin small letter a with circumflex       | 226 | E2  | 11100010 |  â  |      `&acirc;`       |
| Latin small letter a with tilde            | 227 | E3  | 11100011 |  ã  |      `&atilde;`      |
| Latin small letter a with diaresis         | 228 | E4  | 11100100 |  ä  |       `&auml;`       |
| Latin small letter a with ring above       | 229 | E5  | 11100101 |  å  |      `&aring;`       |
| Latin small letter ae                      | 230 | E6  | 11100110 |  æ  |      `&aelig;`       |
| Latin small letter c with cedilla          | 231 | E7  | 11100111 |  ç  |      `&ccedil;`      |
| Latin small letter e with grave            | 232 | E8  | 11101000 |  è  |      `&egrave;`      |
| Latin small letter e with acute            | 233 | E9  | 11101001 |  é  |      `&eacute;`      |
| Latin small letter e with circumflex       | 234 | EA  | 11101010 |  ê  |      `&ecirc;`       |
| Latin small letter e with diaresis         | 235 | EB  | 11101011 |  ë  |       `&euml;`       |
| Latin small letter i with grave            | 236 | EC  | 11101100 |  ì  |      `&igrave;`      |
| Latin small letter i with acute            | 237 | ED  | 11101101 |  í  |      `&iacute;`      |
| Latin small letter i with circumflex       | 238 | EE  | 11101110 |  î  |      `&icirc;`       |
| Latin small letter i with diaresis         | 239 | EF  | 11101111 |  ï  |       `&iuml;`       |
| Latin small letter eth                     | 240 | F0  | 11110000 |  ð  |       `&eth;`        |
| Latin small letter n with tilde            | 241 | F1  | 11110001 |  ñ  |      `&ntilde;`      |
| Latin small letter o with grave            | 242 | F2  | 11110010 |  ò  |      `&ograve;`      |
| Latin small letter o with acute            | 243 | F3  | 11110011 |  ó  |      `&oacute;`      |
| Latin small letter o with circumflex       | 244 | F4  | 11110100 |  ô  |      `&ocirc;`       |
| Latin small letter o with tilde            | 245 | F5  | 11110101 |  õ  |      `&otilde;`      |
| Latin small letter o with diaresis         | 246 | F6  | 11110110 |  ö  |       `&ouml;`       |
| Division sign                              | 247 | F7  | 11110111 |  ÷  |      `&divide;`      |
| Latin small letter o with stroke           | 248 | F8  | 11111000 |  ø  |      `&oslash;`      |
| Latin small letter u with grave            | 249 | F9  | 11111001 |  ù  |      `&ugrave;`      |
| Latin small letter u with acute            | 250 | FA  | 11111010 |  ú  |      `&uacute;`      |
| Latin small letter u with circumflex       | 251 | FB  | 11111011 |  û  |      `&ucirc;`       |
| Latin small letter u with diaresis         | 252 | FC  | 11111100 |  ü  |       `&uuml;`       |
| Latin small letter y with acute            | 253 | FD  | 11111101 |  ý  |      `&yacute;`      |
| Latin small letter thorn                   | 254 | FE  | 11111110 |  þ  |      `&thorn;`       |
| Latin small letter y with diaresis         | 255 | FF  | 11111111 |  ÿ  |       `&yuml;`       |

---

#ANSI #ASCII

## Resources

- [ASCII-ANSI Table](https://www.gaijin.at/en/infos/ascii-ansi-character-table)