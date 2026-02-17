## Test Plan: Navigation & Theme Module

### Test Steps

#### Step 1: Navigate to Dashboard Home
- Navigate to https://dashboard-automation.netlify.app
- Verify the IoT Dashboard page loads

### Expected Results
- Page loads successfully and displays the IoT Dashboard
- Left sidebar with navigation menu is visible
- Header with theme selector is visible
- Main content area displays IoT devices and monitoring data

#### Step 2: Test Theme Selector - Light Theme
- Click on "Light" theme dropdown in header
- Verify Light theme is currently active
- Observe the light color scheme applied

### Expected Results
- Theme selector dropdown displays available themes: Light, Dark, Cosmic, Corporate
- Light theme is selected/active
- Page uses light colors (light backgrounds, dark text)
- All interactive elements are properly styled

#### Step 3: Test Theme Selector - Change to Corporate
- Click on theme dropdown
- Select "Corporate" theme
- Observe color scheme change

### Expected Results
- Theme switches to Corporate theme
- Page colors update to corporate color scheme
- All elements (buttons, cards, text) reflect new theme
- Theme selection is persistent (if page refresh, theme remains)

#### Step 4: Test Theme Selector - Dark Theme
- Click on theme dropdown
- Select "Dark" theme
- Observe dark color scheme applied

### Expected Results
- Dark theme is applied
- Background is dark, text is light
- All interactive elements are visible and readable in dark theme
- No contrast issues

#### Step 5: Test Theme Selector - Cosmic Theme
- Click on theme dropdown
- Select "Cosmic" theme
- Observe cosmic color scheme

### Expected Results
- Cosmic theme is applied with unique color palette
- All UI elements are properly styled for cosmic theme
- Colors are distinguishable and readable

#### Step 6: Test Navigation Menu - Expand/Collapse
- Click on main menu items to expand submenus
- Verify submenu items appear

### Expected Results
- Menu items expand to show child pages
- Collapse icon appears when menu is expanded
- Submenus display all available child pages
- Menu state is visually clear (active item highlighted)

#### Step 7: Test Navigation - Sidebar Links
- Click on "IoT Dashboard" link
- Verify page navigates to dashboard

### Expected Results
- Navigation links work correctly
- Page content changes to reflect selected section
- Current page/section is highlighted in sidebar
- Breadcrumb or active state indicator is visible

#### Step 8: Test Mobile Navigation (if applicable)
- Resize browser to mobile width (< 768px)
- Verify hamburger menu appears
- Click hamburger menu
- Verify sidebar opens/displays

### Expected Results
- Mobile view shows responsive navigation
- Hamburger menu icon appears on mobile
- Menu can be toggled open/closed
- Mobile layout is readable and usable
- No horizontal scrolling required

#### Step 9: Test Header Elements
- Verify page logo is visible
- Verify application title is visible
- Verify search icon is visible (if applicable)
- Verify user profile icon is visible

### Expected Results
- All header elements are properly positioned
- Logo links to home page
- Search functionality is accessible (if available)
- User profile icon is clickable (if applicable)

#### Step 10: Test Theme Persistence
- Change to a different theme (e.g., Corporate)
- Refresh the page
- Verify theme remains applied

### Expected Results
- Selected theme persists after page refresh
- Theme preference is stored (localStorage/cookies)
- User doesn't need to reselect theme

#### Step 11: Test Navigation Across Different Pages
- Navigate to Forms → Form Layouts
- Navigate to Modal & Overlays → Dialog
- Navigate to Charts → Echarts
- Navigate back to Dashboard
- Verify smooth navigation and no broken links

### Expected Results
- All navigation links work correctly
- Page content loads for each section
- No 404 errors
- Page transitions are smooth
- Navigation history works (back button functions)

### Accessibility Requirements
- Navigation is keyboard accessible (Tab through menu items)
- Menu items have proper focus indicators
- Font sizes are readable (16px minimum for body text)
- Color contrast meets WCAG AA standards
- Theme options are labeled and identifiable
- Screen readers announce menu structure and current page
- ARIA attributes properly indicate menu state (expanded/collapsed)

### Test Data Validation
- All navigation links are functional
- No broken links or redirects
- Page titles match navigation labels
- URL structure is consistent and logical
- Theme selector displays all available themes

### Performance Considerations
- Page loads within 3 seconds
- Theme change is instant or very quick (< 500ms)
- Navigation doesn't cause page flicker
- No console errors when changing themes
- Network requests complete successfully

### Browser Compatibility
- Test on Chrome, Firefox, Safari, Edge
- Test on iOS Safari and Android Chrome
- Verify responsive behavior at different breakpoints
- Check theme colors render correctly across browsers
