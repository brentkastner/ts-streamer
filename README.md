# TS-STREAMER (TeamSpeak 3 Streamer)

This project builds a command line tool that connects to a TeamSpeak 3 SDK server, changes into a specified channel, and begins streaming the audio to STDOUT (default) or an mp3 file.

## Usage example:
`./ts-streamer <server> <channel ID>`

`./ts-streamer localhost 2`

## Dependencies

- TeamSpeak 3 SDK version 3.0.3.2
- Lame SDK 3.99.5

## Build Instructions

### XCode
- Clone the repo and open the workspace file

### TeamSpeaK SDK
- Download and unpack the TS SDK
- Find the platform specific library for your machine in the `<teamspeaksdk>/bin` directory and copy it to a library search path such as /usr/local/lib

### Lame libraries
- Download lame
- Run `./configure` in the client SDK directory
- Run `make`
- Run `make install`

### TO-DO for Builds
- Write makefile instead of relying on XCode build
