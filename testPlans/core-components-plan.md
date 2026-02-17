## Test Plan: Core UI Components Module

### Test Steps

#### Step 1: Navigate to Extra Components
- Navigate to https://dashboard-automation.netlify.app
- Click on 'Extra Components' in the left sidebar
- Verify available options

### Expected Results
- Extra Components menu expands
- Calendar option is visible
- Other component options are displayed

#### Step 2: Test Calendar Component
- Click on 'Calendar' menu item
- Verify calendar page loads successfully

### Expected Results
- Page loads at `/pages/extra-components/calendar`
- Calendar component displays with current month/year
- Calendar shows all days of the month
- Day names are displayed (Mon, Tue, Wed, etc.)
- Navigation to previous/next months is available

#### Step 3: Test Calendar Navigation
- Click next month arrow (>)
- Verify calendar updates to show next month
- Click previous month arrow (<)
- Verify calendar shows previous month

### Expected Results
- Month/year updates correctly
- Calendar days correspond to correct month
- Navigation arrows work in both directions
- Current date may be highlighted

#### Step 4: Test Calendar Date Selection
- Click on a date in the calendar
- Verify the date is selectable and updates UI

### Expected Results
- Date can be clicked/selected
- Selected date is visually highlighted
- Date information is captured or displayed
- Calendar remains functional after selection

#### Step 5: Test IoT Dashboard - Devices
- Navigate back to IoT Dashboard
- Locate device cards (Light, Roller Shades, Wireless Audio, Coffee Maker)
- Verify each device shows status (ON/OFF)

### Expected Results
- All IoT device cards are displayed
- Each device shows name and current status
- Device icons are appropriate and visible
- Device cards are arranged in a grid layout

#### Step 6: Test Dashboard - Device Control (if interactive)
- Locate a device card
- Look for toggle or control element
- Attempt to change device status

### Expected Results
- Device cards may show control buttons
- If interactive, status can be changed
- UI updates to reflect new status
- No errors occur during status change

#### Step 7: Test Dashboard - Energy Monitoring
- Locate the energy consumption section
- Verify display of "Consumed" and "Spent" metrics
- Look for consumption value and currency

### Expected Results
- Energy data is displayed with proper formatting
- Consumed kWh value is shown correctly
- Spent USD amount is shown correctly
- Units are labeled (kWh, USD)

#### Step 8: Test Dashboard - Chart Section
- Locate the temperature and energy charts
- Verify charts render properly

### Expected Results
- Temperature chart displays with proper visualization
- Energy/cost chart shows data graphically
- Charts have proper labels and axes
- Chart data appears to be valid and scaled correctly

#### Step 9: Test Responsive Layout - Desktop
- Verify page layout is optimal for desktop (> 1024px)
- Sidebar is visible
- Main content takes appropriate width

### Expected Results
- Desktop layout is well-proportioned
- No horizontal scrolling
- Content is properly aligned and spaced
- Multi-column layouts work as expected

#### Step 10: Test Responsive Layout - Tablet
- Resize browser to tablet width (768px - 1024px)
- Verify layout adapts appropriately

### Expected Results
- Layout adjusts for tablet size
- Sidebar may collapse or resize
- Content remains readable and accessible
- Touch targets are appropriately sized

#### Step 11: Test Responsive Layout - Mobile
- Resize browser to mobile width (< 768px)
- Verify layout adapts for mobile viewing

### Expected Results
- Layout is optimized for mobile
- Sidebar is hidden or hamburger menu appears
- Content stacks vertically
- Touch-friendly spacing and sizing
- No horizontal scrolling

### Accessibility Requirements
- Calendar has keyboard navigation (arrow keys)
- Calendar dates are semantic (table or list structure)
- Device cards have appropriate ARIA labels
- Chart data is accessible via alternative means
- Color is not the only indicator of status
- Buttons have descriptive text/labels
- Focus indicators are clearly visible
- Form labels are associated with inputs

### Content Validation
- All device names are spelled correctly
- Energy values are numeric and make sense
- Date formatting is consistent
- Chart labels are clear and relevant
- Sample data is realistic and accurate

### Performance Considerations
- Charts render smoothly without lag
- Calendar interactions are responsive
- Page load time is under 3 seconds
- No console errors or warnings
- Network requests complete successfully
- Memory usage is reasonable

### Browser & Device Testing
- Test on latest Chrome, Firefox, Safari, Edge
- Test on iOS and Android devices
- Verify touch interactions work on mobile
- Test with different screen resolutions (1920x1080, 1366x768, 375x667, etc.)
- Test with browser zoom (75%, 125%, 150%)

### Data Integrity
- Device status reflects actual state
- Energy consumption values are consistent
- No data truncation or overflow
- Dates are correctly formatted
- Currency symbols are appropriate
