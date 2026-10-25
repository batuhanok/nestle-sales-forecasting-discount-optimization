# Sales Forecasting and Discount Optimization for Nestlé Professional

Industry engineering project with Nestlé Professional on how trade discounts drive sales and which discount level maximizes profit for each product and customer group.

> The code, data and detailed results of this project are covered by a confidentiality agreement with Nestlé. This repository only shares the project summary and the front matter of the report (title pages and table of contents).

## Overview

Nestlé Professional sells to out of home channels where discounts are a major lever, but it was not clear how much extra volume each discount level actually brings. We built a two stage approach that first forecasts how sales respond to discounts and then picks the most profitable discount for every product and customer combination under business constraints.

## What I did

- Led the industry project measuring how sales respond to 41 discount levels (0% to 40%) using 24 months of sales and discount data across 276 products and 19 customer groups
- Cleaned the data and checked outliers with IQR, Z-score and Euclidean distance methods, then compared 4 regression models on R-squared and RMSE and selected the linear-log model to capture diminishing returns
- Formulated a binary integer linear programming model and solved it with Gurobi in Python to recommend the discount level for each of 1,697 product and customer combinations, subject to a 20% minimum unit margin and a discount budget of 15% of revenue, projecting an 11.1% profit increase
- Built the models at three levels of detail (customer group, customer subgroup and individual customer) and verified and validated the results

## Methods and tools

Python, Gurobi, regression analysis (linear, log-linear, linear-log, log-log), outlier detection, binary integer linear programming.

## Files

| File | Description |
|---|---|
| [docs/report-front-matter.pdf](docs/report-front-matter.pdf) | Title pages and table of contents of the final report |

## Team

Batuhan Ok, Beyza Sude Kaymakcı, Melek Melisa Akay, Doğa Güz, Alaz Kurt

ISE 491 and ISE 492 Engineering Project, Yeditepe University, November 2024 to June 2025. Academic advisors Assist. Prof. Dr. Zeynep Özlem Ocak and Prof. Dr. Dilek Tüzün Aksu. Industry coordinators Arif Cihat Dağdelen and Begüm Alıcı from Nestlé Professional.
