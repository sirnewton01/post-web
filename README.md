# The Post-Web

The current world-wide-web is an experiment mixing multi-media, hyperlinks and the internet.
In its early form it allowed anyone to write content with simple and freely available tools
and post it online for others to read from the comfort of their web browsers, which made
it easy to read and learn. It has gradually drifted from this ideal into something quite
different and terrible.

## Failure

It's difficult to pinpoint one particular failure point and doing so is probably unnecessary
and counterproductive. Instead, let's highlight the major failure points. The purpose of this
exercise is to derive a post-web (or post-webs) that would address many or all of these.

### Content: inaccessible or locked in

If you want to author something simple on the world wide web on your own it is largely impossible
for an average, yet computer literate, person. There are so many items to consider at all
points of the stack: IP addresses, routing, servers, monitoring, domain names, operating systems,
firewalls, web servers, proxies, server-side language / framework, client-side language / framework,
authentication, secure transport, HTML, styling and web browsers. Each point in this stack has suffers from a
number of problems that requires specialists or even entire industries to constantly monitor
and improve. It forces people to be willfully ignorant at their own peril.

Another option for an author is to pick proprietary frameworks or sites. On one extreme
you have micro-blogging platforms like Facebook and Twitter that take total and complete control
of hosting your content and even the content itself. You have no access to the source code
for these systems and so it is completely opaque to you how your data is being used until there
is a disaster and the companies are forced to reveal soome of the inner details. Many of these
sites are free to the end user and require highly skilled workers to maintain and so there is
constant pressure to resort to intrusive advertising or encroachment of privacy in order to 
pay their employees.

You could pick a variety of Wordpress blogging sites where you have slightly more control
and freedom with your content, but then you are still locked-in to the Wordpress system itself
unable to easily move your content onto another system. Moving off of the web entirely and onto
something else is also an exercise in futulity as the web itself makes it challenging to scrape
the flash away from the content so much so that enterprises have cropped up specializing in
just that.

### Security

Due to the increasing complexity of each point in the web stack and some lack of foresight security
has become another complex topic in its own right. A whole infosec industry has spawned in response
to problems, such as cross-site scripting, which were brought to the forefront because of the web
and its lack foresight. Instead, the web was and contues to be focused on pushing the boundaries of
infinite flexibility of the mashing and presentation of content at the cost of security. Ultimately,
end users have become numb or entirely uninformed of the problems leaving the tech industry along
with infosec to repair the damage afterwards.

### Size

The web now requires 2-3MB transfers for each web page on average. It is worth noting that much or
even most of this data does not constitute the actual content of the page. Instead, it is all
of the framework, branding and advertising for the site. There is abundant bloat.

Home, commercial and mobile internet technologies have responded so far with fatter pipes. Web
browsers have to do more aggressive caching. Web sites rely on highly security critical content
distribution networks to avoid overwhelming their servers with all of the transfers.

### Implementation complexity

Web browsers are famously large and complex code bases riddled with bugs and other problems.
They are second only to operating systems and database management systems in their immensity.
Mozilla, the maker of the Firefox web browser, is inventing their own highly sophistocated
programming language called Rust with the goal of preventing any code from entering the code base
that isn't 100% safe. This is a clear sign that the code base necessary to support a web browser
is no longer readable enough to rely on developers themselves and code review techniques to catch
serious errors.

The web standards are always in flux and getting larger all of the time. This helps to ensure
that web browsers are never really finished. The Chrome browser abandoned version numbers and instituted
transparent upgrades to force users to keep up when it would be unreasonable to ask them to update
on their own.

### Lack of transparency

Most web pages are too complex for all but the most savvy users to view the source and understand
what is happening. This lack of readability can be a real problem for a number of reasons. Most users
can't have a real understanding of what is going on when they perform an action on the page. The actions
are largely site-specific with little standardization.

The REpresentational State Transfer (REST) movement has attempted to standardize interactions of RESTful
APIs, but has fallen short of standardizing UI presentation and gestures. Each website remains entirely
unique necessitating more and more site interaction logic being executed by the web browser in the page.
As is typical with the web REST looks to be a passing fad that will soon be superceded by a much more
flexible and complex "GraphQL" system leaving REST behind along with JQuery, XHTML and the rest of the
trail of abandoned web standards.

### Hidden content

Content is often hidden from the user making it a real problem when some of that content is malicious.
Hyperlinks are often abbreviated hiding the real destination making it more difficult for users to
discern whether they are going to a trusted or untrusted site. The same applies to hidden HTML elements
on the page.

### Future fragile

