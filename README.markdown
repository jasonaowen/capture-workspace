# Capture Workspace

## What are you doing all day?

This is a simple script to take a screenshot and record the active application.

Set it to a cron job!

```crontab
*/5 * * * * DISPLAY=:0.0 ~/bin/capture-workspace
```

Setting the `DISPLAY` variable is necessary as the cron job is run in a
different environment.

## Dependencies

This depends on [scrot(1)](https://en.wikipedia.org/wiki/Scrot),
[jq(1)](https://stedolan.github.io/jq/), and
[xdotool(1)](http://semicomplete.com/projects/xdotool).

On Debian derivatives (like Ubuntu), they are in packages of the same names:

```sh
$ sudo apt install scrot jq xdotool
```

<a href='http://www.recurse.com' title='Made with love at the Recurse Center'><img src='https://cloud.githubusercontent.com/assets/2883345/11325206/336ea5f4-9150-11e5-9e90-d86ad31993d8.png' height='20px'/></a>
![Licensed under the GPL, version 3](https://img.shields.io/badge/license-GPL3-blue.svg)
