# Text
##### When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.
* Structural markup: the elements that you can use to describe both headings and paragraphs

* Semantic markup: which provides extra information such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on



### paragraphs
##### \<p> To create a paragraph, surround the words that make up the paragraph with an opening <p> tag and closing \</p> tag. By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.


#### bold & italic
##### \<b> By enclosing words in the tags \<b> and \</b> we can make characters appear bold. The \<b> element also represents a section of text that would be presented in a visually different way (for example key words in a paragraph) although the use of the <b> element does not imply any additional meaning.

##### \<i> By enclosing words in the tags\<i> and \</i> we can make characters appear italic. The \<i> element also represents a section of text that would be said in a different way from surrounding content — such as technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized.
### Superscript & Subscrip
##### \<sup>
##### The \<sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22 .
##### \<sub>
##### The \<sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H2 0.

### Line Breaks & Horizontal Rules
#### \<br />
##### As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag \<br />.
#### \<hr />
##### To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the \<hr /> tag.
<hr/>

# Introducing CSS
##### CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.
![typesofCSS](https://www.bitdegree.org/learn/storage/media/images/8c4493d3-110c-4a95-8b70-7626ce2d2f4e.jpg)

### external CSS
##### \<link>
##### The \<link> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the \<head> element. It should use three attributes:
##### href <br/> This specifies the path to the CSS file (which is often placed in a folder called css or styles). 
##### type <br/> This attribute specifies the type of document being linked to. The value should be text/css. rel This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.
![externalCSS](https://codebridgeplus.com/wp-content/uploads/download-5.png)

### Internal CSS
##### \<style> <br/> You can also include CSS rules within an HTML page by placing them inside a \<style> element, which usually sits inside the \<head> element of the page.The \<style> element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/ css. When building a site with more than one page, you should use an external CSS style sheet. This:
* Allows all pages to use the same style rules (rather than repeating them in each page).
* Keeps the content separate from how the page looks.
* Means you can change the styles used across all pages by altering just one file (rather than each individual page).

![internal CSS](https://i.stack.imgur.com/K59EF.gif)
<hr/>

# Basic Java script instructions
### statements
##### A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon. 
##### We will look at what the code on the right does shortly, but for the moment note that:

### COMMENTS
##### You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code. 


### WHAT IS A VARIABLE?
##### A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.<br/> When you write JavaScript, you have to tell the interpreter every individual step that you want it to perform. This sometimes involves more detail than you might expect. <br/> Think about calculating the area of a wall; in math the area of a rectangle is obtained by multiplying two numbers: 

### USING COMPARISON OPERATORS
##### at the most basic level, you can evaluate two variables using a comparison operator to return a true or false value.
##### In this example, a user is taking a test, and the script tells the user whether they have passed this round of the test.
##### The example starts by setting two variables:
1. pass to hold the pass mark
2. score to hold the users score
##### To see if the user has passed, a comparison operator checks whether scor e is greater than or equal to pass. The result will be true or false, and is stored in a variable called has Passed. On the next line, the result is written to the screen 