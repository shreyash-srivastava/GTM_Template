# Jio CMP Template for Google Tag Manager

This tag template integrates a Consent Management Platform (CMP) with
Google Tag Manager using Consent Mode v2.

## What it does

- Sets a safe default consent state (all types denied) via `setDefaultConsentState()`
- Loads the CMP's banner script onto the page via `injectScript()`
- The banner script itself calls `gtag('consent', 'update', ...)` when the
  user makes a choice, which this template does not handle directly

## Fields

| Field | Description |
|---|---|
| CMP Account ID | The unique account/site ID assigned when you register with our CMP |
| CMP Script URL | The URL of the CMP banner script to load (defaults to our hosted script) |

## Setup

1. Add a new tag using this template
2. Fill in your Account ID
3. Set the trigger to **Consent Initialization - All Pages**
4. Publish

## Support

Please open a GitHub Issue on this repository for bugs or questions.
