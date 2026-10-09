# Editing your site

Every change: open `index.html` in GitHub, click the pencil, use Ctrl+F to find the spot, make the change, then click **Commit changes**. The live site updates in a minute or two (hard-refresh with Ctrl+Shift+R).

## Add a photo or graphic
1. Upload the file to the right folder, e.g. `images/tigers/new-shot.jpg` (export around 1200 px on the long side).
2. In `index.html`, find the page's list (search `org:tigers`, `org:bisons`, `org:bulldogs`, or a service like `service:photography`) and add one line:
   - Photo: `p("Warmup: Smith", "", img("tigers/new-shot.jpg")),`
   - Graphic: `g("Home opener", "", img("tigers/home-opener.jpg")),`

On a service page, put the organization in the second spot so it shows under the title: `g("Home opener", T.tigers, img("tigers/home-opener.jpg")),`

## Add a YouTube video
No upload needed. The ID is the part after `youtu.be/` (or after `v=`).

`y("Season hype video", "", "npiEUs-_MR8", "shot-edited"),`

Credit options: `"shot-edited"`, `"edited"`, `"edited-some-shot"`, your own wording in quotes, or `""` for none.

## Add a section to the More page
Search `var MORE` and add:

`{name:"New Client", items:[ g("Event poster", "", img("more/poster.jpg")) ]},`

## Change text
Search for the sentence (your bio, a job title) and retype it.

## Social links and contact form
- Search `var SOCIAL` and paste your full profile links. Buttons only appear once a real link is in.
- Search `var CONTACT_EMAIL` and type your email between the quotes. "Send message" will then open the visitor's email app with their message filled in.

## Avoid these
- Apostrophes in text: type `’` (curly) or `&rsquo;`, never a straight `'`.
- Every gallery line ends with a comma except the last one in its list.
- Keep the quote marks around each piece of text.

If a page goes blank after a change, one of those is usually why. GitHub keeps every version, so you can roll back from the file's History.
