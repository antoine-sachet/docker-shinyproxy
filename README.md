# docker-shinyproxy

Docker image for Shinyproxy server. Just add the yml configuration and run!

# Example

The following `Dockerfile` will launch a shinyproxy server configured from an application.yml.
Everything is already set in the shinyproxy-base: the WORKDIR, the CMD, etc.

Just add the config (and any required resources e.g. a favicon in `www/`).

```
FROM asachet/shinyproxy-base:SP2.3.0
# CMD is already set to running the shinyproxy jar
COPY application.yml .
```
