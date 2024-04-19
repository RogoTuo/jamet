# jamet
"jamet": "^3.0.0"
"main": "dist/index.cjs.js",
"module": "dist/index.esm.js"
"@babel/runtime": "^7.7.7"
const { getConfig } = require("rogo");

const options = {};

module.exports = [
  getConfig({ ...options, format: "esm" }),
  getConfig({ ...options, format: "cjs" }),
  getConfig({ ...options, format: "umd", minify: true, sourcemap: true }),
];
