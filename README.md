# The Post-Web

The current world-wide-web is an experiment mixing multi-media, hyperlinks and the internet.
In its early form it allowed anyone to write content with simple and freely available tools
and post it online for others to read from the comfort of their web browsers, which made
it easy to read and learn. It has gradually drifted from this ideal into something quite
different and terrible.

## Failure

It's difficult to pinpoint one particular failure point and doing so is probably unnecessary
and counterproductive. Instead, let's highlight the particular failure points for the purpose
of analysis. The purpose of this exercise is to derive a post-web (or post-webs) that would
address many or all of these.

### Content: inaccessible or locked in

If you want to author something simple on the world wide web on your own it is largely impossible
for an average, yet computer literate, human. There are so many items to consider at all
points of the stack: IP addresses, routing, servers, monitoring, domain names, operating systems,
firewalls, web servers, proxies, server-side language / framework, client-side language / framework,
authentication, secure transport, HTML, styling and web browsers. Each point in this stack has suffers from a
number of problems that requires specialists or even entire industries to constantly monitor
and improve leaving an author bewildered or worse. It forces them to be willfully ignorant at their
own peril.

Another option for an author is to pick proprietary frameworks or sites. On one extreme
you have micro-blogging platforms like Facebook and Twitter that take total and complete control
of hosting your content and even the content itself. You have no access to the source code
for these systems and so it is completely opaque to you how your data is being used until there
is a disaster and the companies are forced to reveal soome of the inner details. Many of these
sites are free to the end user and require highly skilled workers to maintain and so there is
constant pressure to resort to intrusive advertising and invasion of privacy to pay their
employees.

You could pick a variety of Wordpress blogging sites where you have slightly more control
and freedom with your content, but then you are still locked-in to the Wordpress system itself
unable to easily move your content onto another system.

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

