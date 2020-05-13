# Itch.io Button Shortcode
[![Mirroring](https://github.com/OmiyaGames/itchio-button/workflows/Mirroring/badge.svg)](https://bitbucket.org/OmiyaGames/itchio-button) [![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/I3I51KS8F)

Adds a shortcode that generates a button allow the user to purchase a game on [Itch.io](https://itch.io).

# Usage
Create a download button for the game, [*Air Flip Drive* by Omiya Games](https://omiyagames.itch.io/airflipdrive).
```
[itchio-button game="airflipdrive" user="omiyagames"]
```

Create a buy button for the game, [*Air Flip Drive* by Omiya Games](https://omiyagames.itch.io/airflipdrive).
```
[itchio-button game="airflipdrive" user="omiyagames" text="Buy Now"]
```

Create a download button for the game, [*Air Flip Drive* by Omiya Games](https://omiyagames.itch.io/airflipdrive), that's 1280 pixels wide, and 720 pixels tall.
```
[itchio-button game="airflipdrive" user="omiyagames" width="1280" height="720"]
```

# Options
The following options are supported:

## `game`
(string) (required) The name (slug) of the game.  For example, if the URL of the game is "[`https://omiyagames.itch.io/airflipdrive`](https://omiyagames.itch.io/airflipdrive)," then fill this field with the string that comes after "`itch.io/`," i.e. "`airflipdrive`."

## `user`
(string) (required) The username (slug) of who the game belongs to.  For example, if the URL of the game is "[`https://omiyagames.itch.io/airflipdrive`](https://omiyagames.itch.io/airflipdrive)," then fill this field with the string that comes in between "`https://`" and "`.itch.io/`," i.e. "`omiyagames`."

## `text`
(string) (optional) The text that'll appear on the button.

Default: "Download"

## `width`
(integer) (optional) The width of the pop-up that appears after clicking the download button, in pixels.

Default: 650

## `height`
(integer) (optional) The height of the pop-up that appears after clicking the download button, in pixels.

Default: 400

# Known Issues

- Only one button can be created per webpage (so be careful about adding this to a widget).  The shortcode does not create a unique ID for each button.

# References

- [`Itch.attachBuyButton()`](https://itch.io/docs/api/javascript#reference/itchattachbuybuttonelement-options)
