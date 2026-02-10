# ah-journal-template

## My Journal Template
---
This is a template journal made from standard HTML5 and tailwind CSS and NO Javascript.
The journal template is structured in the following manner:

- css/input.css - the input CSS that imports tailwindcss and packages, used as input to the tailwindcss CLI
- css/output.css - the output CSS that includes the CSS for the styles used in the HTML documents
- src/index.html - the root or home page for the journal
- src/about.html - the page containing info about me and a contact form
- src/archives.html - the page containing the chronological list of posts
- src/404.html - the page for error handling
- src/thank-you.html - the page to show when the contact form has been submitted
- src/feed.xml - the RSS XML feed
- src/images/blog.png (the logo for my blog)
- .gitignore - the file containing files or folders not to commit to get
- src/notes/YYYY/MM - the folder containing the list of journal notes
- src/tags/<tag-name>/index.html - the tag name, the index.html contains the list of notes that match the tag

## Building
To build the code you need to make sure that node is installed. Then, install tailwindcss and related packages:

`npm install tailwindcss @tailwindcss/cli`

`npm install -D @tailwindcss/typography`

`npx @tailwindcss/cli -i ./src/css/input.css -o ./src/css/output.css`

## Running locally
To run the a local web-server to test the site, `cd src` and then

`python3 -m http.server &`

As you are developing you may want to run the tailwindcss CLI in `--watch` mode to update the `output.css`.

`npx @tailwindcss/cli -i ./css/input.css -o ./css/output.css --watch`
