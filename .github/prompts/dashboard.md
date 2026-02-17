
mode: agent
description: 'Manually test a site & create a report'
tools:['browser_navigate',
  'browser_navigate_back',
  'browser_navigate_forward',
  'browser_click',
  'browser_type',
  'browser_select_option',
  'browser_drag',
  'browser_hover',
  'browser_press_key',
  'browser_file_upload',
  'browser_handle_dialog',
  'browser_snapshot',
  'browser_wait_for',
  'browser_network_requests',
  'browser_console_messages',
  'browser_take_screenshot',
  'browser_pdf_save',
  'browser_generate_playwright_test',
  'browser_screen_capture',
  'browser_screen_click',
  'browser_screen_drag',
  'browser_screen_type',
  'browser_screen_move_mouse',
  'browser_tab_list',
  'browser_tab_new',
  'browser_tab_select',
  'browser_tab_close',
  'browser_resize',
  'browser_close',
  'browser_install']


# Manual Testing Instructions
1. Use the Playwright MCP server to manually test the user provided scenario, if no scenario is provided ask the user to provide one.
2. Navigate to the url provided & preform the interactions.If no url is provided, ask the user to provide one.
3. Observe and verify the expected behaviour, focusing on accessibility, UI structure and User Experience.
4. Report back in clear, natural language: 
    - What steps you performed (navigation, interactions, assertions).
    - What are your observations (outcomes, UI changes, accessibility results).
    - Any issues, unexpected behaviours found,
5. Reference URLs, element roles, and relevant details to support your findings.



Example report format:
- **Scenario:** [Brief description]
- **Steps Taken:** [List of actions performed]
- **Outcome:** [What happened, including any assertions or accessibility checks]
- **Issues Found:** [List any problems or unexpected results]

Generate a .md file with the report in the 'test-results' directory and include any relevant screenshots or snapshots.

Take screenshots or snapshots of the page if necessary to illustrate issues or confirm expected behaviour. save them in the 'test-results' directory

close the browser after completing the manual test.
