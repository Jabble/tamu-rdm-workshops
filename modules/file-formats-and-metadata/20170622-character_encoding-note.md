## ASCII
Encoding using 7 bits in an 8-bit byte to encode characters, these 7 bits are able to represent characters using a numbers between 32 and 127. "Characters" here refer to unaccented English letters and punctuation. Numbers below 32 are control characters.

## ANSI
Since ASCII only took advantage of 7 out of 8 bits in a byte, more could be done with the last bit, accounting for numbers 128 to 255. In fact, "lots of people got to thinking, 'gosh, we can use the codes 128-255 for our own purposes.'" These were called the OEM character sets and many of them were devleoped. "This OEM free-for-all got codified in the ANSI standard." Below 128 all are pretty much the same as ASCII, but different ways to handle the characters from 128 and on up are documented in *code pages*.

## Unicode 
Added a layer of abstraction in an "effort to create a single character set that included every reasonable writing system on the planet." In Unicode, a character maps to a *code point*, e.g. English letter 'A' is U+0041. This code point is then encoded into some number of bytes. In UTF-8 encoding, every code point from 0-127 is stored in a single byte. Only code points 128 and above are stored using 2, 3, or up to 6 bytes. Due to this, in UTF-8 0–127 are the same as ASCII and ANSI. Unicode can also be used in character encodings UTF 7, UTF 8, UTF 16, UTF 32 each character will then be represented either as a sequence of one to four 8-bit bytes (UTF 8), one or two 16-bit code units (UTF 16), or a single 32-bit code unit (UTF 32). 

Traditional store-it-in-two-byte methods of encoding Unicode are called UCS-2 (because it has two bytes) or UTF-16 (because it has 16 bits).  Visual Basic, COM, and Windows NT/2000/XP use UCS-2 (two byte) Unicode as their native string type. However, with two byte encoding you can store characters in two different ways, high-endian UCS-2 mode or low-endian UCS-2 mode. Due to the ability to store code points in high-endian or low-endian mode, a Unicode Byte Order Mark is needed to indicate the mode. FE FF is added at the beginning of every Unicode string to indicate high-endian or low-endian mode.

<table>
	<tr>
		 <th>Name</th>
		 <th>UTF-8</th>
		 <th>UTF-16</th>
		 <th>UTF-16BE</th>
		 <th>UTF-16LE</th>
		 <th>UTF-32</th>
		 <th>UTF-32BE</th>
		 <th>UTF-32LE</th>
	   </tr>
	<tr>
		 <th>Smallest code point</th>
		 <td align="right">0000</td>
		 <td align="right">0000</td>
		 <td align="right">0000</td>
		 <td align="right">0000</td>
		 <td align="right">0000</td>
		 <td align="right">0000</td>
		 <td align="right">0000</td>
	   </tr>
	<tr>
		 <th>Largest code point</th>
		 <td align="right">10FFFF</td>
		 <td align="right">10FFFF</td>
		 <td align="right">10FFFF</td>
		 <td align="right">10FFFF</td>
		 <td align="right">10FFFF</td>
		 <td align="right">10FFFF</td>
		 <td align="right">10FFFF</td>
	   </tr>
	<tr>
		 <th>Code unit size</th>
		 <td align="center">8 bits</td>
		 <td align="center">16 bits</td>
		 <td align="center">16 bits</td>
		 <td align="center">16 bits</td>
		 <td align="center">32 bits</td>
		 <td align="center">32 bits</td>
		 <td align="center">32 bits</td>
	   </tr>
	<tr>
		 <th>Byte order</th>
		 <td align="center">N/A</td>
		 <td align="center">&lt;BOM&gt;</td>
		 <td align="center">big-endian</td>
		 <td align="center">little-endian</td>
		 <td align="center">&lt;BOM&gt;</td>
		 <td align="center">big-endian</td>
		 <td align="center">little-endian</td>
	   </tr>
	<tr>
		 <th>Fewest bytes per character</th>
		 <td align="center">1</td>
		 <td align="center">2</td>
		 <td align="center">2</td>
		 <td align="center">2</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
	   </tr>
	<tr>
		 <th>Most bytes per character</th>
		 <td align="center">4</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
		 <td align="center">4</td>
	 </tr>
</table>

In the table <BOM> indicates that the byte order is determined by a byte order mark, if present at the beginning of the data stream, otherwise it is big-endian.

UTF-16 and UTF-32 use code units that are two and four bytes long respectively. For these UTFs, there are three sub-flavors: BE, LE and unmarked. The BE form uses big-endian byte serialization (most significant byte first), the LE form uses little-endian byte serialization (least significant byte first) and the unmarked form uses big-endian byte serialization by default, but may include a byte order mark at the beginning to indicate the actual byte serialization used.

## Others
Some popular encodings of English text are Windows-1252 (the Windows 9x standard for Western European languages) and ISO-8859-1, aka Latin-1 (also useful for any Western European language). But try to store Russian or Hebrew letters in these encodings and you get a bunch of question marks.

## References
- Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)
- Unicode. "UTF-8, UTF-16, UTF-32 & BOM" [website](http://unicode.org/faq/utf_bom.html)