Because the web is moving so quickly it is very easy for content that is as young as ten years old to
become obsolete and inaccessible. If you wrote a web site using Microsoft Silverlight or ActiveX at that time
it will no longer function with any modern web browsers. Likewise, a web site written today that relies on
a CDN to host the once popular JQuery library may not work if the CDN company goes out of business or
JQuery falls out of support as its use wanes. This can make it challening to maintain a website that
has old, but important data as it requires active maintenance and even rewriting the code and content
in order to keep up. An alternative is to rely on frameworks that themselves are future proof
and continue to be updated over time, which doesn't seem likely for many of them.. The only other
solution is to rely on internet archives, which themselves must be funded somehow and only work with
public, not private content.

In contrast, text files can be retrieved from Apple II or Commodore 64 tapes and read with any modern
text editor. The same can be said of old CompuServe GIF files. These are ancient scrolls in relative
terms. Say what you will about simple text but it is one of the most future-proof computer formats
in existence and one that is being used extensively in the lightweight markup community to great effect,
with github being a great example.

## Post-Web

The post-web is something that should emerge from the failures of the world-wide-web and attempt to fix
these problems while adding greater capability at a lower cost than the original. For those aware of the
history of computing an apt metaphor here would be to live in a world of Multics and finally have Unix.
Another way of putting this is that we live in a world of Mainframes (ie. Cloud, maybe) and we want our
personal computers. Users of the post-web should be capable of understanding some of the internal workings
without too much specialized knowledge because the system itself is designed with simplicity in mind.

### Text as the default

Much of the world-wide-web glosses over the actual content with branded and magazine-list presentation.
If content, not presentation, is the primary goal, which it should be, then the simplest and
most elegant way to represent that is plain text. That is not to say that there are cases
where other media types better represent or enhance the content, but text should be the default
unless there is good reason to deviate for a number of reasons covered below. This document being a
good example provided that you have checked it out with git or view it in "Raw" mode.

Over time text has gradually gained new capabilities. Unicode/UTF-8 has allowed us to add foreign
languages to our files. Also, certain mathematical symbols have been added recently. Even emojis
are relatively easy to use and ubiquitous in certain contexts. Markdown and other plain text formatting
languages standardize headings, hyperlinks and other document syntaxes. There are even plain text
languages for describing graphs, tables and diagrams in a somewhat readable way. The envelope is being
pushed further over time.

### Interoperability

Text can be read and processed with a wide variety of tools, many of which are provided as part
of your operating system. Unix has demonstrated a rich foundation based on text inputs and outputs,
which are easily lost when moving to rich file types, such as the world-wide-web. It should be possible
to use the post-web system with the standard operating system tools for the most part, which can help
to stem the repeated reinvention of these tools over and over for different file formats. If the standard
tools are too complex or incomplete then perhaps the operating system itself should be simplified.

It is worth mentioning that tools such as PGP (or GPG) are quite easy to use with text files. Cryptographic
signatures can be appended to the end of a text file. Decryption is also a relatively simple matter.

### Transparency

It is difficult to hide content in plain text. Opportunities for malicious content are much less.
Since everything is out in the open it forces the author to be more concise and clear, which is
probably a good thing in general. Even hyperlinks are exposed and not abbreviated preventing
phishing attacks.

### Hyperlinking

Hyperlinking is preferred over embedding because embedded content can be distracting. A hyperlink gives
the ready a means to access a related document and lets them control when or if that document should be
opened.

The preferred hyperlink format for the world-wide-web is URL and URI. There is alot of unneeded baggage
here. The protocol/scheme for most links is http or https, making it largely repetititive. The query
parameters are difficult to handle due to the possibility of repeating or non-repeating keys. All that
should remain is the host, path and fragment portions.

Relative paths are also quite handy at times to make documents host and path independent for intra-site
links.

### In-depth reading

Sometimes, a topic is worth exploring in more detail and over a longer period of time. Plain text is
great for reading short content or even exploring the breadth of information available but there are
better ways of digesting a large document in-depth. In those cases the user can convert text into a
rich text representation, such as PDF, for a focused reading session. Since an author can't know
how their content will be consumed by different readers making the plain text representation readable
is a necessity. They can use formats such as Markdown to enable conversion of their content into
rich representations, while making the plain text more readable as well.

### File extensions

File extensions are well used and understood by users. They also have operating system support.
This is in contrast with media types, which are hierarchical and needlessly complex. Many of the
reasons for the existence of media types are disappearing over time. Text file encoding is being
standardized around a single Uncide/UTF-8. Hierarchical meta-types, such as XML are in decline.
File extensions work just fine.

### RESTful text UI's

