## ajs

<p>
  <a href="https://github.com/standard/standard">
    <img src="https://img.shields.io/badge/Version-0.0.1-green.svg?style=for-the-badge" alt="Version">
  </a>
  <a href="/License.md">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" alt="License">
  </a>
</p>

`ajs` is an opensource shell script that save/update secrets from AWS Secrets
Manager via `.json` files. It use [jq](https://github.com/stedolan/jq) for
json file manipulation and [aws cli](https://aws.amazon.com/cli/) for the AWS
comunication.

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

Is it possible to specify an aws profile

```bash
ajs --profile aws-profile --secret aws-secret-name --get
```

### Contribute

`ajs` is an opensource project that runs on donations. If you want to
contribute feel free to open an issue or a pull request. If you want to 
say thank you and/or support the active development add a :star: to the
project or donate a :coffee:

<a href="https://www.buymeacoffee.com/o0th">
  <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=o0th&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff">
</a>

