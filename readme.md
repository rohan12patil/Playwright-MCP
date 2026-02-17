# Playwright MCP
- MCP based manual testing

- Below is the list of MCP tools 
- 
  // Navigation
  "browser_navigate",
  "browser_navigate_back",
  "browser_navigate_forward",
  
  // Interaction
  "browser_click",
  "browser_type",
  "browser_select_option",
  "browser_drag",
  "browser_hover",
  "browser_press_key",
  "browser_file_upload",
  "browser_handle_dialog",
  
  // State & Observation
  "browser_snapshot",          // Gets accessibility tree snapshot
  "browser_wait_for",          // Waits for text or time
  "browser_network_requests",  // Lists network activity
  "browser_console_messages",  // Retrieves console logs
  
  // Artifacts & Testing
  "browser_take_screenshot",
  "browser_pdf_save",
  "browser_generate_playwright_test",
  
  // Vision Mode (Coordinate-based)
  "browser_screen_capture",
  "browser_screen_click",
  "browser_screen_drag",
  "browser_screen_type",
  "browser_screen_move_mouse",
  
  // Tab & Session Management
  "browser_tab_list",
  "browser_tab_new",
  "browser_tab_select",
  "browser_tab_close",
  "browser_resize",
  "browser_close",
  
  // Utilities
  "browser_install"            // Installs required browser binaries
