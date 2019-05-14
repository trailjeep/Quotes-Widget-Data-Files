# Quotes-Widget-Data-Files
Some data files in JSON format for [Quotes Widget](https://play.google.com/store/apps/details?id=com.ashwin.apps.android.quoteswidget)

Contributions ~~welcome~~ needed.

Go [here](https://trailjeep.github.io/Quotes-Widget-Data-Files/) to download the individual files to your device (GitHub does not allow direct download links.)

Note-to-self:
convert to UNIX Fortune files
```bash
$ jq -r '.quotes[] | "\(.quote)\n\t--\(.author)\n%"' criminal-minds.json | head -n -1 > ~/.local/share/fortune/criminal-minds
$ strfile -c % ~/.local/share/fortune/criminal-minds ~/.local/share/fortune/criminal-minds.dat
```
