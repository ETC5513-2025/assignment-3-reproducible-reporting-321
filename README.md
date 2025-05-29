# COVID-19 Impact Analysis: Cases, Deaths, and Vaccination Rates Across Canada, France, Germany, India, the United Kingdom, and the United States.

This project analyzes the impact of COVID-19 confirmed cases, deaths, and vaccination rates across Canada, France, Germany, India, the United Kingdom, and the United States from February 2020 to July 2023. It explores the role of vaccination in reducing case numbers and mortality rates, providing insights into effective pandemic responses.

## 👥 Group Members
- Midhun Unnikrishnan (GitHub: @MidhunUnnikrishnan7)
- Sumintra Boonmat (GitHub: @SumintraB)
- Lin Qi (GitHub: @linqi70)

## 📌 Project Description
This project examines the temporal relationship between COVID-19 confirmed cases, deaths, and vaccination rates across six countries: Canada, France, Germany, India, the UK, and the US. Using time series data from Our World in Data, we analyze trends from February 2020 to July 2023, focusing on the period from January 16, 2021, to September 4, 2022, for consistent vaccination data comparison. The analysis includes visualizations of vaccination uptake, daily changes in cases and vaccinations, and the lagged effect of vaccination on case numbers. Key findings highlight that early and sustained vaccination campaigns significantly reduced case numbers and mortality rates, with countries like the US and UK showing notable declines in cases following vaccination rollouts.

The project is implemented using R and Quarto, producing a comprehensive PDF report with embedded visualizations and tables. The analysis underscores the importance of timely vaccine deployment and consistent data reporting for effective public health responses.

## 📁 Project Structure
```
├── Analysis_files/                                # Folder of figures png files
│   ├── figure-pdf                                 # Figures png files
├── Analysis.qmd                                   # Quarto source file for the analysis report
├── Analysis.pdf                                   # Rendered PDF output of the report
├── Analysis.tex                                   # LaTeX output file from Quarto rendering
├── Covid-19_analysis.Rproj                        # RStudio project file
├── custom-header.tex                              # LaTeX header for PDF formatting
├── data/                                          # Folder for datasets
│   ├── COVID-19 confirmed case per million.csv    # Dataset for confirmed cases per million
│   ├── Total confirmed deaths due to COVID-19 per 100,000 people.csv  # Dataset for deaths per 100,000
│   ├── COVID-19 vaccination.csv                   # Dataset for vaccination doses per million
├── Presentation.qmd                               # Quarto Reveal.js presentation
├── covid19_presentation.html                      # Rendered HTML slides
├── covid19_presentation_files/                    # Reveal.js support files
├── images/                                        # Image assets for slides
│   ├── cases_vaccination.png
│   ├── cases_deaths_vaccination.png
│   ├── lagged_vaccination_vs_cases.png
├── README.md                                      # Project overview and instructions
├── LICENSE                                        # Apache License 2.0
├── references.bib                                 # Citations
├── renv/                                          # R environment management folder
├── renv.lock                                      # R environment lockfile
```

## 🚀 Getting Started

### Prerequisites
To run this project, ensure you have the following installed:
- **R** (version 4.5.0 or higher)
- **Quarto**
- **R Packages**:
  - `tidyverse`
  - `lubridate`
  - `ggplot2`
  - `knitr`
  - `here`
- **LaTeX** distribution
- **Renv** 

Install the required R packages using:
```R
install.packages(c("tidyverse", "lubridate", "ggplot2", "knitr", "here"))
```

Restore the R environment using `renv`:
```R
renv::restore()
```

### Running the Project
1. Clone the repository:
   ```bash
   git clone git@github.com:ETC5513-2025/assignment-3-reproducible-reporting-321.git
   ```
2. Open `Covid-19_analysis.Rproj` in RStudio to load the project.
3. Render the Quarto file to generate the PDF report:
   ```bash
   quarto render Analysis.qmd --to pdf
   ```
4. View the output in `Analysis.pdf`.

## 📜 License
This project is licensed under the Apache License 2.0.
See the LICENSE file for details.