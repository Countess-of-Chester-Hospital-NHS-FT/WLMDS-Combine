
# WLMDS Combine

### Status
This project is completed, but not actively being maintained. This was completed as an adhoc piece of work and as such, could definitely be improved upon goven some more time / resource.

### About the project
All the Waitlist MDS submission files live in the Corrected Submissions folder with one submission file for each week. This repo contains a script which selects the latest version of the OpenPathways submission files for each week and combines them into one table that is output as a .csv file (for manual import into the data warehouse) or a pickle file for further analysis in python.

For further training materials see Skill Swap session (25.04.10 - Python for analysts 1).

No data is shared in this repository

### In order to use this code

* Download a copy of this repo (Big Green code button, download as zip, extract the zip file to your Desktop or other sensible location)
* Open script.py in the IDE of your choice
* Add the filepath of the Corrected Submissions folder to the relevant part of the script
* Run the script (should receive confirmation "All file dates are unique")
* The combined data should appear in the outputs folder
* Import manually into the data warehouse (delete the currect WLMDS_Combined table, use Tasks, Import Flat File, follow wizard - note that you will need to adjust datatypes for many of the fields to either nvarchar(50) or datetime2 and allow nulls for all columns - the automatic data detection doesn't work very well)

### Built with
Should run fine using anaconda Base Python environment (3.11.7)

### Contributing
Contributions and identification of issues are welcomed.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/Feature`)
3. Commit your Changes (`git commit -m 'Add some Feature'`)
4. Push to the Branch (`git push origin feature/Feature`)
5. Open a Pull Request

### License
Unless stated otherwise, the codebase is released under the MIT Licence. This covers both the codebase and any sample code in the documentation.

See LICENSE for more information.
