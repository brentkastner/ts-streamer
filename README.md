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
- cd to the <teamspeak-sdk-dir>/examples/client directory
- Pick the makefile for your platform and `cp MAKEFILE.macosx MAKEFILE`
- Run `make`
- Copy the soundbackends directory into the project (mine was built on a mac YMMV)

### Lame libraries
- Download lame
- Run `./configure` in the client SDK directory
- Run `make`
- Run `make install`

### TO-DO for Builds
- Write makefile
