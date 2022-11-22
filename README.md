# RADx Data Dictionary Analysis

A repository for the analysis of various RADx data dictionaries.  The repo contains a folder called "curated" that contains a collection of cleaned data dictionaries by Data Collection Center (DCC).  To process the data dictionaries run the "process-data-dictionaries.sh" script.  The processing will produce a series of folders containing intermediate processed data dictionaries and then a merge of all data dictionaries in a file called `merged.csv`.

## Cloning and Running the Analysis

Open a terminal with the working directory set to the directory where you would like to clone the repo.  Type,

```
git clone https://github.com/RADx/radx-data-dictionary-analysis.git
```

Next, switch to the cloned repo directory, `radx-data-dictionary-analysis` directory,

```
cd radx-data-dictionary-analysis
```

Next run the script (see note below),

```
./process-data-dictionaries.sh ./curated ./generated
```

This will output processing files in the `generated` directory.

## RADx Data Dictionary Explorer Tool

This script requires the [RADx Data Dictionary Explorer](https://github.com/RADx/radx-data-dictionary-explorer) command line tool.  The script uses an alias `dd` to this tool.  You should build and install the tool and then set up an alias to the tool.

