**Currently still in alpha.** [![Build Status](https://travis-ci.org/moraxy/libpurple-feed.svg?branch=travis_test)](https://travis-ci.org/moraxy/libpurple-feed)

# Building (preliminary)
    $ sudo apt-get install build-essential make libpurple-dev libmrss0-dev
    $ sudo apt-get build-dep libpurple0
    download/clone the newest libpurple-feed version
    $ cd libpurple-feed
    $ sudo make
    $ sudo make install

# Configuration
 * Restart your client if you haven't already done so, ideally in debug mode (e.g. `pidgin --debug`)
 * "Accounts" > "Manage Accounts" > "New"
 * Select the PurpleFeed protocol
 * Enter an account name
 * Set any additional options in the "Advanced" and "Proxy" tabs
 * Save the account

# Usage
 * "Accounts" > "Enable Account" > Enable your account
 * Set your status to "Available"
 * "Buddies" > "Add Buddy..."
 * Select a PurpleFeed account for the new buddy
 * `Username` is the feed's URL
 * Enter an `Alias` if you want to
 * Choose a `Group` or create a new one (Note: Groups will allow you to bundle different feeds together)
 * Save buddy and you're done
 * **Note:** There's currently no automated fetch & display method, you have to force it, so...
 * If the buddy's status is shown as available, open the context menu (right-click on the buddy) and choose "Feed URL Test" to force a feed update

# TODO / Known bugs
See Issues

# Future
 * Some sort of caching?
 * Templates?
 * Maybe port libmrss to libpurple's libxml2?
 * Some custom UI dialogs?
 * Proper Buddy struct?
