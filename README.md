# KSEL Match Results Entry System

A web-based form for entering Fortnite match results for the Kern Scholastic Esports League (KSEL).

## Live Form Access

**Students and Coaches:** Access the form at: [Match Results Form](https://erikmadams.github.io/ksel-fortnite-results/)

## What This Form Does

This form allows Duo teams to quickly enter match results including:
- Team placement (Victory Royale through 50th place)
- Individual player statistics for both players on the Duo
  - Eliminations
  - Assists
  - Revives
  - Accuracy
  - Damage to Players
  - Damage Taken
  - Distance Traveled
  - Hits
- Automatic point calculations based on the KSEL scoring system
- Live gamer tag verification against real Fortnite accounts
- Direct submission to a database for data collection

**Students and Coaches:** Make sure to grab a screenshot of each athlete's Match Stats at the end of their match! (They will need it)

## KSEL Scoring System

- **Victory Royale (1st Place):** 25 points
- **2nd - 9th Place:** 20 points
- **10th - 17th Place:** 15 points
- **18th - 35th Place:** 10 points
- **36th - 50th Place:** 5 points
- **Eliminations:** 2 points each

## How to Use

1. **Fill in Match Information**
   - Select your school
   - Select your team name from the dropdown
   - Select the date (current date is automatically populated)
   - Choose game mode (Battle Royale or Zero Build)

2. **Enter Team Placement**
   - Input where your team finished. Victory Royale is 1st place; placements through 50th earn points.

3. **Add Player Stats**
   - Enter both players' gamer tags
     - When you tab out of a gamer tag field, the form checks it against Fortnite and shows a ✓ Verified or ✗ Not found note next to it. This is just a heads-up for typos — it never blocks you from saving.
   - Fill in each player's individual statistics
     - Make sure to use the screenshot you took of your match stats
   - The form automatically calculates team totals

4. **Submit Results**
   - Click "Save Results" to submit to the database
   - Results are automatically saved to the database

## Tips for Coaches

- **Accuracy:** Enter as a percentage (e.g., 45.2 for 45.2%)
- **Damage:** Enter whole numbers without commas
- **Required Fields:** ALL FIELDS ARE REQUIRED
- **Gamer Tag Check:** The ✓/✗ next to each gamer tag is a helpful nudge, not a hard requirement — a ✗ (or no result at all) just means double-check the spelling before saving
- **Real-time Updates:** Team summary updates automatically at the bottom as you type

## 🔧 Technical Details

- Built with HTML, CSS (Tailwind), and JavaScript
- No installation required - runs in any modern web browser
- Responsive design works on desktop, tablet, and mobile
- Data submitted directly to database (Google Sheets) via Google Apps Script
- Gamer tags are verified against Fortnite through that same Google Apps Script backend, so no API key is ever exposed in the page
- Form validation ensures accurate data entry

## Troubleshooting

**Form won't submit?**
- Check that team name and placement are filled in (Make sure you didn't miss any fields)
- Ensure you have an internet connection
- Try refreshing the page and re-entering data

**Gamer tag shows "✗ Not found"?**
- Double-check the spelling and capitalization of the tag
- It's still fine to save if you're sure the tag is correct — the check can occasionally miss real accounts that have their stats set to private

**Can't access the form?**
- Make sure you're using the correct URL
- Try a different web browser
- Clear your browser cache and try again

## Data Collection

All submitted results are automatically collected in a database that includes:
- Team and match information
- Individual player statistics
- Calculated points and team totals
- Timestamp of submission

## Support

For technical issues or questions about the form:
- Contact your match official
- Report issues on the [GitHub Issues](https://github.com/erikmadams/ksel-fortnite-results/issues) page
- Email: erik_adams@kernhigh.org

## Version History
- v1.0: Initial release with all current features
- v2.0: Switched from Squad (4 players) to Duo (2 players) format; updated the KSEL scoring system (renamed 1st to Victory Royale, new placement brackets through 50th, eliminations now worth 2 points instead of 4); added live gamer tag verification against Fortnite; fixed a school dropdown bug where selecting "Kern Valley" was submitting as "Liberty"; cleared the team name list pending this year's rosters

## Support
For technical support or feature requests, contact the KSEL leadership team.

## License
Developed for Kern Scholastic Esports League by LeagueHQ developers. For KSEL internal use only.
