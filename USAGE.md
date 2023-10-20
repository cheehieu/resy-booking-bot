# Init
- Install Scala-sbt: `brew install sbt`
- Follow the [Getting Started](https://github.com/Alkaar/resy-booking-bot/wiki/Getting-Started) wiki

# Config
- Set params in `./src/main/resources/resyConfig.conf`
  - `apiKey`: 
  - `auth_token`:
  - `date`:
  - `partySize`:
  - `venueId`:
  - `resTimeTypes`:
  - `hour`:
  - `minute`:
  - ``:
- Remember to adjust for timezone differences (bot runs based on local time of machine)
- Add User-Agent to POST request as described in https://github.com/Alkaar/resy-booking-bot/issues/133

# Run the Bot
- From the root directory, run the bot using CLI

```
$ sbt
$ run
```

# Functional Status
- 2023.10.20: Broken. Tried running a test with a venue with open reservations, but bot returned 502 Bad Gateway and "Could not find any available reservations"

