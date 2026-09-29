<p align="center"><img src="assets/logo.svg" width="96" alt="FrameFit Engine"></p>

<h1 align="center">FrameFit Engine — Game Compatibility Database</h1>

<p align="center">Signed compatibility profiles for <b>FrameFit Engine</b>: dynamic aspect adaptation for PC games — without modifying the game.</p>

---

## What is this repository?

This is the **official, cryptographically signed database** the FrameFit Engine
app downloads to know how to treat each game. Today it lists the games the app
refuses to work on because an anti-cheat system protects them.

| Status | Meaning |
|---|---|
| 🔴 BLOCKED | Refused by design — anti-cheat protected or unsupported |

Every database update is **signed**, and the app accepts only a database signed
with the key below — a compromised mirror can never mark a protected title as
safe.

## Verify a database yourself

```sh
minisign -Vm profiles.json -P RWR5uhqueYAw51JlSn5oUQo23/835rCjl1baNRWIoDZ6VVC5bTNXgs78
```

## Rules

**Offline single-player games only.** Titles protected by anti-cheat systems
(EasyAntiCheat, BattlEye, Vanguard, Ricochet) are permanently blocked.

## From the same makers

[FastForward Engine](https://github.com/buildwiserevenue/Fast-Forward-Engine) —
game speed control for offline, single-player PC games, with its own signed
database.

## Distribution

- Database (this repo, served via GitHub Pages): `profiles.json` + `profiles.json.minisig`

## License

Database contents: [CC BY 4.0](LICENSE) — attribution "FrameFit Engine".
FrameFit Engine is a trademark of its project. Not affiliated with any
game publisher or platform.
