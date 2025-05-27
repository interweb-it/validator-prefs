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


## Example
```bash
./set-prefs -c polkadot -a 12WUg5s5hxBh9GZVVpqyZvbBravHhJSc548K9k1E2mjWP123 -m 1.5 
Connecting to polkadot with address 12WUg5s5hxBh9GZVVpqyZvbBravHhJSc548K9k1E2mjWP123 and commission 1.5
Enter seed: *************************************************************************


Secret captured (hidden).
Loaded account: 12WUg5s5hxBh9GZVVpqyZvbBravHhJSc548K9k1E2mjWP123
Sending transaction to set commission to 1.5%...
✅ Included in block: 0xbcae6e3338c5fcd37aaba9505faed2c638a5035e9b680407c85651e09ef7a1e1
🎉 Finalized in block: 0xbcae6e3338c5fcd37aaba9505faed2c638a5035e9b680407c85651e09ef7a1e1
```

# Dependencies
- `@polkadot/api`
- `commander`

