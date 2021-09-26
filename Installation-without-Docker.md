## Installation without Docker

### Requirements
- [Node.js](https://nodejs.org/en/)
- npm (installed with Node)
- git

### Instructions

#### Downloading source code

```bash
# clone repository
git clone https://github.com/pawelmalak/snippet-box
cd snippet-box

# install dependencies
npm run init
```

#### Building server & client code
```bash
# server
npm run build

# client
npm run build --prefix=client
```

#### Preparing app directory
```bash
mkdir public data
mv client/build/* public
```

#### Cleanup
```bash
rm -rf src client
npm prune --production
```

#### Run
```bash
PORT=5000 NODE_ENV=production node build/server.js
```

Expected initial output:
```bash
[2021-09-27 01:35:07.108 UTC+2] [INFO] db: Database connected
[2021-09-27 01:35:07.322 UTC+2] [INFO] db: Found pending migrations. Executing...
[2021-09-27 01:35:07.836 UTC+2] [INFO] server: Server is working on port 5000 in production mode
```

Snippet Box should be now running at `localhost:5000`