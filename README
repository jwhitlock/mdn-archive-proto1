This is a prototype of exporting MDN revisions to files.

Prototype 1
---
Revisions are exported as GitHub commits. The revision comment becomes the commit message, and the MDN name and username is used to construct authorship.

English documents are stored in content.md at a path related to their slug.
The format is inspired by Jeykl.
A section at the top has revision metadata as a key-value table.
The raw content, including unrendered macros, appears in the next section.

The export script attempts to place translations in the same folder as the English revision.
This is not always possible, and the translations are not moved when the English page is moved.

This prototype doesn't attempt to gather redirect data, or other data.

How this was generated
---
This depends on the Kuma development environment.

The base image doesn't include ``git`` by default. I added ``git`` in ``docker/images/kuma_base/Dockerfile``, and rebuilt locally with ``VERSION=latest make build-base``.

The script ``export_revisions.py`` is placed in the root of Kuma repo. I enter the environment with ``make bash``, then run ``./manage.py shell_plus``, and ``import export_revisions; export_revisions.do_it()``. It took about an hour to export the 2354 revisions in the sample database.

This script creates the repo in a new ``revisions`` subdirectory. This directory needs to be moved or renamed to run the script.

I then added this README and other data to the generated repo before pushing.

Next steps
---
I still think there is a lot of work before we can use a GitHub-based contribution model for edits. My plan is to ship projects with incremental benefits:

* Ask MDN contributors (as a profile setting) how they want their authorship on GitHub.
* A git-based archive of MDN content, such as this. It can be generated periodically. More work is needed to define the format, and to handle issues like redirects.
* An offline renderer that generates a static version from the archive. I believe at least two passes would be required, one to collect metadata, and a second to render. New code as well as a highly modified version of KumaScript would be needed to accomplish this. A deliverable would be a second repository with the statically generated HTML and metadata.
* Linting and contribution tools that make it easier to author content in the "archive" format. Tools would be needed for common operations such as moving page, linters to prove the edit is consistent, and algorithms to minimize the number of pages regenerated for an edit.
* Incorporate the new workflows into MDN. It is unclear if this should be a "big bang" conversion of all pages, or if it would be better to select a little-used subset (Archives) or a subset needing refreshing (HTML docs).

Others will probably be less patient and more willing to break everything.
