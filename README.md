# SiVote

**SiVote** is an open-source internet voting system designed to support **secret ballots** for private organizations. It consists of two main components:

- **SiVote Engine**: Handles ballot creation, voter interaction, unique voting code generation, and secure result collection.
  
- **SiVote Sender**: Manages voter lists and sends email invitations with ballot links.

The tool offers a CLI, and a GUI is available at [eGlasovanje.si](https://eglasovanje.si). This system is provided by the non-profit organization [IP21](https://ip21.si).

## Features

- **Secret Ballots**: Uses random codes to ensure anonymity.
- **Independently Verifiable**: Voters receive a vote dump to verify their vote and the results.
- **Easy to Understand**: No blockchain or complex tech, enabling transparency and trust.
- **Not Experimental**: Designed - support organisation and all - to be a dependable solution.
- **Complete Solution**: Create ballots, validate users, collect votes, and communicate results.
- **User-Friendly**: Voters cast ballots via a browser on any device using a simple email invitation.
- **Customizable Security**: Supports [different security levels](https://eglasovanje.si/nivoji-varnosti) to fit organizational needs.
- **Theming**: Add your logo to the top of ballots and results. Revolutionary, we know.

## How It Works

The system generates a list of codes (equal to the number of voters) and randomly sends them via email. After voting, voters receive a CSV dump of all votes to verify that their vote was recorded correctly and results were calculated accurately.

## Usage

1. Use [eGlasovanje.si](https://eglasovanje.si) or install it yourself.

## Installation

See the [Sender](https://github.com/Institut-IP21/SiVoteSender) and [Engine](https://github.com/Institut-IP21/SiVoteEngine) documentation for installation instructions.
