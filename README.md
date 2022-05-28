# Introduction
Hi! I'm Jarryd. I recently graduated from the University of Georgia (2018-2022) with a certificate in Financial Technologies, a BBA in Management Information Systems (MIS) with an emphasis in Data Analytics, and a MS in Business Analytics. 

# Portfolio Directory
A repository consisting of projects completed through my part time graduate assistantship, online courses, and personal projects. These projects will primarily be in R and Python 

## Web Application Development Portfolio
### Assistantship
During my time in grad school, I held a position with the MIS department at the Terry School of Business and built out several web applications (some of which have been made public and are available below).

These web applications were developed for greenhouse growers as part of [Project LAMP](https://www.hortlamp.org/outreach/determine-lighting/), lighting approaches to maximize profits. Our goal is to maximize controlled environment agriculture (CEA) grower profits through improved lighting systems and support tools.

These calculators (LightingCalc, SupplementalCalc, and TargetCalc) use a geolocation API to transform a user inputted zipcode to latitude and longitude which is then passed to the TMY API to retrieve location specific weather data. The core idea behind the calculators is this: plants require light to grow. There's an optimal (target) amount of light that a plant can receive over the course of the day (Target DLI). These calculators all focus on the target DLI, but they do so in different ways:

#### LightingCalc
**Background:** When I started my assistantship,the two previous students who held this position over the last two years had developed LightingCalc. My first task was to tweak the UI and server code to display values at a weekly view as opposed to a monthly view and add in demand charges. After familiarizing myself with LightingCalc, I discovered that it was making an unrealistic assumption: growers want to provide enough supplemental light to reach their target DLI _every single day of the year_. Because of that unrealistic assumption, I decided not to calculate demand charges and begin working on two new calculators (SupplementalCalc and TargetCalc). LightingCalc is hosted on ShinyApps and is available [here](https://uga-lighting-calc.shinyapps.io/lightingcalc/).

**Description:** LightingCalc was created to determine how much electricity is required to reach the target DLI every single day of the year. To do so, a lighting system would need to be designed to provide enough light on even the darkest day of the year. On the Electricity Cost page, users will view a dashboard that calculates lighting costs at an annual, monthly, and weekly view.

**General Skills:** APIs, Data Transformation, Data Analytics, Data Visualization, Web App Development
**Specific Skills:** R (main libraries: shiny, dyplr, ggplot2, lubridate, tidygeocoder)

#### SupplementalCalc
**Background:** After realizing the unrealistic assumption made in LightingCalc, I set out to build a new calculator that relaxed that assumption. The result was a web application that allows a user to specify what percent of the year they'd like to reach their target DLI and how many hours they light their greenhouse. I also rebuilt the dashboard to calculate demand charges and visualize a scatterplot of the amount of sunlight coming into the greenhouse and how much supplemental light is needed. SupplementalCalc is hosted on ShinyApps and is available [here](https://uga-lighting-calc.shinyapps.io/supplementalcalc/).

**Description:** SupplementalCalc was created to determine how much electricity is required to reach the target DLI given what percent of the year the user wants to reach that target and how many hours their lights are on per day. On the Electricity Cost page, users will view a dashboard that calculates lighting costs at an annual, monthly, and weekly view. The page components are dynamic and change to the user's mouse click on the scatterplot, which represents changing the percentile of days. 

**General Skills:** APIs, Data Transformation, Data Analytics, Data Visualization, Interactive Web App Development
**Specific Skills:** R (main libraries: shiny, dyplr, ggplot2, lubridate, tidygeocoder)

#### TargetCalc
**Background:**  

**Description:** 
TargetCalc is hosted on ShinyApps and is available [here](https://uga-lighting-calc.shinyapps.io/TargetCalc/).

**General Skills:** APIs, Data Transformation, Data Analytics, Data Visualization, Web App Development
**Specific Skills:** R (main libraries: shiny, dyplr, ggplot2, lubridate, tidygeocoder)


## Data Analytics Portfolio


## Data Science Portfolio
