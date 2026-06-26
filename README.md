# Simple Node.js App

A minimal HTTP server built with Node.js core modules — no external dependencies.

## Requirements

- [Node.js](https://nodejs.org/) v14 or higher

## Setup

1. Download `app.js` and `package.json` into a folder.
2. Open a terminal in that folder.

No `npm install` is needed since this app has no dependencies.

## Running the App

```bash
node app.js
```

Or, using the npm script:

```bash
npm start
```

You should see:

```
Server running at http://localhost:3000
```

## Usage

Once running, open these in your browser or test with `curl`:

| Route     | Method | Description                  |
|-----------|--------|-------------------------------|
| `/`       | GET    | Returns a hello world message |
| `/health` | GET    | Returns server health status  |
| `/time`   | GET    | Returns the current server time |

Example:

```bash
curl http://localhost:3000/
# {"message":"Hello, world!"}

curl http://localhost:3000/time
# {"time":"2026-06-26T10:15:00.000Z"}
```

## Changing the Port

By default the server runs on port `3000`. To use a different port, set the `PORT` environment variable:

```bash
PORT=8080 node app.js
```

## Project Structure

```
.
├── app.js          # Main server file
├── package.json    # Project metadata and scripts
└── README.md       # This file
```

## License

MIT
