# Box-Plots for Education: Improving educational equity through transparent financial coding


## Problem Overview
United Stated educational spending falls short of United Nations
Educational, Scientific, and Cultural Organization (UNESCO) global
standards by $16,993 per pupil per year [1] [2]. Within the United
States, these disparities are further exacerbated as the spending gap
between high-income and low-income areas is nearly $1,000 per
pupil per year [3]. Therefore, schools and school districts must
maximize the return on investment on each dollar of their limited
budgets to provide quality education to all students. However, due
to non-uniform financial coding and irregular reporting, there is
little opportunity to analyze the direct educational impact of budget
allocations across schools and school districts. 

Educational Resource Strategies (ERS) is a national non-profit working to promote educational equity and transform how schools analyze and allocate their resources by easing this cross-district budget comparison [5]. ERS has developed a comprehensive financial spending framework, codifying schools budget line items by what the spending "is" (e.g; "benefits", "property rental") and what the spending "does" (e.g; "special education", "substitute compensation") [4]. This coding scheme promotes educational equity by providing schools the ability to analyze their spending with respect to other schools and other districts. When combined with additional data on teaching and learning, this provides rich insight into how allocation of funds impacts student outcomes across the United States. 

##  Solution Framework

This financial coding is both time and resource intensive. The goal of this project is to apply machine learning concepts to automate this process. Specifically, the goal is to construct a multi-class-multi-label classification problem to attach canonical labels to the freeform text in budget line items. These labels let ERS understand how schools are spending money and tailor their strategy recommendations to improve outcomes for students, teachers, and administrators[4].

## Solution Summary
The team combined all text columns into a single text feature per instance. This text feature was then vectorized using TF-IDF. A simple logistic regression classifier was applied to the resultant vector. This approach classifies labels with a multi-class-multi-label loss of 0.4934 and over 91% accuracy.

## Authors 

Jin-sol Jung, Jackson Livanec, Danny Mathieson

## License
Creative Commons

## References
1. U.S. Census Bureau. 2020. Annual Survey of School System Finances. https: //www.census.gov/programs-surveys/school-finances.html
 
2. Melanie Hanson. 2022. U.S. Public Education Spending Statistics. https:// educationdata.org/public- education- spending- statistics

3. American University School of Education. 2020. Inequality in Public School Funding: Key Issues Solutions for Closing the Gap. https://soeonline.american. edu/blog/inequality- in- public- school- funding/

4. Driven Data. 2020. Reboot: Box-Plots for Education. Code Repository. https://github.com/drivendataorg/box-plots-for-education

5. Educational Resource Strategies. 2022. ERS, Who We Are. https://www. erstrategies.org/info/who_we_are

