# Nix Windows Demo

A lightweight Nix Flake demonstration project targeting `x86_64-linux`.

---

## Project Specifications

* **Architecture Target:** `x86_64-linux`
* **Nix Feature Requirement:** Nix Flakes (`nix-command flakes`)
* **Key Components:**
  * `flake.nix`: Defines the environment, unfree package permissions, and the default execution app.
  * `flake.lock`: Locks dependency versions (`nixos-unstable`).

---

## How to Use

### Prerequisites
Ensure Nix with flakes is enabled:
```bash
mkdir -p ~/.config/nix
echo "experimental-features = nix-command flakes" >> ~/.config/nix/nix.conf
