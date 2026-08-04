# talk2fit-pp — retired

The Talk2Fit site moved to **https://talk2fit.app** (built from `web/` in the
main app repository).

Every page here is now a redirect. They are kept, not deleted, because links
to them are already in the wild: store-console fields, invite messages people
have sent, and whatever search has indexed. Deleting the pages would turn all
of those into 404s.

The redirects preserve the query string and the fragment, which is not
decoration:

* `/get/?ref=CODE` — invite links already sent carry the referral code;
* `/support.html#delete-account` — Google Play requires a working
  account-deletion URL.

GitHub Pages cannot issue a real 301, so each page uses a canonical link, a
script redirect and a meta refresh together.
