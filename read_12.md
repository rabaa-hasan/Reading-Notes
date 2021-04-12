# EJS Partials

Partials are like functions, they make larger websites easier to maintain so you don't have to go and change a piece of text in every page it appears in. You define a resulable bundle of code in a file and include it wherever you need it.

Our home page will look like so:

![e](https://miro.medium.com/max/2538/0*VngdKfkNNx5f2un0.png)

and the post page:

![e](https://miro.medium.com/max/700/0*oUmdAzjcwkQZb_AR.png)

As you can see from the above, the same navigation bar and footer appear in both the home and post view. This makes them perfect candidates for partials.

To  create a views/partials directory file that is called __navbar.js__ :

```
<!-- views/partials/navbar.ejs -->
    <div class="header clearfix">
        <nav>
            <ul class="nav nav-pills pull-right">
                <li role="presentation"><a href="/">Home</a></li>
            </ul>
            <h3 class="text-muted">Node.js Blog</h3>
        </nav>
    </div>
```

__Footer.js__ :

```
<!-- views/partials/footer.ejs -->
    <footer class="footer">
        <p>© 90210 Lawyer Stuff.</p>
    </footer>
```

Now that we have our partials defined, we can use them in our home.ejs and post.ejs templates! In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters (you could change these delimiters if you really wanted to).

The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’,

