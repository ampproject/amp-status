status.ampproject.org
=====================

This is the source code of the AMP status page. This repository is a Github Pages instance, commits to this repository
are immediately and automatically reflected in [status.ampproject.org](https://status.ampproject.org/).

How to update
-------------

For new incidents, create a new file in the `_posts` directory. See `_posts/_1999-12-31-example.md` for instructions.
For existing incidents, edit the existing incident file.

Set the `active_incident` field in `_config.yml` to `true` to denote an ongoing incident. Remember to set it back to
`false` once the incident is resolved.

### Test locally

Before committing and pushing your code, test it locally by building it with [Jekyll](https://jekyllrb.com/). Run:
```
jekyll serve
```

And open the browser (`http://localhost:4000/` by default) to review your changes.
