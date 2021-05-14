---
title: Sir-Lancebot Environment Variable Reference
description: The full environment variable reference for Sir-Lancebot.
toc: 2
---
## General Variables
The following variables are needed for running Sir Lancebot:

| Environment Variable | Description |
| -------- | -------- |
| `BOT_TOKEN` | Bot Token from the [Discord developer portal](https://discord.com/developers/applications) |
| `BOT_GUILD` | ID of the Discord Server |
| `BOT_ADMIN_ROLE_ID` | ID of the role @Admins |
| `ROLE_HELPERS` | ID of the role @Helpers |
| `CHANNEL_ANNOUNCEMENTS` | ID of the #announcements channel |
| `CHANNEL_DEVLOG` | ID of the #dev-log channel |
| `CHANNEL_COMMUNITY_BOT_COMMANDS` | ID of the #sir-lancebot-commands channel |

---
## Debug Variables
Additionally, you may find the following environment variables useful during development:

| Environment Variable | Description |
| -------- | -------- |
| `BOT_DEBUG` | Debug mode of the bot | False |
| `PREFIX` | The bot's invocation prefix | `.` |
| `CYCLE_FREQUENCY` | Amount of days between cycling server icon | 3 |
| `MONTH_OVERRIDE` | Interger in range `[0, 12]`, overrides current month w.r.t. seasonal decorators |
| `REDIS_HOST` | The address to connect to for the Redis database. |
| `REDIS_PORT` | |
| `REDIS_PASSWORD` | |
| `USE_FAKEREDIS` | If the FakeRedis module should be used. Set this to true if you don't have a Redis database setup. |
| `BOT_SENTRY_DSN` | The DSN of the sentry monitor. |
| `TRASHCAN_EMOJI` | The emoji to use for the trashcan during paginated embeds |


---
## Tokens/APIs
If you will be working with an external service, you might have to set one of these tokens:

| Token | Description |
| -------- | -------- |
| `GITHUB_TOKEN` | Personal access token for GitHub, raises rate limits from 60 to 5000 requests per hour. |
| `GIPHY_TOKEN` | Required for API access. [Docs](https://developers.giphy.com/docs/api) |
| `OMDB_API_KEY` | Required for API access. [Docs](http://www.omdbapi.com/) |
| `REDDIT_CLIENT_ID` | OAuth2 client ID for authenticating with the [reddit API](https://github.com/reddit-archive/reddit/wiki/OAuth2). |
| `REDDIT_SECRET` | OAuth2 secret for authenticating with the reddit API. *Leave empty if you're not using the reddit API.* |
| `REDDIT_WEBHOOK` | Webhook ID for Reddit channel |
| `YOUTUBE_API_KEY` | An OAuth Key or Token are required for API access. [Docs](https://developers.google.com/youtube/v3/docs#calling-the-api) |
| `TMDB_API_KEY` | Required for API access. [Docs](https://developers.themoviedb.org/3/getting-started/introduction) |
| `NASA_API_KEY` | Required for API access. [Docs](https://api.nasa.gov/) |
| `IGDB_API_KEY` | Required for API access. A Twitch account is needed. [Docs](https://api-docs.igdb.com/#about) |
| `WOLFRAM_API_KEY` | |
| `UNSPLASH_KEY` | Required for API access. Use the `access_token` given by Unsplash. [Docs](https://unsplash.com/documentation) |

---
## Seasonal Cogs
These variables might come in handy while working on certain cogs:

| Cog | Environment Variable | Description |
| -------- | -------- | -------- |
| Advent of Code | `AOC_LEADERBOARDS` | List of leaderboards seperated by `::`. Each entry should have an `id,session cookie,join code` seperated by commas in that order. |
| Advent of Code | `AOC_STAFF_LEADERBOARD_ID` | Integer ID of the staff leaderboard. |
| Advent of Code | `AOC_ROLE_ID` | ID of the advent of code role.
| Advent of Code | `AOC_IGNORED_DAYS` | Comma seperated list of days to ignore while calulating score. |
| Advent of Code | `AOC_YEAR` | Debug variable to change the year used for AoC. |
| Advent of Code | `AOC_CHANNEL_ID` | The ID of the #advent-of-code channel |
| Advent of Code | `AOC_FALLBACK_SESSION` | |
| Valentines | `LOVEFEST_ROLE_ID` | |
| Wolfram | `WOLFRAM_USER_LIMIT_DAY` | |
| Wolfram | `WOLFRAM_GUILD_LIMIT_DAY` | |