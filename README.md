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
- A Team Name dropdown that automatically filters to just your school's teams once you select your School
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
   - Select your team name from the dropdown (this list automatically narrows down to just your school's teams once a school is selected — if your team isn't listed, contact your league admin so it can be added)
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
- **Team Name list looks empty or wrong?** The Team Name dropdown only fills in once a School is selected, and only shows teams that have been added for that school — contact your league admin if a team is missing

## For League Admins: Managing the Team Roster

The Team Name dropdown pulls its list live from a Team Roster that league admins manage directly from the same page — no separate site or login to remember.

**Access:** Only administrators can access this management page.  If you know how to get there, you are an admin.

**What you can do there:**
- Pick a school and see every team currently on file for it
- Add a new team to that school
- Remove a team that's no longer active

Changes save immediately and show up in the Team Name dropdown on the regular form right away — no redeploy or page refresh gymnastics needed. Behind the scenes, this reads and writes a "Teams" tab in the same Google Sheet the match results themselves go into, so the full roster is also visible (and editable in a pinch) directly in Google Sheets if needed.

## 🔧 Technical Details

- Built with HTML, CSS (Tailwind), and JavaScript
- No installation required - runs in any modern web browser
- Responsive design works on desktop, tablet, and mobile
- Data submitted directly to database (Google Sheets) via Google Apps Script
- Gamer tags are verified against Fortnite through that same Google Apps Script backend, so no API key is ever exposed in the page
- The Team Name list is loaded live from a "Teams" tab in the same Google Sheet, via the same Google Apps Script backend — kept in sync with the Team Roster Admin view (see above)
- Form validation ensures accurate data entry

## Troubleshooting

**Form won't submit?**
- Check that team name and placement are filled in (Make sure you didn't miss any fields)
- Ensure you have an internet connection
- Try refreshing the page and re-entering data

**Team Name dropdown is empty or missing your team?**
- Make sure a School is selected first — the Team Name list only loads after that
- If your team truly isn't listed, it hasn't been added to the roster yet — contact your league admin (see the Team Roster Admin section above)

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
- v2.1: Added a Team Roster Admin view for league admins to add/remove teams per school; the Team Name dropdown now loads live from that roster and filters to the selected school, replacing the old static/placeholder team list

## Support
For technical support or feature requests, contact the KSEL leadership team.

## License
Developed for Kern Scholastic Esports League by LeagueHQ developers. For KSEL internal use only.
