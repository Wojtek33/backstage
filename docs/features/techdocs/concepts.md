# Concepts

This page describes concepts that has been introduced with Spotify's
docs-like-code solution in Backstage.

### TechDocs Core Plugin

The TechDocs Core Plugin is a MkDocs plugin created as a wrapper around multiple
MkDocs plugins and Python Markdown extensions to standardize the configuration
of MkDocs used for TechDocs.

[TechDocs Core](../../../packages/techdocs-container/techdocs-core/README.md)

### TechDocs container

The TechDocs container is a Docker container available at
[DockerHub](https://hub.docker.com/r/spotify/techdocs). It builds static HTML
pages, including stylesheets and scripts from Python flavored Markdown, through
MkDocs.

[TechDocs Container](../../../packages/techdocs-container/README.md)

### TechDocs publisher (Coming Soon)

### TechDocs CLI

The TechDocs CLI was created to make it easy to write, generate and preview
documentation for publishing. Currently it mostly acts as a wrapper around the
TechDocs container and provides a easy to use interface for our docker
container.

[TechDocs CLI](../../../packages/techdocs-cli/README.md)

### TechDocs Reader

Documentation generated by TechDocs is generated as static html sites. The
TechDocs Reader was therefore created to be able to integrate pre-generated html
sites with the Backstage UI.

The TechDocs Reader purpose is also to open up the opportunity to integrate
TechDocs widgets for a customized full-featured TechDocs experience.
([Coming Soon V.2](https://github.com/spotify/backstage/milestone/17))

[TechDocs Reader](../../../plugins/techdocs/src/reader/README.md)

### Transformers

Transformers is different pieces of functionality used inside the TechDocs
Reader. The reason to why transformers were introduced is to provide a way to
transform the html content on pre and post render. (e.g. rewrite docs links or
modify css)

[Transformers API docs](../../../plugins/techdocs/src/reader/transformers/README.md)