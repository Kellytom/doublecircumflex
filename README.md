# Double circumflex

## Proposing to reserve special characters "^^". Use them to replace tabs in outlines.  

#### From outline to plaintext and back.

...Or how to change from tabs to something human readable. Tabs are not really human readable because they can be confused with spaces.

Why is this even necessary? Because when Markdown and Multimarkdown editors open outlines, they usually leave tabs in, making the text move too far to the right. Any sub points become unreadable, especially on a thin smartphone (e.g. iPhone)

Plain text outlines can be imported and exported from many outlining apps, but they don't play well with markdown editors.

I propose using `^^` or `..`  or`_`as a marker for the tab character in markdown or multimarkdown documents.

One can convert from an outline to a plain text (or markdown) document for readability. On the other hand, one can convert from a markdown document to an outline by changing the double circumflex `^^` to tab characters. The tab character is not available on the iPhone keyboard. Making a file in an outline format often requires the tab character.

I want to use outline formats with multimarkdown because I want to fold the document to see the structure, and rearrange the paragraphs. Currently I use Taskpaper on the iphone to rearrange markdown documents. Using the outline format gives me more flexibility when changing and editing plain text documents.

#### The choice of double circumflex as tab replacement characters.

What character(s) should one use? In order to solve these problems mentioned above, one needs to convert the tabs to special characters, and back again.

If I convert tabs to 4 spaces then it turns into a code block in markdown. If I convert to three spaces or two spaces then two tabs in a row turn into a code block. A better solution is to convert tabs to a special character combination.


#### First of all, investigate the "one character" option:  

These are the special characters available on a regular keyboard.  

ALL special characters:

> backtick \`, ~, !, @, #, %, ^, &, *, -, _, +, =, |, \, {}, [], <>, /

RESERVED markdown characters:

> backtick \`, !, #, *, |, [], > (= blockquote)

> \\ backslash escapes a special character.

RESERVED punctuation, HTML and web characters:

> !, @, /, $, %, &, -, +, =, <>, :, ;, quotes

> {} are used in critic markup  
> ~ is used in latex  
> ^ Circumflex is used in math formulae.

That leave these possible single characters:  
`^, ~, _` These are OK for my personal use, but will break if someone uses latex or math equations. (I use the `~` symbol personally sometimes when writing about tao, tai chi and human philosophy in general.)

#### The next option is two or more characters:  

The best options to investigate seem to be:
> ~~ or  
^^  or
__


(All possible combinations are not completely investigated here. I start with double characters because they are easier to type and recognize in a body of text.)

RESERVED double characters:  
> `<!--` = html or latex raw code begin  
> `-->` = html end  
> `==` = a markdown title


Other possibilites not used:    

critic markup already uses:

> Substitution {~~ ~> ~~}  

> Addition {++ ++}  

That leaves ^^ or __ for outline.

#### The double circumflex or double underscore seems to be the best option left for a two character marker for tab.

Example Outline:  

^^ point one  
^^ point two  
^^^^ sub point a  
^^^^ sub point b  

or
.. point one  
.. point two  
.... sub point a  
.... sub point b  

So replace ^^ or __with tab to convert to outline format, and  
replace tab with ^^ or __ to convert to Markdown.

Of course, this does not need to be in the markdown or Multimarkdown OR Critic spec because they don't need a parser to change back and forth. No parsing is necessary, only search and replace with any text editor.

There are many formats for outlines including OPML, etc. but most robust programs will import tabbed outlines.


PS. To keep versions straight, "OL" can be added to the end of the filename for outlines, for example:

test OL.txt  (contains tabs)  
test MD.txt (contains ^^) or  
test MMD.txt (contains ^^)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4NjgyMjczMjRdfQ==
-->