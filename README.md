# status.ampproject.org

This is the source code of the AMP status page. This repository is a Github Pages instance, commits to this repository
are immediately and automatically reflected in [status.ampproject.org](https://status.ampproject.org/).

## How to update

* Clone this repository: 
  `git clone git@github.com:ampproject/amp-status.git`

* **For new incidents:**

  * Create a new file in the `_posts` directory by creating a copy of `_posts/_1999-12-31-example.md`, e.g.:
    `cp _posts/_1999-12-31-example.md _posts/2018-01-03-this-is-fine.md`
  
  * Make sure that the new post file *does not* begin with an _ underscore.

  * Modify the `title` and `date` field in the section between the three dashes

  * Modify the text description of the incident below the three dashed section

  * Set the `active_incident` field in `_config.yml` to `true` to denote an ongoing incident

* **For existing incidents:**

  * Edit the text description of the incident in the latest `_posts` file

* **Once the incident is over:**

  * Set the `active_incident` field in `_config.yml` to `false`

* Test your changes locally by building and serving them with [Jekyll](https://jekyllrb.com/): `jekyll serve`

* Open the browser (`http://localhost:4000/` by default) to review your changes.

* Commit and push the changes: `git commit -am "Short commit description" && pit push`

* Refresh `http://status.ampproject.org/`. Your update should appear within 30 seconds

### I don't have Jekyll installed

Testing and building locally requires Jekyll>3.x. If your package manager does not have Jekyll>3.x, install it with
`gem install jekyll`
