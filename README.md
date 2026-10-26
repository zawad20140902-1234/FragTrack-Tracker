# FragTrack

FragTrack is a Windows desktop app for viewing public Steam profile and Counter-Strike 2 data.

## Setup

1. Create your own Steam Web API key at [steamcommunity.com/dev/apikey](https://steamcommunity.com/dev/apikey). Accept Valve's terms and enter `localhost` as the domain.
2. Open FragTrack, choose **API KEY**, and enter your key. Keep it private. Each user needs their own key; do not post it in this repository or share it publicly.
3. In Steam, open **Profile → Edit Profile → Privacy Settings → Game details** and set **Game details** to **Public**. If playtime is hidden, turn off **Always keep my total playtime private even if users can see my game details**.
4. Extract the downloaded ZIP, run `FragTrack.exe`, add a SteamID64 or public profile URL, then select **SYNC PLAYERS**.

## What the data means

- Steam playtime is shown in hours in the Steam Players section.
- CS2 stats are available only when Steam returns them for that profile. Lifetime K/D is calculated from the available kills and deaths.
- Steam's public API does not provide Premier rating, competitive rank, match history, or ADR. Stats may be missing or out of date depending on Steam and the profile's privacy settings.

## Requirements

Windows 10 or 11, .NET Framework 4.8 or later, and an internet connection.

## Security and attribution

FragTrack stores the API key encrypted for the current Windows account in local settings. Never include your API key in screenshots, uploads, or shared files. FragTrack is an independent community app and is not affiliated with or endorsed by Valve or Steam. See [Steam Web API terms](https://steamcommunity.com/dev/apiterms).
