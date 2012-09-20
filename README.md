# Git dns hooks

Checks zone sanity before deploying updates to production

# Features

## Checks

- Zones compiles with zonec
- SOA serial has been incremented

# Deployment

- Rebuild nsd db
- Reload nsd

# Install

Put files in directory hooks of your git repo

## Files pattern

Forward zones:
  forward.foobar.com.db

Reverse zones:
  reverse.foobar.com.db


# LICENSE

2 clause BSD

# TODO

- sanity check reverse zones
- handle dnssec (see https://gist.github.com/2125545)

