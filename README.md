# CMT Explorer 3.0

> Designed and developed from the ground-up, using lean & fast developmental frameworks (Tailwind CSS & Vue.JS).

## Build Setup

### 1. Clone the repository

```bash
git clone https://github.com/CMTEcosystem/CMT-explorer
```

### 2. Install Dependencies

```bash
yarn install
```

### 3. Build for Production

#### 3.1 Mainnet

```bash
yarn build:mainnet
```

#### 3.2 Devnet

```bash
yarn build:devnet
```

#### 3.3 Custom

```bash
yarn build --network my-custom-network
```

#### 3.4 GitHub Pages

If you are going to host your explorer instance on GitHub Pages you will need to specify your base url in most cases as GitHub Pages serves repositories from sub-directories instead of sub-domains.

```bash
yarn build --base https://username.github.io/repository/
```

A running instance of the explorer on GitHub Pages can be found at https://CMTecosystem.github.io/.

> This step is not required if you are hosting the explorer on your "root" repository which is usually your username https://username.github.io/.

#### 3.5 Run Express Server

You can run the explorer as an express server. This makes it a little more light-weight but not needing to have services such as apache or nginx.

```bash
EXPLORER_HOST="127.0.0.1" EXPLORER_PORT="4200" node express-server.js
```

## 4. History Mode

If you wish to remove the `/#/` from your URLs you can follow those steps https://router.vuejs.org/en/essentials/history-mode.html.

### 4.1 Build

```bash
yarn build:mainnet --history
```

### 4.2 Development

```bash
yarn dev --env.routerMode=history
```

> Keep in mind that this requires you to run your own server and a running instance of nginx.

## 5. Development

#### Mainnet

```bash
yarn dev # or yarn dev:mainnet
```

#### Devnet

```bash
yarn dev:devnet
```

#### Custom

```bash
yarn dev --env.network=custom
```

#### Change Router Mode

```bash
yarn dev --env.routerMode=history
```

## 6. Testing

``` bash
$ yarn test
```

## 7. Security

If you discover a security vulnerability within this package, please send an e-mail to security@CMT.io. All security vulnerabilities will be promptly addressed.

## 8. Credits

- Lorenzo Caruso <lorenzo.caruso@outlook.com>

## 9. License

[MIT](LICENSE) © [CMTEcosystem]
