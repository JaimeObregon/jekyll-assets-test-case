# jekyll-assets-test-case
A test case for jekyll/jekyll-assets#268

## Steps to reproduce

1. `git clone` this repo.
2. `bower update`.
3. `jekyll build`.
4. Check line 572 at `build/assets/app.js`, and compare it to line 571 at `source/_assets/lib/mustache.js/mustache.js`.

Results:

    mustache.tags = [ '{{', '}}' ];

Expected:

    mustache.tags = [ ', ' ];
