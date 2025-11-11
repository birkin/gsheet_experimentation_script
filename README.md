# gsheet-experimentation-script


## purpose

Repo to experiment with accessing google-sheets programmatically.


## gspread documentation
<https://docs.gspread.org/en/latest/>


## resources

- "[Automate Google Sheets With Python - Google Sheets API Tutorial](https://www.youtube.com/watch?v=zCEJurLGFRk)" -- `Tech With Tim` youtube channel


## notes

- "project" vs "service account"
    - A "project" is the top-level entity in the Google Cloud Platform (GCP) hierarchy. I think analytics operate that this level. I've seen recommendations to think of a project as a kind of "environment", and name accordingly, like `bdr_connector_prod`.
    - A "service account" is an entity that represents an application in the GCP environment. I've seen recommendations to name a service account to indicate the application and its function -- something like `sa-warctracker-gsheet-writer`.

- "batching" -- either at the free "project" or "service account" level, there's a limit to how many connections you can make in a given amount of time. gspread, and likely other tools, enable "batching" to group multiple edits together -- to make the most of the available quota.

- previous work: ocra-extractor script -- add link.

---