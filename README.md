node
typescript
gRPC


protocol buffers
server -> gRPC -> client


setup
$ yarn init -y
$ yarn add typescript -D
$ yarn run tsc --init
$ yarn add grpc
$ yarn add ts-node
$ yarn add ts-node grpc-tools @types/google-protobuf grpc_tools_node_protoc_ts -D


reference:

Coding with Justin - Implementing a gRPC client and server in Typescript with Node
https://www.youtube.com/watch?v=H0c4Wjl4kRQ&t=31s

------
# commitlint

commitlint io
https://commitlint.io/
------
https://commitlint.js.org/#/
https://commitlint.js.org/#/guides-local-setup
------
# install commitlint cli
npm install -g @commitlint/cli @commitlint/config-conventional
# install on project
npm install --save-dev @commitlint/{cli,config-conventional}
# create file
echo "module.exports = {extends: ['@commitlint/config-conventional']}" > commitlint.config.js
------
# install rusky-git hook helper
npm install husky --save-dev
# active hooks
yarn husky install
# add hook
yarn husky add .husky/commit-msg 'yarn commitlint --edit $1'