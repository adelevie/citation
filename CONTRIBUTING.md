## Public domain

The project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication][CC0].

All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.

[CC0]: http://creativecommons.org/publicdomain/zero/1.0/

## Browser Builds

`citation` uses `gulp` and `browserify` and a few other tools to create browser-ready builds.

If you modify any `citation` code and want to send a pull request, please update the browser builds (located in the `browser` folder) by running `gulp`. (Install `gulp` first by running `npm install gulp -g`.)


If you are unable to do this, you should still contribute! Just make a note of this in the text of the pull request.

Currently three different files are created for browser use:

1. `browser/citation.js`: an unminified, uncompressed version. Good for development, and includes a (large) source map so that debugging references the original files and line numebrs. Very unideal for production **>1 MB**.
2. `browser/citation.min.js`: a minified, uncompressed version. Decent for production, does not include a source map. **~200 KB**.
3. `browser/citation.min.js.gz`: a minified, gzipped version. Best for production. **~50 KB**.