## Geniusee Timesheets — User Manual

### What it does
A fast, Tempo‑style month view for Jira Cloud to review logged work:
- Employees × days grid with weekend highlighting
- Per‑day and per‑user monthly totals
- Expand users to see issue‑level time per day
- Filters for month, employees, and projects
- Issue keys open in a new tab

### Accessing the app
- From any Jira project: sidebar → Apps → Geniusee Timesheets
- From top navigation: Apps → Geniusee Timesheets

### Permissions
- Read‑only access to worklogs, issues, users, and projects
- Respects Jira permissions; you only see data you’re allowed to view

### Layout overview
- Top toolbar:
  - Month switcher (‹ ›)
  - Employees and Projects multi‑selects with search and chips
  - Apply button
- Grid:
  - First column: employee
  - Second column: monthly total (hours)
  - Day columns (1–31): daily hours; weekends are lightly shaded
  - Click the triangle next to a user to expand issue/task rows

### Color coding
- Cells with < 8h: red pastel
- Cells with ≥ 8h: green pastel
- Weekends: light gray background

### Filters
- Month: use the arrows to switch months
- Employees: click field, search, select; multiple selections become chips
- Projects: same as employees
- Click Apply to refresh the grid

Notes:
- Filters persist between visits
- To reset saved filters, clear browser storage for:
  - `localStorage.removeItem('gts.filters.v1')`

### Drill‑down to tasks
- Expand a user to see issue keys as nested rows
- Each nested row shows per‑day time on that issue
- Click an issue key to open it in a new tab

### Totals
- Per‑day totals per user are shown in day cells
- Per‑user monthly total is shown in the second column
- Per‑issue total is shown on the nested row’s second column

### Tips for accurate results
- Use Projects filter to limit scope for large instances
- Pick a month with actual worklogs
- Expand a user to validate time distribution across issues

### Troubleshooting
- “No data” for selected month:
  - Remove filters or pick another month with worklogs
- Not seeing someone in the list:
  - Only active Atlassian accounts are shown; system/users like “Geniusee” (company placeholder) are excluded
- Links don’t open:
  - Ensure your browser allows pop‑ups in Jira; links open with `target=_blank`

### Keyboard/mouse shortcuts
- Expand/Collapse user: click the triangle next to the user name
- Open issue: click the issue key link (opens in a new tab)

### Data privacy
- Read‑only; no changes to Jira data
- No external storage 

### Support
- For help, feedback, or feature requests (CSV export, targets, holidays, workload schemes), contact your vendor support channel or file a request via your Jira site’s app management page. 
