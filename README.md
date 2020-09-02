# COVID-19 Dataset for Berlin / Germany

This dataset describes the development of known COVID-19 cases in the city of Berlin/Germany and in its districts. The dataset was compiled from the data given in the [official press releases](https://www.berlin.de/sen/gpg/service/presse/2020/) of the Berlin administration (Senatsverwaltung für Gesundheit, Pflege und Gleichstellung) and may be used e.g. for educational or academic research purposes. Please always check with the official data sources before use, as the data may still contain typos or mapping errors. Please do not use this data for any kind of medical advise.

The data set collects the data from March 1 to August 30, 2020. Since August 31, 2020, the data is now summarized as a [daily status report](https://www.berlin.de/corona/lagebericht/desktop/corona.html#start) by the State of Berlin.

## Known Cases

![Known cases in Berlin](/plots/berlin_cases.png)

## Daily Reports (daily\_report)

The folder contains daily case reports. All timestamps are in CET (GMT+1). Files are named by the convention: YYYY-MM-DD.csv. All data is stored in a [comma-seperated value](https://en.wikipedia.org/wiki/Comma-separated_values) file with the first line containing the field names. 

* berlin\_districts: daily reports of confirmed and recovered cases for each district.
* berlin: daily reports of confirmed, hospital, critical, death and recovered cases for the city of Berlin.

## Field Description 

All datasets contain combinations of the following fields. Blank fields or unknown values are represented explicitly by the value "".

* publication\_date: defines the date of the press release in the format YYYY-MM-DD. The date does not necessarily correspond to the date of elicitation.
* district: district name, e.g. "Spandau"
* state: province name, e.g. "Berlin"
* country: country name, e.g. "Germany"
* confirmed: the number of confirmed cases (includes hospital cases).
* hospital: the number of cases staying at a hospital (includes critical cases).
* critical: the number of cases staying at a hospital in a critical care unit.
* deaths: the number of deaths.
* recovered: the number of recovered cases.
* source: the URL to the official press release that contains the numbers, e.g. "https://www.berlin.de/sen/gpg/service/presse/2020/pressemitteilung.908263.php"

## Data Sources

We compiled our data from the following sources:

* Press releases of the Berlin administration (Senatsverwaltung für Gesundheit, Pflege und Gleichstellung): <https://www.berlin.de/sen/gpg/service/presse/2020/>

A big thanks to the maintainers of these sources.

## Other Projects

* the user plebln has also collected the COVID data of Berlin in his [corona-berlin-2020](https://github.com/plebln/corona-berlin-2020) project

## Terms of Use

The repository and its contents herein, including all data ist published under the CC0 1.0 public domain license (no rights reserved). The data relies upon publicly available data from multiple sources, that do not always agree. The maintainer of this repository makes no warranties about the work, and disclaims liability for all uses of the work, to the fullest extent permitted by applicable law. Also see the [LICENSE](LICENSE) file for more details.
