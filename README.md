# NO_SHOW_APPOINTMENT-Udacity-Data-Analyst-Nanodegree
This repository contains all effort put into investigate the No_show_appointments dataset.
## Dataset Description
> The dataset was obtained from [kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments) <br/>
> Sometimes, some people do make doctor appointment and refuse to show up even after receiving necessary instructions. Who or what can we blame for this attitude? The No-show appointments dataset contains 110527 obsrvations and 14 features about each patient. The features are
> 1. PatientId: provides identification of a patient.
> 2. AppointmentID: gives the identification of each patient' appointment.
> 3. Gender: a categorical variable that provides the sex of each patient (Male or Female).
> 4. ScheduledDay : provides the actual appointment date.
> 5. AppointmentDay: provides the date an appointment was made.
> 6. Age: provides the age of each patient.
> 7. Neighbourhood: gives info on the appointment location.
> 8. Scholarship: provides True of False info on whether a patient receives financial aid(social welfare) from the government or not
> 9. Hipertension: returns True or False on whether the patient has hypertension or not
> 10. Diabetes: returns True or False on whether the patient has Diabetes or not
> 11. Alcoholism: Provides information on if a patient takes alcohol or not (True or False)
> 12. Handcap: returns True or False on whether a patient is handicapped or not
> 13. SMS_received: provides one or more messages sent to the patient.
> 14. No-show: Gives information on if a patient shows up for the appointment or not. ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.

## Question(s) for Analysis
> 1. What is the correlation or relationship between the numerical variables?
> 2. Does gender affect if a patient will show up or not?
> 3. Does Age determine if a patient will show up for the appointment?
> 4. Does the difference between scheduled_day and appointment_day affect no_show feature?
> 5. Does scholarship affect no_show feature?
> 6. Which nighbourhood has the highest show count and highest no_show count?

## Conclusions
> To answer the first question, there are relationships mostly negative between my feature of interest(no_show) and other features. There are some positive relationship, but I can't make much deduction from the heatmap. The reason for this is because the correlation heatmap cannot do justice to visualizing the relationship between each features of the variables. This is probably because most of the features are categorical.<br/>
> From question 2 'Does gender affect if a patient will show up or not?'. From the bar plot, it is obvious that the difference between the percentage of females to males that did not show up is very small. Therefore, it cannot be declared that gender affect chance of showing up.<br/>
> For question 3, Age did determine if a patient will show up for the appointment. From the plots, it is obvious that age does affect the if a patient will keep appointment or not. <br/>
> Time difference affect the chance of keeping up with appointment. Those with appointment time frame within the day the schedule was made tend to show up that those whose appointment date is far from the day they made the appointment. It may be that they have forgotten that they have an appointment due to the long time lapse.<br/>
>Scholarship does not really affect no ahow rate, althoug, a greater percentage of those with scholarship tend to show up for their appointment<br/>
> People in certain neighbourhood also tend to show up for appointment than others. This may be due to the proximity of their neigbourhood to the hospital.<br/>
>Most of the deductions from this analysis are based on assumptions, a machine learning model can help to provide more accurate deductions and insight.

## Limitation
The Date column(appointment_day and scheduled_day) were in UTC format. My plan was to get the time interval and not days interval, but somehow I could'nt do that as I was getting negative time interval and had to opt for days interval.

## References
https://stackoverflow.com/ <br/>
https://medium.com/ <br/>
https://www.geeksforgeeks.org/ <br/>
https://practicaldatascience.co.uk/ <br/>
https://www.codegrepper.com/ <br/>
https://towardsdatascience.com/
