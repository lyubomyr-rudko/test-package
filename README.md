How to publish to npm

npm init -y
npm install -g typescript -D
-D - for dev dependencies
npx tsc --init --rootDir src --outDir lib --declaration --sourceMapn --declarationMap
update package.json
"main": "lib",
"types": "lib",

"scripts": {
"build": "tsc",
"watch": "tsc -w",
},

npm install --scope=lyubomyr.rudko // must match exactly user name, creates scoped package

how to publish to npm?

1. register on npmjs.com
2. npm login
3. confirm email
4. npm publish (npm publish --access=public)
5. npm version patch
