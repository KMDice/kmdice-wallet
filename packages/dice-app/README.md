<h1 align="center">
  <br>
  Dice Application
  <br>
</h1>

## Follow this instruction to run dice app in your local:

### Prerequisites:

- Nodejs: v10.13.0 or newer

- Yarn: v1.9.4 or newer

- Npm: v6.3.0 or newer

### Install

1. Clone the repo via git:
   `git clone --depth 1 -b master git@github.com:KMDice/kmdice-wallet.git`

2. To setup the Komodo daemon, [download](https://github.com/KomodoPlatform/komodo/releases) unzip and copy it to `packages/dice-app/app/bin/linux`.

```
atomicdex/packages/dice-app/app
							├── bin
							│   ├── mac
							│   ├── linux
							│   └── win
							└── src
```

3. Install project dependencies

- Root project

```
$ cd atomicdex
$ yarn install
```

- komodo-rpc-lib project

```
$ cd packages/komodo-rpc-lib/
$ yarn install
$ yarn build
```

- barterdex-utilities project

```
$ cd packages/barterdex-utilities/
$ yarn install
```

- barterdex-rssm project

```
$ cd packages/barterdex-rssm/
$ yarn install
```

- dice-app project

```
$ cd packages/dice-app/
$ yarn install
```

### Running

- Export your kmdice pubkey

```
export PUBKEY=YOUR_KEY
```

- Run app via yarn

```
yarn dev
```

- If your install is successful, you will see the application looks like this
  ![screen shot 2019-01-29 at 20 31 31](https://user-images.githubusercontent.com/3245868/51911742-2ecaf480-2405-11e9-8f9e-19395fbe2360.png)

- Please wait a litte bit until komodod is ready in background and you can start betting
  ![screen shot 2019-01-29 at 20 37 10](https://user-images.githubusercontent.com/3245868/51911954-af89f080-2405-11e9-94f8-74d2f50ea10c.png)
