<a href="https://github.com/standard/standard">
  <img src="https://img.shields.io/badge/ajs-0.0.1-green.svg?style=for-the-badge" alt="Standard">
</a>
<a href="/License.md">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" alt="License">
</a>
<a href="https://www.buymeacoffee.com/o0th" target="_blank">
  <img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="28">
</a>

### Installation

```bash
curl -o ajs https://raw.githubusercontent.com/o0th/ajs/master/ajs
sudo install ajs /usr/local/bin
```

### Usage

Save secret from aws secretsmanager to a local json file (`aws-secret-name.json`)

```bash
ajs --secret aws-secret-name --get
```

Update secret in aws secretsmanager from a local json file (`aws-secret-name.json`)

```bash
ajs --secret aws-secret-name --put
```

Is it possible to specify aws profile

```bash
ajs --profile aws-profile --secret aws-secret-name --get
```
