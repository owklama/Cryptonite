# Welcome Cryptonite Ecosystem

## Main Features
- [ ] NFT Market place
- [ ] DeFi Exchange
- [ ] DAO Governance

## Tech stack
`NextJS` , `Typescript` , `Tailwindcss` , `Solidity`

## Experimental practices
`React 18.0` , `Layout RFC` 

## Engine lock

`use yarn only` \
`node >=14.0.0` \
`yarn >=1.22.0` 

#  Frontend

## Create Next App

```bash
yarn create next-app frontend --typescript
```

## Install dependencies
```bash
yarn add ethers hardhat @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers web3modal @openzeppelin/contracts ipfs-http-client@50.1.2 axios
```

## Install dev dependencies
```bash
yarn add -D tailwindcss@latest postcss@latest autoprefixer@latest prettier
```
## Tailwind
```bash
npx tailwindcss init -p
```
### Replace `content` in `tailwind.config.js` to:
```javascript 
['./pages/**/*.{js,ts,jsx,tsx}',
'./components/**/*.{js,ts,jsx,tsx}',],
```

### Add to `styles/global.css`
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```
## Hardhat
```bash
npx hardhat
```

### Add to `hardhat.config.js`
```typescript
const projectId: string = process.env.NEXT_PUBLIC_PROJECT_ID;
const apiSecret: string = process.env.NEXT_PUBLIC_API_SECRET;
const privateKey: string = process.env.NEXT_PUBLIC_PRIVATE_KEY;
```

## Husky
```bash
npx husky install
```

Create pre-commit hook
```bash
npx husky add .husky/pre-commit "yarn lint"
```

Create pre-push hook
```bash
npx husky add .husky/pre-push "yarn build"
````


