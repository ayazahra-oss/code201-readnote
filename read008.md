## HTML and CSS
Basics
### 1.  Introduction to HTML/CSS
If you are the content provider, read HTML. If you are the graphic designer, read CSS. If you are a programmer and want to add dynamic effects to your web page, read JavaScript. But if you operate in OMO (one-man-operated) and are expected to create a reasonably good-looking website, you need to understand HTML, CSS and JavaScript. This is the reason that I combine both the HTML and CSS in this article as they are inseparable.

To create an OMO website, I suggest that:

Understand HTML, CSS and JavaScript thoroughly.
Pick an authoring tool. Use Dreamweaver if you can afford. Otherwise, find a free HTML text editor (such as NotePad++, Sublime). For programmers, NetBeans/Eclipse are good choice for HTML/CSS/JavaScript as they perform syntax checking and provide auto-complete.
Design and organize your page. Decide on the look and feel of your website. How many columns? What are the major sections (e.g., header, navigation menu, main content, sidebar, table of content, footer)? Do you need a navigation menu or panel? What is your theme (colors, fonts)? And so on.
Take a close look at your favorite websites!!! CSS is humongous and complex! You can't invent this wheel! Use Firefox plugin "Firebug" (@ getfirebug.com) or the built-in "Web Developer Tools" to inspect HTML/CSS of your favorite websites.
Alternatively, you can use a CSS framework (I recommend BootStrap) to jump-start your design.
Start with an initial CSS design. Website design begins with CSS, NOT HTML?!. Work on your CSS:
Partition your web page into logical section via <div> (or HTML5' <header>, <footer>, <section>, <nav>), such as header, content, footer. Assign an id to <div> that is unique (e.g., "header", "footer". Assign a common classname to sections (non-unique) that share the same style (e.g., "entry", "side-note"). Write the CSS id-selectors and class-selectors (e.g., #header tag-name,... #footer tag-name,... #menu tag-name,...) for common tags (such as h1, h2, h3, p, a:link, a:visited, a:hover, a:active), in each of the <div>'s. Basically, what I am saying is to design each of the sections by itself - a "divide and conquer" strategy.
Create sub-classes for common styles, such as layout out tables and images and special effects (e.g., ".highlight", ".underline", ".center"). They could be used in <div> and <span>.
There are many good and free CSS templates (or web templates) available online (just google "CSS Templates" or "Web templates"). Pick one that meets your taste to model after. You can also look at the CSS of any website that you find interesting. Be aware of the Intellectual Property Right, do not use any images or graphics unless they are in the public domain. It is extremely easy to create one yourself with an imaging tool, such as PhotoShop, Element, Illustrator or even Paint.
Alternatively, use CSS framework such as BootStrap and pick your favorite design from the samples.
Write your HTML pages. You may need to modify the CSS as you go along. The most challenging thing for an OMO web author is that he has to be concerned about both the contents and appearances at the same time, and can lose focus at times!
Repeat the previous steps until you are happy with your page's look and feel, layout, and most importantly, the contents - try not to create yet another insignificant website.
### 2.  Introduction to HTML
What is HTML (HyperText Markup Language)?
HTML is the language for publishing web pages on the WWW (World-Wide Web, or World-Wide Wait?).
HTML is a Document Description Language (aka Document Markup Language). HTML is NOT a programming language like C/C++/C#/Java, which is used to implement programming algorithm.
An HTML document is a text document, and it is human-readable.
HTML Versions - HTML4.01, XHTML1.0 and HTML5
Today, the W3C (World-Wide Web Consortium) (@ http://www.w3c.org) maintains the specifications of HTML and CSS (and many other related web technologies).

HTML has gone through these changes:

HTML Draft (October1991): Tim Bernes-Lee (of CERN) proposed the early HTML for sharing of document in a hypertext system.
HTML 2.0 (November 1995): Published as IETF RFC 1866.
HTML 3.2 (January 1997): Published as W3C Recommendation.
HTML 4.0 (December 1997): Published as W3C Recommendation, with strict, transitional and frameset.
HTML 4.01 (December 1999): Touched up HTML 4.0. The supposedly final HTML specification published by W3C.
XHTML 1.0 (January 2000): W3C considered HTML 4.01 as the final release for HTML, and moved on to develop XHTML 1.0 with stricter rules and syntaxes, followed by XHTML 2.0. XHTML 2.0, although theoretically elegant, is impractical as it is not backward compatible with HTML4/XHTML1.0. A rebel group called WHATWG (Web Hypertext Application Technology Working Group) continued to work on extending HTML with more features in a backward-compatible manner. In 2004, WHATWG released HTML5. By 2007, HTML5 has captured the attention of the developers. W3C decided to abandon the XHTML 2.0 and embraced the HTML5.
HTML 5 (October 2014): Published as W3C Recommendation.
Today, the prevailing specifications are HTML5 (2014) (@ http://www.w3.org/TR/2014/REC-html5-20141028/). Nonetheless, the most interesting thing about standards is that nobody really follows them strictly. Every browser (Chrome, Firefox, Opera, Safari and Internet Explorer) has its own variations and support the standards to various extents.

Markup Tags
HTML uses markup tags, such as <p> (for Paragraph), <h1> to <h6> (for Heading Level 1 to 6), <img> (for Image), <a> (for Anchor or Hyperlink), to markup a document. HTML markup tags perform these functions:

Layout the documents, e.g., <p> (layout as a paragraph), <h1> to <h6> (layout as heading level 1 to 6), <br> (perform a line break), <hr> (draw a horizontal rule), <table> (tabulating data), <ol> (layout an ordered list).
Provide link (called hyperlink) to another HTML document, via the <a> (Anchor tag). These hyperlinks, a distinct feature in HTML, greatly help the users in navigating the web and enrich the users' experience. Hyperlinks make the HTML popular.
Embed images, audios, videos, programs (in JavaScript, VBScript, Applet, Flash, or MS ActiveX control), and objects within an HTML document. HTML is multimedia! The hypertext document may contain texts, images, audios, videos, and even programs.
Separating Content and Presentation
The purpose of a markup language is to relieve the content provider from worrying about the actual appearance of the document. The author merely indicates (via markup tags) the semantic meaning of the words and sentences (such as paragraph, heading, emphasis, and strong), and leave it to the browser to interpret the markups and render the document for display on the screen. In other words, it allows the separation of content and presentation. The content provider focuses on the document contents, while the graphic designer concentrates on the view and presentation.

Nowadays, HTML should be used solely to markup the contents, while its companion technology known as CSS (Cascading Style Sheet) be used for defining the presentation of the document, so as to separate the content and presentation.

These are the common pitfalls in older HTML documents and you should avoid:

Do not specify "appearance" properties, such as foreground and background color, text alignment, font face, font size, border, margin and padding, in the HTML document. Use an external CSS instead to set the appearance and presentation. Presentation-related tags (such as <font>, <center>) and attributes (such as align, bgcolor, link, vlink, alink) have been deprecated in HTML 4, in favor of CSS.
Do not use nested tables or frame for formatting the document, use <div> and <span>, or HTML5 new tags such as <header>, <footer>, and <section>.
HTML Authoring Tools
HTML documents can be created by a wide range of tools, from simple plain text editors (such as Windows' NotePad, Mac's TextEdit) to sophisticated WYSIWYG authoring tools (e.g., DreamWeaver).

 

Let's go thru some HTML examples and the syntaxes. Do not attempt to start designing your website until you understand the CSS.
  
### 3.  HTML By Examples
#### 3.1  Example 1: Basic Layout of an HTML Document
Let's begin with a simple example to illustrate the basic layout of an HTML document.


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Basic HTML Document Layout</title>
</head>
<body>
  <h1>My First Web Page</h1>
  <hr>
  <p>This is my <strong>first</strong> web page written in HTML.</p>
  <h3>HTML</h3>
  <p>HTML uses <em>markup tag</em> to <em>markup</em> a document.</p>
</body>
</html>
