# Structure web pages with HTML
## How People Access the Web

1. Browsers
People access websites using 
software called a web browser. 
Popular examples include 
Firefox, Internet Explorer, Safari, 
Chrome, and Opera.
2. Web Servers
When you ask your browser for 
a web page, the request is sent 
across the Internet to a special 
computer known as a web 
server which hosts the website.
3. Devices
People are accessing websites 
on an increasing range of devices 
including desktop computers, 
laptops, tablets, and mobile 
phones.
4. Screen readers
Screen readers are programs 
that read out the contents of a 
computer screen to a user. They 
are commonly used by people 
with visual impairments.

All websites use HTML and CSS, but content 
management systems, blogging software, and 
e-commerce platforms often add a few more 
technologies into the mix.

## How the Web Works
1. When you connect to the web, 
you do so via an Internet Service 
Provider (ISP). You type a 
domain name or web address 
into your browser to visit a site.
2. Your computer contacts a 
network of servers called 
Domain Name System (DNS) 
servers. These act like phone 
books; they tell your computer 
the IP address associated with 
the requested domain name. 
An IP address is a number 
of up to 12 digits separated 
by periods / full stops. Every 
device connected to the web 
has a unique IP address; it is 
like the phone number for that 
computer.
3. The unique number that the 
DNS server returns to your 
computer allows your browser 
to contact the web server 
that hosts the website you 
requested. A web server is a 
computer that is constantly 
connected to the web, and is set 
up especially to send web pages 
to users.
4. The web server then sends the 
page you requested back to your 
web browser.

HTML Uses Elements
to Describe the 
Structure of Pages
Each 
element has an opening tag and a closing tag.

## The Evolution of HTML
__HTML 4__
Released 1997

__XHTML 1.0__
Released 2000

__HTML5__
Released 2000

## DOCTYPES
Because there have been
several versions of HTML, each
web page should begin with a
DOCTYPE declaration to tell a
browser which version of HTML
the page is using (although
browsers usually display the
page even if it is not included).
We will therefore be including
one in each example for the rest
of the book.
## Comments In HTML
<! --  -->

If you want to add a comment
to your code that will not be
visible in the user's browser, you
can add the text between these
characters:

< !-- comment goes here -->
## ID Attribute
Every HTML element can carry
the id attribute. It is used to
uniquely identify that element
from other elements on the
page. Its value should start with
a letter or an underscore (not a
number or any other character).
It is important that no two
elements on the same page
have the same value for their id
attributes (otherwise the value is
no longer unique).
## Class Attribute
Every HTML element can
also carry a class attribute.
Sometimes, rather than uniquely
identifying one element within
a document, you will want a
way to identify several elements
as being different from the
other elements on the page.

## HTML Layout Elements
HTML has several semantic elements that define the different parts of a web page:

< !DOCTYPE html>

< html>

< head>

< title>HTML5 Layout< /title>


< /head>

< body>

< header>< /header>

< nav>< /nav>

< main>< /main>

< footer>< /footer>

< /body>

< /html>


