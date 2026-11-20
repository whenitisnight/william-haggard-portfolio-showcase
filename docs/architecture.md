# Architecture

React and TypeScript provide the interface, using an App Router application deployed through Cloudflare Workers. D1 and a typed database layer hold durable profile and project content; R2 stores uploaded images. Source deployments are separate from studio edits.

The public site queries published records. The studio uses platform sign-in plus a server-side owner allowlist. Shared validation, same-origin writes, safe URL schemes, file-signature checks and revision comparisons protect the content boundary. These mechanisms are implementation features, not an independent security certification.

The project map and index are views of the same paginated records. Stable IDs and slugs support connected projects, direct story URLs, import reconciliation and next-project navigation. Motion can stop when paused, hidden or reduced motion is requested, with a fallback when the WebGL background is unavailable.
