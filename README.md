# VS Code Web Test

Repository for recreating the issue outlined at:

# Setup

## vscode.dev

Extension host used: UI
Status: WORKING

- Clone this repository
- Head to https://vscode.dev
- Install the recommended extension `arm-debug.mock-debug-test`
- Open the cloned folder in vscode.dev
- Start a debug session for 'Debug readme.md'
- Observe it working

## codespaces (remote)

Extension host used: REMOTE
Status: WORKING

- Create a codespace on this repository and open it
- Install the recommended extension `arm-debug.mock-debug-test` in the REMOTE extension host
- Start a debug session for 'Debug readme.md'
- Observe it working

## codespaces (local)

Extension host used: UI
Status: BROKEN

- Create a codespace on this repository and open it
- Install the recommended extension `arm-debug.mock-debug-test` in the LOCAL extension host
- Start a debug session for 'Debug readme.md'
- Observe the file sent from the debugger to the UI fails to open:

## github.dev

Extension host used: UI
Status: BROKEN

- Hit the `.` key or open https://github.dev/thegecko/vscode-web-test
- Install the recommended extension `arm-debug.mock-debug-test`
- Start a debug session for 'Debug readme.md'
- Observe the file sent from the debugger to the UI fails to open:

# Log information

Follow these steps to view the debug adapter protocol traffic and debug logging:

- Open the output pane
- Select the `Mock Debug` channel from the dropdown 

# Notes

- This demo uses a modified version of [Mock Debug]() in order to add logging and fix some file schemas. This can be found here:
https://github.com/thegecko/vscode-mock-debug/tree/mock-debug-test

- As it's not possible to sideload browser extensions in codespaces or github.dev, this extension has had to be published here:
https://marketplace.visualstudio.com/items?itemName=arm-debug.mock-debug-test
