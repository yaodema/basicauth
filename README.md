# basicauth
Basic Authentication Token Generator in HTML5

This project was made after trying to find anything similar online from a source I could recognize. Since it didn't appear to exist, I went ahead and made it.

Whatever is typed in the "username" and "password" fields will be converted from JavaScript's UTF-16 into UTF-8 bytes, concatenated with a single
colon in between, and converted into a base64 token for use with HTTP Basic Authentication. The conversion happens as you type into the fields.

The index.html file is the generator itself. All instructions are included in text on the generator, and it uses very plain HTML for all of its
elements, with no CSS necessary. If this impacts readability, I can add CSS to make it look far nicer.

The original index.html file in the initial commit took less than two hours to write. As it was made so quickly, there is likely room for
improvement. Feel free to create a new issue on the tracker if you find anything that needs sprucing up!

## OK, but, why?

I've had a few people ask what the use-case is for this project, in the first
place. XMLHttpRequest.open() already does Basic Auth in the browser, and most
languages have HTTP functions that do the same, so why would we need this?

While I do recommend that projects use those functions instead of a pre-built
Basic Auth token whenever possible, there are some apps out there that just
don't do this for the user, and expect a pre-built token to be entered into them
manually. Sometimes this affects the whole app, while other times it affects
just some modes of the program. Either way, I ran into one of these cases
recently, so I felt I needed to make this.

If you haven't dealt with a program that has this quirk, count yourself lucky!
Someday, if you do need this, the tiny HTML file you see here will do the trick.

