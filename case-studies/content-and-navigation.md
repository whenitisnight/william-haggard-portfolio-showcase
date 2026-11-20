# Making the visual map maintainable

A visual portfolio becomes expensive to maintain when every new project requires hand-editing the layout. I chose a shared content model so the expressive map and the straightforward index remain consistent as projects are added or archived.

The studio stores project status, ordering, relationships and media separately from the code. A deliberate tracker import updates the selected fields while preserving authored stories, images and existing URLs. Stable tracker identifiers prevent duplicates. The importer validates the complete selection before its atomic update; projects absent from an import remain unchanged.

The same separation creates an operational obligation: Git preserves source, while content and image objects need separate exports/backups. A repository push cannot substitute for a content backup. The visual map also remains an optional way to browse; the index and keyboard paths provide a simpler route to the same work.

Earlier source checkpoints are preserved in the same private repository. The current design is an evolution of the portfolio rather than a collection of duplicate websites.
