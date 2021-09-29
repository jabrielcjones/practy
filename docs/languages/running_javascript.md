# Running JavaScript

## MacOS

### Create Working Directory

```bash
mkdir practice/javascript

cd practice/javascript
```

### Run `test.js`

```bash
echo "console.log('Test Successful!')\nalert('Test Successful!')" > test.js

echo '<head><script src="test.js" charset="utf-8"></script></head><body></body>' > index.html

open -a "Google Chrome" index.html
```

Open `Developer Tools` - OPTION + COMMAND + J
