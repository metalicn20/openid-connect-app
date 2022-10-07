# OpenID Connect App

<p>
    <a href="https://github.com/ebrahimmfadae/openid-connect-app/blob/main/LICENSE" target="_blank">
        <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="Released under the MIT license." />
    </a>
    <a>
        <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs welcome!" />
    </a>
    <a href="https://github.com/ebrahimmfadae/openid-connect-app/last-commit" target="_blank">
        <img src="https://img.shields.io/github/last-commit/ebrahimmfadae/openid-connect-app? style=flat-square" alt="Last commit">
    </a>
    <a href="https://github.com/ebrahimmfadae/openid-connect-app/issues" target="_blank">
        <img src="https://img.shields.io/github/issues/ebrahimmfadae/openid-connect-app? style=flat-square"/>
    </a>
</p>

<p>
  Sample project for implementing <b>OIDC</b> server with a web application and an API service.
</p>

## Article reference

The article associated to this repository is written in 4 parts plus an introduction.

- Introduction: [Creating OpenID server with Node.js and MongoDB](https://dev.to/ebrahimmfadae/setup-openid-with-nodejs-and-mongodb-451j)
- Part I: [Develop an OpenID server with Koa & Typescript & EJS](https://dev.to/ebrahimmfadae/develop-an-openid-server-with-nodejs-typescript-9n1)
- Part II: [Persist OpenID server data with MongoDB](https://dev.to/ebrahimmfadae/persist-openid-server-data-with-mongodb-5f95)
- Part III: [Add a resource server to an OpenID provider](https://dev.to/ebrahimmfadae/add-a-resource-server-to-an-openid-provider-noo)
- Part IV: [OpenID security configuration](https://dev.to/ebrahimmfadae/openid-security-configuration-4nn8)

## Project requirements

The project is developed and tested in this environment.

```
$ node -v
v16.17.0

$ yarn -v
v1.22.19

$ docker
Docker version 20.10.7, build f0df350

$ docker-compose version
Docker Compose version v2.11.2
```

## Run

Step one, install the dependencies

```
$ yarn install
```

We can move the `yarn install` step to the container, but installing the dependencies inside the container when we have no caching bothers me! Especially in the development phase.

Step two, start the containers.

```
$ yarn docker-compose:up
```

You can see the front end by navigating to [http://localhost:3005](http://localhost:3005) with your browser.

To shut down the containers, run this command.

```
$ yarn docker-compose:down
```

## How to Contribute

To suggest code change, Open an issue or create a pull request.
