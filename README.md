# MEMEFI BOT 


- Multi account support.
- Auto tap tap `AUTO ON`.
- Auto Use Free Daily Booster Energy.
- Auto Use Free Daily Turbo Booster.
- Semi Auto Complete Daily Combo.
- Crazy Damage / God Mode (adearmanwijaya).



   cd memefi-bot
   ```

Create a virtual environment (optional but recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```
Install the dependencies:

```bash
pip install -r requirements.txt
```

## Configuration
Create or edit `config.json` :

This file should be located in the root directory of the project. Here is a sample configuration:

```json
{
    "energy_booster": false,
    "turbo_booster": false,
    "auto_claim_combo": false,
    "crazy_damage": false,
    "attempt_hit_boss": 6,
    "min_damage": 2000000,
    "max_damage": 50000000,

    "ACCOUNT_DELAY": 5,
    "LOOP_COUNTDOWN": 800
}


```

Create or edit `proxy.txt` :
List your proxies in the following format:

```ruby
username:password@host:port
```

Create or edit `combo.txt` :
input combo numbers in combo.txt using the format as below, separated by commas ( , ) and without spaces.

```bash
3,4,1,2
```

## Usage
before starting the bot you must have your own initdata / queryid telegram! why query id? with query_id it is definitely more profitable because you don't have to bother changing your init data every time.

1. Use PC/Laptop or Use USB Debugging Phone
2. open the `memefi bot miniapp`
3. Inspect Element `(F12)` on the keyboard
4. at the top of the choose "`Application`" 
5. then select "`Session Storage`" 
6. Select the links "`memefi`" and "`tgWebAppData`"
7. Take the value part of "`tgWebAppData`"
8. take the part that looks like this: 

```txt 
query_id=xxxxxxxxx-Rxxxxuj&user=%7B%22id%22%3A1323733375%2C%22first_name%22%3A%22xxxx%22%2C%22last_name%22%3A%22%E7%9A%BF%20xxxxxx%22%2C%22username%22%3A%22xxxxx%22%2C%22language_code%22%3A%22id%22%2C%22allows_write_to_pm%22%3Atrue%7D&auth_date=xxxxx&hash=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```
9. add it to `query_id.txt` file or create it if you dont have one


You can add more and run the accounts in turn by entering a query id in new line like this:
```txt
query_id=xxxxxxxxx-Rxxxxuj&user=%7B%22id%22%3A1323733375%2C%22first_name%22%3A%22xxxx%22%2C%22last_name%22%3A%22%E7%9A%BF%20xxxxxx%22%2C%22username%22%3A%22xxxxx%22%2C%22language_code%22%3A%22id%22%2C%22allows_write_to_pm%22%3Atrue%7D&auth_date=xxxxx&hash=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
query_id=xxxxxxxxx-Rxxxxuj&user=%7B%22id%22%3A1323733375%2C%22first_name%22%3A%22xxxx%22%2C%22last_name%22%3A%22%E7%9A%BF%20xxxxxx%22%2C%22username%22%3A%22xxxxx%22%2C%22language_code%22%3A%22id%22%2C%22allows_write_to_pm%22%3Atrue%7D&auth_date=xxxxx&hash=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

after that run the kombat hamster bot by writing the command:

```bash
python main.py
```

## License
This project is licensed under the `MIT License` - see the LICENSE file for details.

