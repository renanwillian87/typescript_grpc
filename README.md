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