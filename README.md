# School_District_Analysis
## Overview
The purpose of the School District Analysis was to clean, sort, and analyze data from the city school district in order to uncover trends in relation to standardized test scores, school funding, and school size and type. We performed detailed analysis of two csv files, one containing student information and one containing school information, which we then merged. The data we discovered using PANDAS and Jupyter notebook included:
- The top 5 performing schools
- The bottom 5 performing schools
- School performance based on budget
- School performance based on school size
- School performance based on the type of school (District or Charter)

However, the analysis showed evidence of potential academic dishonesty, specifically in one area. So we then performed a second analysis, this time with the 9th graders from Thomas High School's test scores replaced with NaN and we explored how this altered our data.

## Results

### Top 5 performing Schools 

***Original Dataframe:***

![Testing Top Schools](https://user-images.githubusercontent.com/106620821/179420930-e905f03e-e133-4156-a3a4-d4c893e5348a.png)

***Updated Dataframe:***

![Challenge Top Schools](https://user-images.githubusercontent.com/106620821/179420976-bd6d868a-4c71-48c3-877a-2c2546571764.png)

***Analysis***:
After removing the 9th Graders from Thomas High School's math and reading scores, Thomas High School still remained in the top 5 performing schools. However, the average math score dropped from 83.41835 to 83.35094, the average reading score dropped from 83.84893 to 83.89608, and the overall passing % dropped from 90.94801 to 90.63032.

### Bottom 5 Performing Schools

***Original Dataframe:***

![Testing Bottom Schools](https://user-images.githubusercontent.com/106620821/179421231-095e10e2-a408-420c-bed6-f60e2b6cad46.png)

***Updated Dataframe:***

![Challenge Bottom Schools](https://user-images.githubusercontent.com/106620821/179421243-ce51112d-4ee8-48da-a285-41731d829f4e.png)

### School Performance Based on Budget

***Original Dataframe:***

![Testing Spending Ranges](https://user-images.githubusercontent.com/106620821/179421470-341447a3-85ca-4bed-83e8-125cdc069c14.png)

***Updated Dataframe:***

![Challenge Spending Ranges](https://user-images.githubusercontent.com/106620821/179421488-67994346-0656-4b7e-be4f-c61ef94f4091.png)

***Analysis***: The % Passing Reading in the ($631 - $645) range dropped from 84% to 77% after removing the 9th grade reading scores from Thomas High School.

### School Performance Based on School Size

***Original Dataframe:***

![Testing School Size](https://user-images.githubusercontent.com/106620821/179421603-455072be-abc3-4518-90d7-8fefb11c033c.png)

***Updated Dataframe:***

![Challenge School Size](https://user-images.githubusercontent.com/106620821/179421613-18bf173e-a8fc-4371-9bfd-799d2b3fd952.png)

***Analysis***: Here again we see the % Passing Reading in the (Medium school size: 1000-1999) range drop from 97% to 91%.

### School Performance Based on School Type

***Original Dataframe:***

![Testing Final](https://user-images.githubusercontent.com/106620821/179421759-f2cf2586-4472-4d89-8e49-6abd948e3235.png)

***Updated Dataframe:***

![Challenge Final](https://user-images.githubusercontent.com/106620821/179421774-0feeb6b4-b427-4910-9f5c-56fd897d45d2.png)

***Analysis***: Here we discover the overall % Passing Reading for Charter Schools drop from 97% to 93%.

### School Summary

***Original Dataframe:***

![Testing School Summary](https://user-images.githubusercontent.com/106620821/179422585-17983aec-6e92-4b83-8181-aee5435f7ce8.png)

***Updated Dataframe:***

![Challenge School Summary](https://user-images.githubusercontent.com/106620821/179422109-6f50b3f2-e374-4f60-a757-f66b1b816364.png)

***Analysis***: We can see that the % Passing Reading from Thomas High School dropped substantially from 97.30887% to 69.66361%, also leading to a drop in the overall passing % at Thomas High (from 90.94801% to 90.63032%).


## Summary

After analyzing both dataframes, one that included all scores from all grades, and the other that did not include the 9th grade reading scores from Thomas High School, we discovered a few minor changes in the data, and one substantial change in the data for Thomas High School. Thomas High School still remained in the top 5 performing schools. However, the average math score dropped from 83.41835 to 83.35094, the average reading score dropped from 83.84893 to 83.89608, and the overall passing % dropped from 90.94801 to 90.63032. Additionally, the % Passing Reading in the ($631 - $645) spending range dropped from 84% to 77%. We also saw the % Passing Reading in the (Medium school size: 1000-1999) range drop from 97% to 91%, and the overall % Passing Reading for Charter Schools drop from 97% to 93%. What created these changes appears to be the substantial drop in overall % passing reading at Thomas High (from 97.30887% to 69.66361%). 
