# KSEL Match Results Entry System

A web-based form for entering Fortnite match results for the Kern Scholastic Esports League (KSEL).

## Live Form Access

**Students and Coaches:** Access the form at: [[https://erikmadams.github.io/ksel-fortnite-results](https://erikmadams.github.io/ksel-fortnite-results/)]

## What This Form Does

This form allows teams to quickly enter match results including:
- Team placement (1st-25th place)
- Individual player statistics
-   Eliminations
-   Assists
-   Revives
-   Accuracy
-   Damage to Players
-   Damage Taken
-   Distance Traveled
-   Hits
- Automatic point calculations based on KSEL scoring system
- Direct submission to Google Sheets for data collection

**Students and Coaches:** Make sure to grab a screenshot of each athletes Match Stas at the end of their match! (They will need it)

## KSEL Scoring System

- **1st Place:** 25 points
- **2nd-5th Place:** 20 points  
- **6th-9th Place:** 15 points
- **10th-18th Place:** 10 points
- **19th-25th Place:** 5 points
- **Eliminations:** 4 points each (max 50 points per team)

## How to Use

1. **Fill in Match Information**
   - Enter your team name (Liberty Squad 1)
   - Select the date
   - Choose game mode (Battle Royale or Zero Build)

2. **Enter Team Placement**
   - Input where your team finished (1-25)

3. **Add Player Stats**
   - Enter each player's gamer tag
   - Fill in their individual statistics
   -   Make sure to use the screen shot you took of your match stats
   - The form automatically calculates team totals

4. **Submit Results**
   - Click "Save Results" to submit to the database
   - Results are automatically saved to Google Sheets

## Tips for Coaches

- **Accuracy:** Enter as a percentage (e.g., 45.2 for 45.2%)
- **Damage:** Enter whole numbers without commas
- **Required Fields:** ALL FIELDS ARE REQUIRED
- **Real-time Updates:** Team summary updates as you type at the bottom

## 🔧 Technical Details

- Built with HTML, CSS (Tailwind), and JavaScript
- No installation required - runs in any modern web browser
- Responsive design works on desktop, tablet, and mobile
- Data submitted directly to Google Sheets via Google Apps Script
- Form validation ensures accurate data entry

## Troubleshooting

**Form won't submit?**
- Check that team name and placement are filled in (Make sure you didn't miss any fields)
- Ensure you have an internet connection
- Try refreshing the page and re-entering data

**Can't access the form?**
- Make sure you're using the correct URL
- Try a different web browser
- Clear your browser cache and try again

## Data Collection

All submitted results are automatically collected in a Google Sheet that includes:
- Team and match information
- Individual player statistics
- Calculated points and team totals
- Timestamp of submission

## Support

For technical issues or questions about the form:
- Contact your match official
- Report issues on the [GitHub Issues](https://github.com/erikmadams/ksel-fortnite-results/issues) page
- Email: erik_adams@kernhigh.org

## Updates

This form is regularly updated to improve functionality. Bookmark the URL above for the latest version.

---

**Last Updated:** September 2025  
**Version:** 1.0  
**League:** Kern Scholastic Esports League (KSEL)
