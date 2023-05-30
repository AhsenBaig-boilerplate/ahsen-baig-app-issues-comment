# GitHub-App-Issues-Comment

> A GitHub App built with [Probot](https://github.com/probot/probot) that GitHub App for issues that adds a comment.

## Setup

### Create a new Probot app

> Version: v5.0.9 - As the latest version of Probot is not compatible with Node v8.0.0 and higher
>```
>npx create-probot-app@v5.0.9 ahsen-baig-app-issues-comment
>```

```sh
code .\ahsen-baig-app-issues-comment\
```

### Start the app

> Install dependencies
>```sh
>npm install
>```

```sh
npm start
```

> Or change port
>```sh
>npm start -- --port 8000
>```

### GitHub sync


```sh
git init
git remote add origin https://github.com/AhsenBaig-boilerplate/ahsen-baig-app-issues-comment.git
git pull origin main --allow-unrelated-histories
```

### Start smee
> See .env WEBHOOK_PROXY_URL for smee url
> ```sh
> smee -u https://smee.io/<smee-id>
> ```

### Docker

```sh
# 1. Build container
docker build -t ahsen-baig-app-issues-comment .

# 2. Start container
docker run -e APP_ID=<app-id> -e PRIVATE_KEY=<pem-value> ahsen-baig-app-issues-comment
```

## Resources

- [Probot documentation](https://probot.github.io/docs/) - learn about Probot
- [Developing an app](https://probot.github.io/docs/development/) - Getting started guide

## Contributing

If you have suggestions for how GitHub-App-Issues-Comment could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

For more, check out the [Contributing Guide](CONTRIBUTING.md).

## License

[ISC](LICENSE) © 2023 Ahsen Baig
