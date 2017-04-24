# CRTR: A Social Curation Tool for Museums

### Background

[Read the blogpost here.](https://cms633.github.io/updates/peter-pojiang-chaoran-xinwen-project-summary.html)

### Technical Overview

* Backend
    * Python
    * [Django](https://www.djangoproject.com/) because of past experience and ease of development.
    * [Postgres](https://www.postgresql.org/) as primary data store.
        * This supports some [full text search](https://www.postgresql.org/docs/8.3/static/textsearch.html) concepts, which we will use as first stab at implementation. If more complex queries are needed, we'll use [Elasticsearch](elastic.co).
    * [Fast R-CNN](https://github.com/rbgirshick/fast-rcnn#requirements-hardware) implementation for doing some feature extraction. Can hopefully also be used for [similarity search](http://code.flickr.net/2017/03/07/introducing-similarity-search-at-flickr/).
        * Instead of silly hand-rolled, maybe use [FALCONN](https://falconn-lib.org/pdoc/falconn/) for cosine similarity search
        * It would be dope to find a trained version of [this model](https://arxiv.org/pdf/1412.7755v2.pdf)
* Frontend
    * Frontend components will be created with [React](https://facebook.github.io/react/).
    * Standard HTML/CSS

### Timeline
* April 19, 2017 – Initial Project Presentation, feedback
* April 26, 2017 – Short write-up of project progress (Github), brief in-class presentation, possible paper prototype
* May 3, 2017 – Written summary of project progress, draft of Digital Prototype, refinement of prototype, brief presentation & feedback in class
* May 10, 2017 – Presentation of prototypes (dry run), draft of final paper
* May 17, 2017 – Presentations of completed projects, design document completed 