# taskchampion-fly

Get [taskchampion-sync-server](https://gothenburgbitfactory.org/taskchampion-sync-server/introduction.html)
running on [Fly.io](https://fly.io/) for dirt cheap (or free).

## getting started

1. Provision and start the server: `make launch`
2. Generate the random client ID you will use with all your clients: `uuidgen`
3. Save this client ID in your password manager (i.e. [Bitwarden](https://bitwarden.com/)).
4. Tell your server what client ID to allow: `make client-id`
5. Visit [the sync docs](https://taskwarrior.org/docs/man/task-sync.5/#configuration) to
   learn how to setup your taskwarrior clients.

## custom domain (optional)

You are certainly welcome to use your default `app-name.fly.dev` if you want, however
if you want your app to run behind your own custom domain, you can check out [Fly's
official docs on how to do that](https://fly.io/docs/networking/custom-domain/).
