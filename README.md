# Clash Configuration Workspace

This repository manages custom Clash configuration templates and rules, optimized for subconverter usage.

## Files

- `HayGorNoClash.ini`: The primary active template for subconverter. All custom rules and proxy group adjustments are performed here.
- `ACL4SSR_Online_Full_NoAuto.ini`: A reference template based on the ACL4SSR configuration. **Do not modify this file.**
- `HayGorNoClash`: Binary or related tool (if applicable).

## Recent Optimizations

- **Rule Consolidation**: Merged Microsoft (Bing, OneDrive) and Google (FCM, Services) rules into unified groups.
- **Emoji Alignment**: Ensured all major strategy groups use consistent emoji prefixes (e.g., `🌏 Google`, `Ⓜ️ 微软服务`).
- **Rule Ordering**: Optimized the sequence of rulesets to ensure specific service matches take precedence over general GFW or country-based rules.
- **Apple TV Support**: Added dedicated ruleset and strategy group for Apple TV using dler-io providers.
- **Cleanup**: Removed obsolete Bilibili rulesets and the unused `HayGorNoClash.yaml` file.

## Usage

Use `HayGorNoClash.ini` as the remote configuration URL in your subconverter client or web interface.
