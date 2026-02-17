# Playwright MCP - Manual Testing Framework

A Model Context Protocol (MCP) based manual testing framework that enables AI-assisted browser automation and testing using Playwright. This framework allows you to create test plans and execute manual testing scenarios with screenshots, and detailed reporting.

## Overview

Playwright MCP provides a comprehensive set of browser interaction tools that can be used for:
- **Manual Testing** - Execute test scenarios and document results
- **Cross-browser Testing** - Test interactions across different browsers
- **Test Documentation** - Generate detailed reports with screenshots
- **Accessibility Testing** - Verify UI accessibility and semantic structure


## Quick Start

### 1. Create a Test Plan
Create a markdown file in the `testPlans/` directory with your test scenario:
```markdown
## Test Plan

### Test Steps
1. Navigate to the URL
2. Perform interactions
3. Verify expected behavior
```

### 2. Store the URL
Add your test URL to `url.txt`:
```
https://your-website.com
```

### 3. Execute the Test
Follow the instructions in `.github/prompts/dashboard.md` to run manual tests.

### 4. Review Results
Test reports are generated in the `test-results/` directory with:
- Step-by-step test execution details
- Screenshots and snapshots
- Accessibility findings
- Issue documentation

## Setup & Installation

### Install Playwright MCP Extension in VS Code

1. **Open VS Code Extensions**
   - Press `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac)
   - Or go to View → Extensions

2. **Search for Playwright MCP**
   - Type `@mcp playwright` in the search box
   - Click the extension from the search results

3. **Install the Extension**
   - Click the "Install" button
   - Wait for the installation to complete
   - The extension will be activated automatically

### Start the MCP Server

Before running tests in Copilot, you **must** start the MCP server:

1. **Open VS Code Extensions**
   - Press `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac)
   - Or go to View → Extensions

2. **Find Playwright in Installed Extensions**
   - Scroll to find "MCP SERVERS - INSTALLED" section
   - Locate "Playwright" in the list

3. **Click the Settings Icon**
   - Click the settings icon next to the Playwright extension
   - A context menu will appear with options

4. **Select "Start Server"**
   - Click "Start Server" from the dropdown menu
   - The server will initialize and start running

5. **Verify Server is Running**
   - Look for confirmation message in the Playwright output panel
   - You should see status indicating the server is running
  

6. **Keep Server Running**
   - Leave the server running while executing tests
   - The server remains active until you stop it or close VS Code
   - To stop: Click the settings icon again and select "Stop Server"

### Important Notes

⚠️ **Server Must Be Running** - The MCP server must be started before you ask Copilot to run tests. Without a running server, browser automation will fail.

⚠️ **Permissions** - When first running, the extension may prompt for permissions to execute browser automation. Grant these permissions to proceed.

💡 **Troubleshooting** - If tests fail, verify:
- The MCP server is running (check status in command palette)
- Playwright binaries are installed (`browser_install` will download them if needed)
- Your test URL is valid and accessible

## Test Plan Structure

Create test plans in `testPlans/` following this format:

```markdown
## Test Plan: [Feature Name]

### Test Steps

#### Step 1: [Action Description]
- [Sub-action 1]
- [Sub-action 2]

#### Step 2: [Next Action]
- [Expected outcome]

### Expected Results
- [Expected behavior 1]
- [Expected behavior 2]
```

## Test Report Format

Automated reports include:

- **Scenario**: Test description
- **Steps Taken**: Actions performed in order
- **Outcome**: Results and observations
- **Issues Found**: Any problems or unexpected behaviors
- **Screenshots**: Visual artifacts captured during testing

## Directory Structure

```
Playwright-MCP/
├── readme.md                 # This file
├── url.txt                   # Test URL
├── testPlans/               # Test plan markdown files
├── test-results/            # Generated test reports
├── .github/prompts/
│   └── dashboard.md         # Testing instructions
└── .playwright-mcp/         # Screenshots and artifacts
```

## Running Tests

1. Add your test URL to `url.txt`
2. Create a test plan in `testPlans/` folder
3. Execute the test by following the dashboard instructions
4. Review the generated report in `test-results/`

## Tips for Effective Testing

✅ **Accessibility Verification** - Use `browser_snapshot` to verify semantic structure and accessibility attributes

✅ **Screenshot Documentation** - Capture full-page screenshots for visual verification of expected UI

✅ **Error Monitoring** - Use `browser_console_messages` to check for JavaScript errors

✅ **Network Validation** - Use `browser_network_requests` to verify proper API calls

✅ **User Flow Testing** - Test complete workflows from navigation to form submission

## Example Test Execution

See `test-results/dashboard-test-report.md` for an example of a completed manual test with:
- Navigation through menu systems
- Theme/option selection
- Form interaction verification
- Accessibility validation
- Full-page screenshots
