# System Setup / Bootstrapping

Instructions for bootstrapping and/or recovering my systems.
Primarily for personal use, but maybe instructive for others ;-).

## Overview

System configuration involves many steps: drive and partition layout and setup, encryption, boot loader config, account setup, preferred applications, custom configs (dotfiles) and so on.
My goal here is a concise overview of necessary steps, maybe with links/pointers to other crucial information.

For now this is all based on the setup of my primary work laptop running Arch Linux.
Once we ge to the point to cover the setup of multiple systems we differentiate things accordingly.
Until then a flat README should suffice.

## Instructions

This section contains some specific setup instructions.

### Dotfiles

- **Primary Resource:** [my dotfiles repo](https://github.com/landaro/dotfiles)
- **Tool:** [rcm](https://github.com/thoughtbot/rcm)

1. Ensure that `rcm` is installed.
2. Generate a keypair to access github.com and deposit public key:
   ```
   ssh-keygen -a 100 -t ed25519 -C "USER@HOST -> landaro@github.com" -f .ssh/github_id_ed25519
   ```
3. Continue with instructions from dotfiles repo.
