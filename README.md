# The Midwestern — archive site

A static, no-build archive of **The Midwestern**, a private Wisconsin-style
bar and game room in Oceanside, California, which is now closed.

## Where the content came from

The bar's original site, `themidwestern.yourwebsitespace.com`, was still live
and was fetched directly — home, about, and air hockey pages — along with
every photo it linked to. Copy on this site is that original text, lightly
turned from present to past tense for an archive, with the two press quotes
(Chicago Sun-Times, Milwaukee Journal Sentinel) kept verbatim. The ten photos
in `images/` are the originals, downloaded from the source site and renamed.

Facebook (`facebook.com/themidwesternbar`) and Yelp
(`yelp.com/biz/the-midwestern-oceanside`) were the other two sources named for
this rebuild. Both blocked automated fetching — Facebook redirected to a login
wall, Yelp returned a bot-check page — so no content from either was
available to pull in when this was first built. This site links out to both
(homepage and gallery page) as "see for yourself" references rather than
inventing quotes. If real access to either is available, that's the next
thing to fold in.

The look is original: an oxblood-and-brass, wood-and-parchment palette drawn
from the source site's own colors (its `rgb(85, 28, 0)` heading brown, its
warm cream and tan panel backgrounds), rebuilt as a modern responsive layout
rather than the original's fixed-width, absolutely-positioned 2013 markup.

## Structure

Four pages, matching the original site's map: `index.html` (Home),
`about.html`, `air-hockey.html`, and a `gallery.html` added here to hold all
ten recovered photos in one place. One stylesheet, `css/site.css`. No
JavaScript, no forms, no functions — there's nothing here that needs to run.

## Deploying

Plain static site at the repo root: `publish = "."`, no build command — see
`netlify.toml`. Point a Netlify project straight at this repo with no base
directory override. No environment variables are needed.

The whole site is `noindex, nofollow` (`robots.txt`, the Netlify headers, and
every page's `<meta name="robots">` all say so): it's a record for people who
already know to look for it, not something to promote.
