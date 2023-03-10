# VS Code Web Test

Repository for recreating the issue outlined at:

- https://github.com/orgs/community/discussions/44904
- https://github.com/microsoft/vscode-mock-debug/issues/89
- https://github.com/microsoft/vscode/issues/171991

# Test Extension Notes

- This demo uses a modified version of [Mock Debug](https://github.com/microsoft/vscode-mock-debug) in order to fix file schemas. Source for this can be found here:
https://github.com/thegecko/vscode-mock-debug/tree/mock-debug-test

- As it's not possible to sideload browser extensions in codespaces or github.dev, the test extension has had to be published here:
https://marketplace.visualstudio.com/items?itemName=arm-debug.mock-debug-test

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

<img width="1021" alt="Screenshot 2023-03-09 at 16 49 44" src="https://user-images.githubusercontent.com/61341/224095927-a771b807-f3aa-4051-8b49-f84674ba5334.png">

## codespaces (remote)

Extension host used: REMOTE

Status: WORKING

- Create a codespace on this repository and open it
- Install the recommended extension `arm-debug.mock-debug-test` in the REMOTE extension host
- Start a debug session for 'Debug readme.md'
- Observe it working

<img width="953" alt="Screenshot 2023-03-09 at 16 48 29" src="https://user-images.githubusercontent.com/61341/224095058-6bb2a5a9-939a-42a2-b448-31b8dd772975.png">

## codespaces (local)

Extension host used: UI

Status: BROKEN

- Create a codespace on this repository and open it
- Install the recommended extension `arm-debug.mock-debug-test` in the LOCAL extension host
- Start a debug session for 'Debug readme.md'
- Observe the file sent from the debugger to the UI fails to open:

<img width="628" alt="Screenshot 2023-03-09 at 16 47 23" src="https://user-images.githubusercontent.com/61341/224094414-e2dc78a2-4aaa-4cd1-8b89-e7b461a000eb.png">

## github.dev

Extension host used: UI

Status: BROKEN

- Hit the `.` key or open https://github.dev/thegecko/vscode-web-test
- Install the recommended extension `arm-debug.mock-debug-test`
- Start a debug session for 'Debug readme.md'
- Observe the file sent from the debugger to the UI fails to open:

<img width="839" alt="Screenshot 2023-03-09 at 16 45 18" src="https://user-images.githubusercontent.com/61341/224093257-93a3c2dd-e998-40e8-b387-ac55c931b872.png">
