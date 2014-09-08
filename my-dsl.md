# Language
The DSL I will be discussing is the Wiki Markup Language.
A reference can be found at the [help page] (http://en.wikipedia.org/wiki/Help:Wiki_markup).


# Domain
Wikimedia formatted web pages

# Computational model
The Wiki Markup language is used to generate web pages using MediaWiki. A program is executed
when it is rendered as viewable content. MediaWiki is written in PHP and generates HTML
as defined by the simplified wiki markup. This HTML is then rendered as usual.

# DSL-ness
This language is very far on the "purely" domain-specific side of the spectrum.
As a markup language, and one considerably less complex than HTML, wiki markup is able only
to describe specific types of web page content with an emphasis on article-style headers,
tables, and links. None of the standard general-purpose language attributes that create
what we think of as program flow exist.

# Internal or external?
The language is an external DSL. It defines its own syntax external to HTML, and is parsed
by MediaWiki as its own syntax.


# Host language
As it is an external DSL, no other existing language was used to implement the DSL.
The syntax, similar to markdown, uses special characters such as = and ', among others,
to describe common markups such as headers and emphasized text.


# Benefits
The language is considerably more code-efficient than HTMl for many of the tasks
which are used heavily by Wikipedia-style articles. For example, headers, and emphasis are
created using text characters without the need for HTML tags. Similar to markdown,
links are created without the clutter and complication of <a href> silliness which can often
be confusing. The common markup operations are both simplified and emphasized by the syntax
of the DSL, making it easier to create article-style markup without the clutter of tags.


# Drawbacks
Wiki markup is less expressive than HTML, and therefore less powerful in the content that it can represent.
In particular, it does not naturally interface with CSS, making it very difficult to format the
representation of pages that are not simply single-column articles. Additionally, the format for content
in tables makes it difficult to predict the exact output that will result in more complicated cases
that could be more carefully controlled in HTMl.
