from datetime import date
import calendar
dob=input("Enter your date of birth(DD/MM/YYYY):")
bd,bm,by=map(int,dob.split('/'))

today=date.today()
cd=today.day
cm=today.month
cy=today.year

#initial difference
year=cy-by
month=cm-bm
day=cd-bd

if day<0:
    month-=1
    if today.month==1:
        prev_month=12
        prev_year=today.year-1
    else:
        prev_month=today.month-1
        prev_year=today.year
    days_in_prev_month=calendar.monthrange(prev_year,prev_month)[1]
    day+=days_in_prev_month
if month<0:
    year-=1
    month+=12


print(f"your age is:{year} years,{month} months,{day} days")
