## Expo Doctor Exercise

Practice using Expo Doctror to find and resolve problems in your project.

## Setup

Clone this repo and install dependencies with either `yarn` or `npm install`.

## Run Expo Doctor

In your project directory, run `npx expo-doctor` to diagnose issues.

<details><summary>Solution</summary>
<p>

### ✖ Check dependencies for packages that should not be installed directly

> The package "expo-dev-menu" should not be installed directly in your project. It is a dependency of other Expo packages, which will install it automatically as needed.

Uninstall `expo-dev-menu`.

Run `npx expo-doctor` again to verify this error disappears.

### ✖ Check for common project setup issues

> This project has multiple package manager lock files (yarn.lock, package-lock.json). This may cause EAS build to restore dependencies with a different package manager from what you use in other environments.

Remove either the `package-lock.json` or the `yarn.lock` (depending on which package manager you chose).

Run `npx expo-doctor` again to verify this error disappears.

### ✖ Check Expo config (app.json/ app.config.js) schema

> Error: Problem validating fields in /Users/kadi/Code/fix-me-app/app.json. Learn more: https://docs.expo.dev/workflow/configuration/
> • should NOT have additional property 'appIcon'.

Remove the `appIcon` field from `app.json`.

Run `npx expo-doctor` again to verify this error disappears.

### ✖ Check that packages match versions required by installed Expo SDK

> Some dependencies are incompatible with the installed expo version:
>   expo-status-bar@1.5.0 - expected version: ~1.6.0
> Your project may not work correctly until you install the correct versions of the packages.

Run `npx expo install --fix` to update dependencies.

Run `npx expo-doctor` again to verify this error disappears.

</p>
</details>


