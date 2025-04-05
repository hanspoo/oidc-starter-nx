# oidc react keycloak starter nx

React-oidc-context starter with keycloak, built with a simple React project with Nx.

We’ve used the bare minimum libraries, adding only some presentational support with Tailwind, Daisyui, and Heroicons.
The idea is to make it as agnostic as possible so it can serve as a generic starting point.
It provides a good user experience for detecting errors in the Keycloak server and is quite responsive. The mobile version features a disappearing left bar with a hamburger menu and an avatar icon for the user and its session.

This is a sample starter for a react project:

- react
- keycloak
- react-oidc-context
- nx
- tailwind & daisyui
- Hamburger menu
- Sidebar when logged in

## Quick start

(quick video)[https://www.youtube.com/watch?v=NVn1Ewt2t7M]

```
git clone https://github.com/hanspoo/oidc-starter-nx
cd oidc-starter-nx/
npm install
```

Copy .env.sample to .env

```
cp .env.sample .env
```

In one terminal start the keycloak server with the quicktart realm configured:

```
cd docker-dev
docker compose up
```

You can manage the keycloak instance at `http://localhost:8080` with user and pass "admin".

This will keep the compose running in the terminal, if you like to send it
to the background use the -d argument `docker compose up -d`.

Start react app, in other terminal execute:

```
npm run dev
```

Go to the browser at the address shown in the command output, usually: `http://localhost:4200/`

## Credentials

Login with user & password "alice"
