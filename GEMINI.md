# Workspace Instructions (GEMINI.md)

## Foundational Mandates

- **Template Management**: 
    - `HayGorNoClash.ini` is the **only** active template that should be modified for rule updates, strategy group changes, or reordering.
    - `ACL4SSR_Online_Full_NoAuto.ini` is a **Reference Only** file. It must remain in its original state to serve as a baseline.
- **Naming Conventions**: 
    - Strategy groups (`custom_proxy_group`) should follow the emoji-prefix convention (e.g., `🌏 Google`, `🍎 苹果服务`, `📲 电报消息`).
    - Use clear and consistent labels for new rulesets.
- **Rule Ordering Logic**: 
    - Maintain the hierarchical order: 
        1. Ad/Program Blocking
        2. Basic Direct (LAN/UnBan)
        3. Specific Proxied Services (Google, Telegram, AI)
        4. Media Services (YouTube, Netflix, Apple TV, etc.)
        5. Ecosystem Services (Microsoft, Apple)
        6. Games & Downloads
        7. General Proxy (GFW List)
        8. Domestic Direct (China Domains/IPs)
        9. Final Match (漏网之鱼)
- **Tool Usage**: 
    - When updating `.ini` files, ensure the `custom_proxy_group` format `Group`select`[]SubGroup1`[]SubGroup2` is strictly followed.
