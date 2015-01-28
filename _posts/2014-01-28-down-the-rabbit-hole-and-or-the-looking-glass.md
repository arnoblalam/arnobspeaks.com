---
categories: rants
---

# Or how I learned to stop worrying and use kramdown

Every language describes its own entity escaping rules. For urls, "special characters" need to be percent escaped.  For HTML, non-ASCII entities usually need to be ampersnad escpaed.  __Markdown__ also describes it's own set of characters that need to be escaped.  One of the problems with these escaping rules is that we often need to embed one language into another.  For example, in order to include math on an article written using __Markdown__, we might use __LaTex__.  __LaTex__ has its own ideas about escaping, but cruicially, it uses the same character to denote the start of an escape sequence as __Markdown__ (that is, the \\ character).  This leads to bizarre situations where we need to escape the \\ character so that it reaches the __LaTex__ processor after being processed by the __Markdown__ processor (that is, we need to insert \\\\ instead of \\, so that the __LaTex__ processor still sees a single \\ after the __Markdown__ engine is done preparing the document.)  The truly bizzare comes about when we want to insert two slashes, to indicate to the __LaTex__ processor that we mean to begin a new line.  This is accomplished by inserting \\\\\\\\ (that is 4 slashes) whenever we want to start a new line.


Clearly this doubling up of slashes is not a sustainable model.  __XML__ had a brilliant idea of marking off sections of a document that should not be processed (parsed) by an XML processor using the CDATA (character data) tag (as opposed to everything esle, which was PCDATA or parsed character data).  However, the default __Markdown__ engine that comes with __Jekyll__ does not allow you to similarly mark off an area for "non-processing" (even indenting does not help). The __Kramdown__ engine does allow one to mark a section of the text as a math area by using \$\$.

tl;dr: If you need to include __LaTex__ in your blog, use kramdown (over __Maruku__ and __Redcarpet__)