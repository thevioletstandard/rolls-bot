# rolls-bot
Rolls dice for you on Reddit.

## Installation
```
$ git clone https://github.com/thevioletstandard/rolls-bot.git
$ cd rolls-bot
$ pip3 install -r requirements.txt
$ nano praw.ini # enter your settings
$ python3 rolls-bot.py &
```
## Usage

There is currently a hosted instance of the bot with the Reddit account [/u/RollsBot](https://www.reddit.com/u/rollsbot). It is invoked by mentioning it in a comment or replying to it in a thread with a valid dice roll. Valid dice rolls can be surrounded by other text, and follow the format:

`[Number of dice rolled]d[Maximum number rolled][operator][operand]`

The operator and operand are optional, and the operator can be any one of +, -, \*, /, or %. The number of dice rolled, maximum number rolled, and operand must all be positive. Some valid examples of rolls are:

- `1d20` (rolls 1 20-sided die)
- `2d20` (rolls 2 20-sided dice)
- `1d20*5` (rolls 1 20-sided die, multiplies the result by 5)
- `2d20-5` (rolls 2 20-sided dice, adds the results, and subtracts 5)
