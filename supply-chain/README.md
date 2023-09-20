A [`cargo-vet`](https://github.com/mozilla/cargo-vet) audit aggregation folder.

## First party audits

All audits performed as part of my projects will be aggregated into
`first-party-audits.toml` for use by anyone that wants to import it.

## Third party audits

Rather than configuring every project with their own `imports` lists I aggregate
all trusted third party audits into this repo, then simply import that list into
my projects. (If `cargo-vet` were to get the ability to have a trusted
transitive import then this will be replaced by that mechanism, but since it
doesn't I have to copy all the audits into a central location).
