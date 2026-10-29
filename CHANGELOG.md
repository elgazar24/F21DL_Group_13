# Changelog

All notable changes to this project are documented here.
The changelog is maintained from Mon 26 Oct 2026 onwards: every session or
commit that changes the repo must be recorded here.

## [Unreleased]

### Changed - Mon 26 Oct 2026 - @melgazar - commit: `$CommitID`

1. **Repo name** - renamed the repository to meet the naming requirement in
   the [Coursework Process Handbook (v1.1)](assets/docs/uni_materials/CWProcessHandbook-v1.1.pdf).

   - From: `F21DL_Group_13`
   - To: **[f21dl-2026-27-PG-group-13](https://github.com/elgazar24/f21dl-2026-27-PG-group-13)**
2. **Notebooks hierarchy** - restructured the
   [notebooks](src/notebooks) folder into topic-based folders:

   - `Data_Analysis`
   - `Data_Exploration`
   - `Feature_Engineering`
   - `Feature_Selection`
   - `Models`
3. **Models structure** - changed [Models](src/notebooks/Models) from one
   stand-alone notebook file per model to a folder with multiple files per
   model, to avoid spaghetti code and follow best practices and SOLID.

   - To be: `Decision_Tree`, `KNN`, `MLP`, `Naive_Bayes`
4. **Datasets structure** - changed [Datasets](assets/datasets) to four category dataset types
5. **Filled the Info Files for the Datasets in more organized and accurate way**

### Changed - Thu 29 Oct 2026 - @melgazar - commit: `$CommitID`

1. **configs/config.json** - rewrote as the single source for all notebooks:
   dataset folders and file paths (relative to `configs/`), target columns
   and classes, null symbols, the feature list of each dataset with its
   types, per-stage file slots, and `selected_features` per dataset. The
   used dataset is switched in one place.
2. **Data exploration** - rebuilt
   [1_Data_Exploration](src/notebooks/1_Data_Exploration) into three
   self-contained notebooks (`00_main` entry, `get_general_info`,
   `data_cleaning`) that read everything from the config and only show
   results; removed the old helper scripts.
3. **DS1 source repair** - the UCI csv header was missing the `pcv` column,
   which shifted every column after `hemo`; 15 rows carried stray tab
   characters and 3 rows were malformed. Repaired in place, so a plain
   `read_csv` loads 400 rows x 25 columns with the documented 250/150 class
   split. Regenerated `DS1_cleaned.csv` from the repaired source.
4. **Feature selection** - built
   [Feature_Selection](src/notebooks/Feature_Selection): `00_main` entry,
   `target_sanity_check` (labels vs core labs: DS1 labels clearly track
   them, DS2 labels do not), and `feature_selection` (mutual information +
   RF permutation importance, redundancy pruning, agreement ranking) which
   writes `selected_features` into the config per dataset (DS1: 12 of 24,
   DS2: 15 of 47, provisional).
5. **requirements.txt** - added `nbclient`, `nbconvert` and `nbformat` for
   headless notebook execution.
6. **.gitignore** - added `__pycache__/`.
