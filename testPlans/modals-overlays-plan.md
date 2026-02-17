## Test Plan: Modal & Overlays Module

### Test Steps

#### Step 1: Navigate to Dialog
- Navigate to https://dashboard-automation.netlify.app
- Click on 'Modal & Overlays' in the left sidebar
- Click on 'Dialog'

### Expected Results
- Page loads successfully at `/pages/modal-overlays/dialog`
- Dialog test section is displayed with multiple button options for testing different dialog configurations

#### Step 2: Test Basic Dialog - With Component
- Click on "Open Dialog with component" button
- Verify a modal dialog appears on the screen

### Expected Results
- Modal dialog opens with overlay
- Dialog content is visible and readable
- Dialog can be closed (via close button or escape key)
- Page content behind dialog is not accessible while dialog is open

#### Step 3: Test Dialog - Without Backdrop
- Click on "Open Dialog without backdrop" button
- Verify dialog appears without background overlay

### Expected Results
- Dialog opens without dark/semi-transparent backdrop
- Dialog is still visible and interactive
- User can see page content behind the dialog

#### Step 4: Test Dialog - ESC Key Behavior
- Click on "Open Dialog without esc close" button
- Press the ESC key on keyboard
- Verify dialog does not close from ESC key

### Expected Results
- Dialog opens successfully
- ESC key does not close the dialog when disabled
- Must use close button to dismiss

#### Step 5: Test Dialog - Return Result
- Click on "Enter Name" button
- Enter a name in the dialog input field
- Submit or close the dialog
- Verify the name appears in the "Names:" list

### Expected Results
- Dialog accepts input
- Data from dialog is captured and displayed
- List updates with new entries

#### Step 6: Navigate to Additional Overlays
- Click on 'Popover' in the Modal & Overlays menu
- Click on 'Tooltip' in the Modal & Overlays menu
- Click on 'Toastr' in the Modal & Overlays menu

### Expected Results
- Each page loads successfully
- Popover component displays on hover/click
- Tooltip shows helpful text on hover
- Toastr notifications appear and disappear as expected

#### Step 7: Test Toastr Configuration
- At Toastr page, modify the toast position, type, and message
- Check "Hide on click" option
- Click "Show toast" button

### Expected Results
- Toast notification appears with configured settings
- Toast position matches selection
- Toast style/type matches selection
- Toast auto-hides after specified time or on click

### Accessibility Requirements
- Dialogs have proper focus management
- Modal backdrop is properly announced
- Close buttons are accessible
- Popover and Tooltip content is keyboard accessible
- Toast notifications are announced to screen readers

### Test Data
- Test names: John Doe, Alice Smith, Bob Johnson
- Toast messages: "Success!", "Warning!", "Error Message"
- Toast types: primary, success, warning, danger
