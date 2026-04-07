<p align="center">
	<a href="https://sista.ai">
		<img src="assets/sista-logo.png" alt="Sista AI" width="260" />
	</a>
</p>

<h1 align="center">Sista Desktop Companion</h1>

<p align="center">
	<strong>Give your AI employees hands on your computer.</strong><br/>
	The official desktop companion for the <a href="https://work.sista.ai">Sista AI Employee</a> platform.<br/>
	Lets your hired AI employees control your browser and computer, securely and locally.
</p>

<p align="center">
	<a href="https://sista.ai">sista.ai</a> ·
	<a href="https://work.sista.ai">work.sista.ai</a> ·
	<a href="https://github.com/sista-ai/ai-employee-download/releases/latest">Latest Release</a>
</p>

<p align="center">
	<img src="assets/desktop-companion.png" alt="Sista Desktop Companion" width="820" />
</p>

---

## What is Sista?

Sista is a platform where businesses **hire AI employees** the same way they hire humans. You browse a talent market, interview candidates, sign a contract, and manage your AI workforce in a Slack-like workspace. Each employee has skills, duties, memory, and tools, and lives in your company permanently.

Learn more at [sista.ai](https://sista.ai) · Start hiring at [work.sista.ai](https://work.sista.ai)

## What is the Desktop Companion?

The Sista platform runs in the cloud, but your AI employees often need to work **on your machine**: opening your browser with your logged-in sessions, filling forms, reading files, running terminal commands, controlling native apps.

The Desktop Companion is a small, native app that runs locally and gives your AI employees a secure bridge into your computer. It connects to the Sista cloud over an authenticated WebSocket and executes commands on your behalf, under your control.

- **Browser automation** — navigate, click, type, extract data from any web page using your real browser and logged-in accounts
- **Computer control** — take screenshots, move the mouse, type on the keyboard, manage files, run shell commands
- **Runs fully local** — the AI brain stays in the cloud, the hands stay on your machine
- **Human-in-the-loop** — every sensitive action can require your approval
- **Open by design** — installers built in public via GitHub Actions, checksummed, and published here

## Download

Grab the latest installer for your operating system:

| OS       | Installer                      | Link |
| -------- | ------------------------------ | ---- |
| macOS    | `Sista-Mac-Desktop.dmg`        | [Download](https://github.com/sista-ai/ai-employee-download/releases/latest/download/Sista-Mac-Desktop.dmg) |
| Windows  | `Sista-Windows-Desktop.msi`    | [Download](https://github.com/sista-ai/ai-employee-download/releases/latest/download/Sista-Windows-Desktop.msi) |
| Linux    | `Sista-Linux-Desktop.AppImage` | [Download](https://github.com/sista-ai/ai-employee-download/releases/latest/download/Sista-Linux-Desktop.AppImage) |

All releases: [github.com/sista-ai/ai-employee-download/releases](https://github.com/sista-ai/ai-employee-download/releases)

## Install & Connect

1. Download the installer for your OS from the table above
2. Install and launch **Sista Desktop Companion**
3. Click **Sign in with Sista** — your browser opens to [work.sista.ai](https://work.sista.ai), you approve, and the app connects automatically
4. Grant the required OS permissions (Screen Recording + Accessibility on macOS, equivalents on other OSes)
5. Head back to [work.sista.ai](https://work.sista.ai) — your AI employees now have hands

## Security

- **Local execution** — all actions run on your machine, in your user account, with your permissions
- **Authenticated** — connects over TLS WebSocket with a short-lived JWT from your Sista account
- **Path sandboxing** — file operations are restricted to your home directory
- **Destructive command blocking** — dangerous shell patterns (`rm -rf /`, `dd`, `mkfs`, `shutdown`, `sudo`, fork bombs, and more) are refused at the app level
- **Human approval gates** — configurable per action, per employee, per workflow

## About This Repository

This repository **only hosts the signed installer binaries** for the Sista Desktop Companion. There is no application source code here. The source lives in the private [sista-ai/ai-employee](https://github.com/sista-ai/ai-employee) monorepo and is built in public via GitHub Actions, with the installers uploaded as release assets to this repo.

The "Source code (zip/tar.gz)" assets that GitHub auto-attaches to every release contain only this README and the `assets/` folder — not the product source.

## Links

- Website — [sista.ai](https://sista.ai)
- Product — [work.sista.ai](https://work.sista.ai)
- Latest release — [releases/latest](https://github.com/sista-ai/ai-employee-download/releases/latest)

---

<p align="center">
	<sub>© Sista AI · Hire AI like you hire humans.</sub>
</p>
