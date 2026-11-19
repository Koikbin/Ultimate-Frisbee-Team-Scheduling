# Ultimate Frisbee Team Scheduling App

A mobile app (built with Expo / React Native) for scheduling players during an ultimate frisbee game, so that every player on the team gets equal playing time.

> **Status: early development.** The project is currently the Expo starter template. The scheduling features below are planned and not yet implemented.

## Planned features

- Manage the team roster (add / remove players)
- Select the 7 players on the field for each point
- Track how many points each player has played
- Suggest the next line-up so playing time stays balanced
- (Optional) Respect gender-ratio rules for mixed divisions

## Tech stack

| | |
|---|---|
| Framework | [Expo](https://expo.dev) SDK 52, [React Native](https://reactnative.dev) 0.76 |
| Language | TypeScript |
| Navigation | [Expo Router](https://docs.expo.dev/router/introduction) (file-based routing) |
| Testing | Jest (`jest-expo`) |
| Platforms | iOS, Android, Web |

## Getting started

Prerequisites: [Node.js](https://nodejs.org) (LTS) and npm. To run on a phone, install [Expo Go](https://expo.dev/go).

```bash
npm install
npx expo start
```

Then press `i` (iOS simulator), `a` (Android emulator), `w` (web), or scan the QR code with Expo Go.

### Available scripts

| Command | Description |
|---|---|
| `npm start` | Start the Expo dev server |
| `npm run android` | Start and open on Android |
| `npm run ios` | Start and open on iOS |
| `npm run web` | Start and open in the browser |
| `npm test` | Run Jest tests in watch mode |
| `npm run lint` | Run the Expo linter |

## Project structure

```
app/                  Screens and routes (Expo Router)
  (tabs)/             Bottom-tab screens
  _layout.tsx         Root layout (fonts, theme)
components/           Reusable UI components (+ tests in __tests__/)
constants/            Colors and other constants
hooks/                Custom React hooks (color scheme, theme)
assets/               Fonts and images
scripts/              Helper scripts
ultimate-frisbee/     Second copy of the app on Expo SDK 53 (to be merged or removed)
```

## Roadmap

- [ ] Replace the starter screens with a roster screen and a game screen
- [ ] Implement the playing-time balancing logic
- [ ] Save rosters and game history locally on the device
- [ ] Merge the two app folders into one
