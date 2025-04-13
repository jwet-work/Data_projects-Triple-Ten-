# Cohort Analysis 
This project required a review of the raw user data from the store's website which pulled:<br> *user_id<br>*event_type	<br>*category_code	<br>*brand	price	<br>*event_date over the span of several months. We then had to:
1) Create a conversion funnel counting unique users at each of the 3 stages of the funnel. From this, we then added total conversion rates and conversion rates to the data pull. A copy was made from the raw file to make a working version of the raw data which was kept in tact from the original pull. ![image](https://github.com/user-attachments/assets/2b225378-d622-47d4-9c00-9512c3c4c917)

   
2) Build acquisition cohorts based on the month of a user’s first purchase, and track cohort metrics month by month. To do this we create a new blank sheet tab called “purchase_activity.” Then, using the filters in the “raw_user_activity” sheet, we selected only event types that are purchases. After applying the filter, we copied the entire sheet and paste the data into the “purchase_activity” sheet. ![image](https://github.com/user-attachments/assets/3d5e87d7-8743-45d8-9475-43c481a1d3ce)

   
With purchase activity isolated in its own table, we were able to calculate the first purchase date for each user who made a purchase.Using the “purchase_activity” sheet data, we inserted a pivot table as a new sheet called “first_purchase”. Then we configured the settings of the pivot table to calculate the minimum event_date for each user. Finally, for this step, first purchase dates were transferred to a new column in the purchase activity data.  This data was used to determine each user's cohort age by month ![image](https://github.com/user-attachments/assets/ff75a004-ebb5-4e49-99d1-fc09b01a96cf)


3) Aggregate the purchase data into cohorts and then calculate retention rates for each cohort month by month. To do this, we grouped the data into cohorts, creating a pivot table from purchase activity. ![image](https://github.com/user-attachments/assets/ff2cc8e5-40f3-4f0b-a084-367f7be5ed91)

This then allowed us to calculate the overall retention rates month by month, by age ![image](https://github.com/user-attachments/assets/cda921c9-3774-444f-96d0-01ba296bf057)



