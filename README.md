# Set validator preferences

## Setup

```bash
git clone https://github.com/interweb-it/validator-prefs
cd validator-prefs
yarn install 
chmod +x set-prefs
```

## Usage

```bash
./set-prefs -h                    
Usage: set-prefs [options]

Set validator preferences

Options:
  -V, --version              output the version number
  -c, --chain <chain>        Blockchain network to connect to (default: "kusama")
  -a, --address <address>    Validator address
  -m, --commission <number>  Commission percentage (default: 1.5)
  -h, --help                 Display help for command
```

# Dependencies
- `@polkadot/api`
- `commander`

