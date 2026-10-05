# Update the portfolio without a full redeploy

One Wasmer deploy is required for this version, because the live site is still the old static file.

After that deploy, new projects do not need a rebuild.

1. Edit projects.json in this repo.
2. Commit it to main.
3. Refresh https://mohammedaminegoumri.wasmer.app/

The page fetches projects.json from GitHub on each visit. The count and cards update from that file.

Add a project by appending an object with id, cat, filter, title, desc, long, tags, and url.
filter must be one of: bi, ai, data, web.
