# ℹ Determining a Promising Tariff for a Telecom Company

Based on data from a mobile operator's customers, analyze customer behavior and search for the optimal tariff.
Data provided by Yandex.Practicum.

# 🛠 Skills & Tools

`Statistical Data Analysis`
`Data Preprocessing`
`matplotlib` `numpy` `pandas` `scipy` `seaborn`

# 💻 Data Description:

** Table `users` (information about users): **
-   `user_id`: unique user identifier
-   `first_name`: user's first name
-   `last_name`: user's last name
-   `age`: user's age (years)
-   `reg_date`: date of tariff activation (day, month, year)
-   `churn_date`: date of discontinuation of using the tariff (if the value is missing, the tariff was still active at the time of data extraction)
-   `city`: user's city of residence
-   `tariff`: name of the tariff plan

** Table `calls` (information about calls): **
-   `id`: unique call identifier
-   `call_date`: date of the call
-   `duration`: call duration in minutes
-   `user_id`: identifier of the user who made the call

** Table `messages` (information about messages): **
-   `id`: unique message identifier
-   `message_date`: date of the message
-   `user_id`: identifier of the user who sent the message

** Table `internet` (information about internet sessions): **
-   `id`: unique session identifier
-   `mb_used`: volume of internet traffic used during the session (in megabytes)
-   `session_date`: date of the internet session
-   `user_id`: identifier of the user

** Table `tariffs` (information about tariffs): **
-   `tariff_name`: tariff name
-   `rub_monthly_fee`: monthly subscription fee in rubles
-   `minutes_included`: number of minutes included in the monthly subscription fee
-   `messages_included`: number of messages included in the monthly subscription fee
-   `mb_per_month_included`: volume of internet traffic included in the monthly subscription fee (in megabytes)
-   `rub_per_minute`: cost of a minute of conversation above the tariff package (for example, if the tariff includes 100 minutes of conversation per month, then a fee will be charged for minutes beyond the 100th)
-   `rub_per_message`: cost of sending a message above the tariff package
-   `rub_per_gb`: cost of an additional gigabyte of internet traffic above the tariff package (1 gigabyte = 1024 megabytes)