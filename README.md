## timezone-selector

Nice little command-line UI for selecting timezones in Unix systems. It can detect your timezone, ask you if it's correct and let you set it up manually if you want. 

![](https://cldup.com/UohFGbGI34.png)
![](https://cldup.com/-Ud-Q7SNs5.png)

## usage

```bash
source timezone-selector.sh
tzSelectionMenu "Optional background title"
```

It'll set the result to $selected;

```bash
echo "$selected"
# > /usr/share/zoneinfo/Chile/Continental
```

And you can set the timezone by:

```bash
ln -s $selected /etc/localtime
```
