# Requeriments

- Ensure nats-server is installed
- Install protoc if you want to be able to compile the protobuf protocols

# Usage

```
./build.sh usage:

--clone: clone projects
--proto: compile protocol and copy it everywhere
--link: link libraries to kernel
--nats: start nats-server
-b --build: run npm run build on each project
-i --install: run npm ci on each project 
-s --start: run npm run start on each project 
```

## Example

Build only archipelago-service, but start nats, archipelago-service and explorer-bff

```
./build.sh -b archipelago-service && ./build.sh --nats -s archipelago-service explorer-bff 
```

# Comms Repositories

- [Explorer BFF](https://github.com/decentraland/explorer-bff)
- [Archipelago Service](https://github.com/decentraland/archipelago-service)
- [Comms Transports](https://github.com/decentraland/comms3-transports)
- [Kernel (comms package)](https://github.com/decentraland/kernel/tree/main/packages/shared/comms)
