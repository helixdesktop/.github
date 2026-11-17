# Security policy

Helix is a desktop session. Its compositor sees every keystroke and every frame on screen, its lock screen and greeter guard your session, and it handles passwords for polkit and the keyring. Please report security problems privately, so a fix can ship before the problem is public.

## Reporting a vulnerability

**Please don't open a public issue for a security problem.**

Use GitHub's private vulnerability reporting instead: open the **Security** tab of the affected repository and choose **Report a vulnerability**.

- Desktop (compositor, shell, session, portals, greeter): https://github.com/helixdesktop/desktop/security/advisories/new
- Applications: https://github.com/helixdesktop/apps/security/advisories/new
- Website: https://github.com/helixdesktop/web/security/advisories/new

Only the maintainers can see the report. Please include:

- the Helix version, from the package (`dpkg -s helix-desktop`) or the commit;
- the distribution and GPU driver, if they matter;
- the steps to reproduce, and what an attacker gains (for example: who can trigger it, and what they can read, run or bypass).

## What to expect

Helix is a small project with volunteer maintainers. These are goals, not guarantees:

- an acknowledgement within **7 days**;
- an initial assessment, and a fix or plan, within **30 days**;
- a published GitHub security advisory once a fix has been released, crediting you unless you would rather not be named.

If you don't hear back within 7 days, add a comment to the private report.

## Supported versions

Only the **latest release** and the `main` branch get security fixes. There are no long-term support branches yet.

## Scope

In scope: the code in the helixdesktop repositories and the packages built from it, including the files they install. Those files include the PAM configuration, polkit rules, AppArmor profile, systemd units and greetd configuration.

Problems we especially want to hear about include:

- getting past the lock screen or the greeter without the password;
- a client reading another client's input, clipboard or screen contents without the user's consent (for example through a Wayland protocol, a portal or the screen-cast and remote-desktop interfaces);
- a way around the consent dialogs for portals, screen sharing or remote desktop;
- passwords leaking from the polkit, keyring or greeter dialogs (into logs, other clients or memory dumps);
- an extension escaping its sandbox;
- privilege escalation through anything the packages install.

Out of scope:

- vulnerabilities in GTK, GLib, systemd, PipeWire, Xwayland, greetd or other upstream projects. Please report those to the project concerned. Tell us too if Helix makes the problem worse or needs a workaround;
- attacks that need root, or that need the attacker to already run code as the logged-in user. Exceptions: getting past the lock screen, and an extension escaping its sandbox, are in scope;
- the X11 security model: X11 applications on Xwayland can see each other's input and windows, as on any X server.

Thank you for helping keep Helix users safe.
