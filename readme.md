# Secure Traefik configuration

## What is this?

A simple Traefik configuration with SSL using ACME and Digitalocean DNS. It also has Wordpress set up for an example.

## How to use this?

1. Create acme.json and give permissions
```sh
touch /acme.json \ && chmod 600 /acme.json
```
2. Create .env

[example .env](/.env-example)

3. Create traefik.yaml

[example traefik.yaml](/traefik-example.yaml)

4. Go to https://www.ssllabs.com/ssltest/

5. Idk profit maybe???

## Javascript doesn't work!!??

Remove `ContentSecurityPolicy` line from [dynamic.yaml] and you're good to go!

## Why?

I took way too long to do this right. Some say that Traefik documentation is great, though it was really confusing for me. Use this repo as a reference.
