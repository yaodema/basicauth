# basicauth
Basic Authentication Token Generator in HTML5

This project was made after trying to find anything similar online from a reputable source. Since it didn't exist, I went ahead and made it.

Whatever is typed in the "username" and "password" fields will be converted from JavaScript's UTF-16 into UTF-8 bytes, concatenated with a single
colon in between, and converted into a base64 token for use with HTTP Basic Authentication. The conversion happens as you type into the fields.

The index.html file is the generator itself. All instructions are included in text on the generator, and it uses very plain HTML for all of its
elements, with no CSS necessary. If this impacts readability, I can add CSS to make it look far nicer.

The original index.html file in the initial commit took less than two hours to write. As it was made so quickly, there is likely room for
improvement. Feel free to create a new issue on the tracker if you find anything that needs sprucing up!
