# SwiftReposRN

Completed implementation of Lab 05 Swift Repos using Expo and TypeScript.

## Run

1. Install Node.js LTS.
2. Open a terminal in this folder and run `npm ci`.
3. Run `npm start` and open the app in a compatible Expo Go installation or Android emulator. An iOS simulator requires macOS.

## Check

- `npm test -- --runInBand` runs the five required filtering tests.
- `npm run typecheck` checks TypeScript.

## Features

- Fetches the first page of Swift repositories from GitHub, ordered by stars.
- Displays names, optional descriptions and formatted star counts.
- Filters the downloaded list by repository name without case sensitivity.
- Opens a tapped repository inside a WebView with the repository name in the header.
- Shows a loading indicator while fetching.

The project follows the required lab implementation, including returning an empty list on a network error. GitHub may rate-limit unauthenticated requests. Search filters the downloaded results; it does not search all of GitHub. Optional extensions are not included.

## Manual device check

Launch the app with internet access, wait for the list, search for a visible repository, clear the search, then tap a row. Confirm the GitHub page and header title appear and the back button returns to the list.

## Reference

Expo SDK reference: https://docs.expo.dev/versions/v56.0.0/

## Verification completed

- All five required Jest tests passed.
- TypeScript strict checking passed.
- Expo Android JavaScript bundle export completed successfully.
- Live interaction on a phone or emulator has not been verified.

The dependency installer reported 54 dependency advisories (7 moderate and 47 high). The versions remain aligned with Expo SDK 56; review dependency advisories before using this lab project in production.
