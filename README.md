# css-modules
To test this environment:
1. Clone https://github.com/SAP/ui5-webcomponents
2. Run `yarn`
3. Run `yarn ci:releasebuild` command
4. Run `npm link` command respectively in main and fiori packages

## Test Create React App
1. Open `react-js` folder
2. Run `npm i` command
3. Run `npm link @ui5/webcomponents @ui5/webcomponents-fiori` command
4. Run `npm start`

## Test Svelte App
1. Open `svelte` folder
2. Run `npm i` command
3. Run `npm link @ui5/webcomponents @ui5/webcomponents-fiori` command
4. Run `npm run dev -- --open`
