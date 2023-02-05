# ngrok

ngrok exposes local networked services behind NATs and firewalls to the public internet over a secure tunnel. Share local websites, build/test webhook consumers and self-host personal services.

Official Docs: [ngrok docs](https://ngrok.com/docs/)

## Installation

ngrok can easily be installed via their website: [ngrok website](https://ngrok.com)

## Usage

Detailed help for each command is available with `ngrok help <command>`.

Open [localhost:4040](http://localhost:4040) for ngrok's web interface to inspect traffic.

### Connect to ngrok account

```shell
ngrok config add-authtoken TOKEN
```

### Start ngrok

```shell
ngrok http 8000
```

### Securing endpoint

```shell
ngrok http 8000 --basic-auth 'ngrok:issecure'
```

---

#tools #http #server