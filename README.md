# How to run the frontend

## The simple way

```bash
python3 frontend.py [BACKEND PORT]
```

For example:

```bash
python3 frontend.py 5000
```

The backend port is just an integer that is the port the flask server is CURRENTLY running on.

## The complex way

Only complete this step if you're comfortable self-teaching yourself ReactJS.

Run this once on the machine.
```bash
npm install
```

Start up your backend on a specific port.

Then run:
```bash
./run.sh [BACKEND PORT] [FRONTEND PORT]
```

For example:
```bash
./run.sh 5000 12345
```

## Iteration 3 onwards

Update line 4 in src/utils/constants.js to contain your deployed backend url. For example, for a url `https://example.alwaysdata.net`, line 4 should be:
```javascript
const deployedUrl = "https://example.alwaysdata.net";
```

To utilise this deployed backend, run:
```bash
./run.sh 0 [FRONTEND PORT]
```
