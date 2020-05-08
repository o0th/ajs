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
