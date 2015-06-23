# Instructions

## Basic use

If you are running the script for the first time:

    # chmod +x /etc/adblock.sh
    # sh /etc/adblock.sh -f

There should be status updates in the output, but there should be *no* errors.

## Whitelists and blacklists

The script supports defining whitelisted urls. That is, urls that will be filtered out of the downloaded blocklists. To whitelist urls, place them (one per line) in */etc/white.list*.

Similarly, the script supports defining blacklisted urls - urls that will be added to the downloaded blocklists. To blacklist urls, place them (one per line) in */etc/black.list*.

NOTE: The whitelist support is pretty stupid, so don't expect smart filtering (e.g., domain extrapolation).

## Advanced use

The config section of the script has some variables that alter the behaviour of the script.

For example, if you change:

    ONLY_WIRELESS = "N"
    
to

    ONLY_WIRELESS = "Y"
    
Then only the wireless interface of the router will filter the blocklist.

See the config section of the script for more variables.