# README

## What is this?

The Rust community has a number of websites dedicated to keeping track of the state of the ecosystem for specific purposes. (e.g. [arewewebyet](http://www.arewewebyet.org) and [arewelearningyet](http://www.arewelearningyet.com))

This one tracks the state of the ecosystem for Game Development in Rust.

## Contribute
Arewegameyet? uses [semantic-ui](http://semantic-ui.com/), and [zola](https://github.com/getzola/zola) the Rust static site generator. 

### Add to the Ecosystem listing

1. Navigate to whichever folder in `/content/categories/` best fits your project.

2. Edit that folder's `data.toml` file in any plain text editor or straight through [GitHub's editor](https://help.github.com/articles/editing-files-in-another-user-s-repository/).

3. (a) If your library has been published to [crates.io](https://crates.io/) then all you need to do is enter the exact name of your crate and set the source to `crates`, like this:

```
[[crates]]
name = "lewton"
source = "crates"
```

3. (b) If you haven't published to crates you can link directly to your GitHub code repository instead by setting the name to the `user/project` and setting the source to `github`:

```
[[crates]]
name = "Gigoteur/UnicornConsole"
source = "github"
```

4. At this point your PR is ready to be sent. However there's some optional data fields that could be added if applicable.

    `gitter_url = "https://gitter.im/UnicornConsole/Lobby"` takes a full URL. While it's called `gitter_url` feel free to link whichever is the default discussion platform for your project.

    `homepage = "https://gitlab.com/Siebencorgie/jakar-engine"`takes a full URL. Can be used to link to your homepage or a custom URL not yet supported in our default data entries, e.g. like the GitLab link above.

**All done!** We do greatly appreciate PRs, but if you're not comfortable with this process you're welcome to open an issue requesting the addition of your project instead.

### Add a Resource or Game

Resources and games don't have support for data files yet, so you'll have to edit raw HTML in order to add a new entry. 

HTML for resource entries:

```html
<a class="ui card" href="https://doc.rust-lang.org/book/">
    <div class="content">
        <div class="header">The Rust Book</div>
        <div class="meta">Book</div>
        <div class="description">
            The Rust language official book.
        </div>
    </div>
    <div class="ui bottom teal attached button">
        Read
    </div>
</a>
```

HTML for game entries:

```html
<a class="ui card" href="https://rap2hpoutre.github.io/llamassacre-website/">
    <img class="ui image" src="https://rap2hpoutre.github.io/llamassacre-website/screen.png">
    <div class="content">
        <div class="header">Llamassacre</div>
        <div class="description">
            A jump and bump game for two players made with ggez.
        </div>
        </div>
</a>
```

### Enhance this website

If you're comfortable with semantic-ui and Zola please reach out to us in the Issues with your enhancement ideas or just to state your willingness to contribute.

### Errors
It's very likely there are mistakes around, if you find one please file an issue.


*Thanks for helping us map the Rust game development ecosystem!*
