# Hive Analytics Dashboard

A real-time analytics dashboard for monitoring Hive blockchain accounts and their post payouts.

## Screenshots
![image](https://github.com/user-attachments/assets/36e16ef3-b6b2-47bf-82b9-24fb5a8e31ae)
![image](https://github.com/user-attachments/assets/707ac15c-24d7-4bec-9ed4-671781a89910)

## Features

- Real-time monitoring of multiple Hive accounts
- Batch processing with configurable size
- Multiple API endpoint support with load balancing
- Post filtering by date and payout value
- Sortable results table with live updates
- Live progress tracking
- Enhanced activity logging with search and clear functionality
- Pause/Resume functionality
- Reblog filtering (shows only original content)

## Settings

- **Days to Look Back**: Number of days to check for posts (1-365)
- **Min HBD Threshold**: Minimum payout value to include (in HBD)
- **Retry Limit**: Number of API retry attempts
- **Timeout**: API call timeout in seconds
- **Processes**: Number of concurrent processes
- **API Call Delay**: Delay between API calls in seconds
- **Batch Size**: Number of accounts to process in each batch

## Activity Log Features

- Real-time log updates
- Search functionality for filtering log entries
- Clear logs button
- Color-coded log entries by type:
  - Info (blue)
  - Success (green)
  - Error (red)
  - Warning (yellow)
  - API (purple)
  - Fetch (light blue)
  - Process (light green)

## API Endpoints

Default endpoints included:
- api.hive.blog (enabled)
- api.deathwing.me (enabled)
- api.openhive.network (enabled)
- techcoderx.com (disabled)
- api.c0ff33a.uk (disabled)
- rpc.mahdiyari.info (disabled)

You can add/remove endpoints and enable/disable them as needed. The system automatically checks endpoint status and uses only online endpoints.

## Usage

1. Open `index.html` in a modern web browser
2. Enter Hive accounts (one per line) or load from a text file
3. Adjust settings as needed
4. Click "Start Monitoring"
5. View results in real-time as they're found

## Results Table

The results table shows:
- Username
- Post Date
- Link to Post
- HBD Value
- Post Title (truncated)

Click column headers to sort by that column.

## Technical Details

- Pure HTML/CSS/JavaScript implementation
- No external dependencies
- Supports large account lists through batch processing
- Automatic API failover and load distribution
- Real-time updates with sort preservation

## Requirements

- Modern web browser with JavaScript enabled
- Internet connection to access Hive APIs

## File Structure

```
findblacklistaccounts/
├── index.html      # Main application
├── README.md       # Documentation
```

## License

MIT License - Feel free to use and modify as needed.
