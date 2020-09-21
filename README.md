# ⏪ Reverse proxy

A very simple and fast reverse proxy for Nginx + Docker with custom JavaScript injection. It's largely based on [caprover/nginx-reverse-proxy](https://github.com/caprover/nginx-reverse-proxy) with custom script injection.

## 💻 Getting started

To use with Caprover:

Create a new app with the name "reverse-proxy" and add GitHub repository details. The [`captain-definition`](./captain-definition) file will take over from there.

Use with Docker:

```bash
docker run -p 1234:80 --env UPSTREAM_HTTP_ADDRESS='https://example.com' --env SCRIPT_URL='https://example.com/script.js' kojhub/reverse-proxy
```

Then, http://localhost:1234 will show you https://example.com.

## 📄 License

[MIT](./LICENSE) © [Koj](https://koj.co)

<p align="center">
  <a href="https://koj.co">
    <img width="44" alt="Koj" src="https://kojcdn.com/v1598284251/website-v2/koj-github-footer_m089ze.svg">
  </a>
</p>
<p align="center">
  <sub>An open source project by <a href="https://koj.co">Koj</a>. <br> <a href="https://koj.co">Furnish your home in style, for as low as CHF175/month →</a></sub>
</p>
