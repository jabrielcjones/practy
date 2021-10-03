# Running JavaScript

## MacOS

1. Create Working Directory
```bash
mkdir practice/javascript

cd practice/javascript
```

1. Run `test.js`
```bash
echo "console.log('Test Successful!')\nalert('Test Successful!')" > test.js

echo '<head><script src="test.js" charset="utf-8"></script></head><body></body>' > index.html

open -a "Google Chrome" index.html
```

1. Open `Developer Tools` - OPTION + COMMAND + J
