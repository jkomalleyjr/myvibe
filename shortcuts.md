# iPhone Shortcuts Integration

## Capabilities
- **Web APIs**: Use *Get Contents of URL* for GET/POST requests to any endpoint (fully capable HTTP client)  
- **App Shortcuts**: Integrate app intents into Siri, Spotlight, Shortcuts via Apple Developer docs  
- **Automation**: Automate API calls with custom URLs or httpbot.io  

## Example: Ping Repo from iPhone
1. Create shortcut → *Get Contents of URL*  
2. URL: `https://api.github.com/repos/myvibe` (or custom endpoint)  
3. Method: GET  
4. Parse response → log via *Show Result* or update `status.txt` via Working Copy  

## Use with This Repo
- Trigger via Working Copy → update `status.txt`  
- Run via Bonsai on OMEN → test vibe coding flow  

## Siri Example
- **Siri command**: “Run vibe test”  
- **App Intent**: Define intent in your app (e.g., `VibeTestIntent`)  
- **Shortcuts**: Add intent → *Get Contents of URL* → update `status.txt` via Working Copy  
- **Result**: Siri triggers shortcut → updates repo → Bonsai runs on OMEN  

## Media Workflow Example
- **Siri command**: “Run media workflow”  
- **App Intent**: Define intent (e.g., `MediaWorkflowIntent`)  
- **Shortcuts**: Add intent → *Get Contents of URL* → update `status.txt` via Working Copy  
- **Result**: Siri triggers shortcut → updates repo → Bonsai on OMEN runs local workflow (e.g., generate media)

## Multi-Machine Automation
- **Siri command**: “Run on <machine>”  
- **App Intent**: Define intent (e.g., `MultiMachineIntent`)  
- **Shortcuts**: Add intent → *Get Contents of URL* → update `status.txt` via Working Copy  
- **Result**: Siri triggers shortcut → updates repo → Bonsai runs on any networked machine (e.g., OMEN or others) via config update