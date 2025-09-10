
# Assignment 3 – Collaborative Workflows with Git

**Student:** Shokhrukhbek Valijonov (ID: 475154)  
**Professor:** Wojciech Hardy  
**Course:** Reproducible Research 2025  

---

## Task
This assignment focuses on demonstrating collaborative coding workflows using Git and showing how reproducible practices can be applied to real-world datasets.

---

## Git Workflow Demonstrated
```bash
# Stage and commit population analysis script
git add population_analysis.R
git commit -m "feat: add population growth analysis with cleaning and plotting"

# Push changes to remote repository
git push origin main
```

This workflow highlights **clear commit messages**, code structuring, and synchronization with a remote repository to ensure reproducibility in collaboration.

---

## Global Example: Urban Population Growth
To illustrate reproducibility with meaningful data, I used the **World Bank urban population dataset**. This example shows how rapid urbanization affects different regions and how reproducible code can analyze such patterns.

```r
# R example: analyzing urban population growth
library(dplyr)

data <- data.frame(
  country = c("China", "India", "Nigeria", "Brazil", "Poland"),
  year2000 = c(459, 278, 58, 138, 23),
  year2020 = c(641, 483, 110, 185, 24)
)

data <- data %>%
  mutate(growth_rate = (year2020 - year2000) / year2000 * 100)

print(data)
```

This script shows:
- **Data manipulation** with reproducible R code.  
- **Calculation of growth rates** across countries.  
- A global perspective on how urbanization trends can be studied.

---

## Reflection
- Using Git with structured commits supports collaborative research.  
- Documentation and reproducible code are key to transparent scientific practices.  
- Real-world data (like **urban population growth**) makes reproducible workflows practical and impactful.
