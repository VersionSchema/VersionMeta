# VersionMeta
A project to define and promote a standard meta tag to reference a version schema.

Official web site: http://versionmeta.org/

## What's the point?
There are many versioning schemes in use today (ie;semver.org) with varying levels of support and documentation. None of these that I am currently aware of, have a machine readable schema or even include any pointers to their own definitions. The proposal here is something along the lines of, if you're SemVer for instance, then you'd have SemVer 3.0.0 {https://semver.org/schema}, rather than just the bare version scheme. Whats at the end of that URI has yet to be determined, but I suspect something along the lines of an XSD and/or whatever turns out to be the JSON or YAML equivalents, such that tools can instantiate a rules engine that can be used to automatically "reason" about the version number and it's relation to other version numbers for a given package.

There's a lot to be done on the schema end of this, but in the mean-time, we can begin to push for the definition and adoption of some initial meta conventions that can have some meaning to both humans and machines. Perhaps initially we push for all stakeholders to add at least soemthing like {DOCS!https://semver.org} to their version strings. That would be a good fall-back position that says here's the human readable description of this version string. At least then all the parsers are adapted to at least not freak-out when the additional tag is present.

Consider all the four digit version schemes out there. How does a product that uses SemVer internally and all their publicly available propaganda, map their version to the package-dejur's four digit scheme?  The advice today is, it depends!  With VersionMeta and VersionSchema, it's just a matter of mathmatics.

# Looking for stakeholders
- Anyone who owns an existing, documented version scheme.
- Anyone who owns or is a major influencer/contributor to software packaging/publishing tools.
- Anyone with any tool that reads and acts on any kind of version string.

