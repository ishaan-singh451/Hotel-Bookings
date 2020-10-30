# An Analysis of Hotel Booking Data
## Exploratory Data Analysis
The data set contained multiple columns which were not very useful in the analysis; hence, they were dropped from the data frame. It was then important to check the data types contained in each column of the data frame. This produced the following results.

```python
hotel                              object
lead_time                           int64
arrival_date_month                 object
stays_in_weekend_nights             int64
stays_in_week_nights                int64
adults                              int64
children                          float64
babies                              int64
country                            object
is_repeated_guest                   int64
previous_cancellations              int64
previous_bookings_not_canceled      int64
reserved_room_type                 object
assigned_room_type                 object
booking_changes                     int64
deposit_type                       object
dtype: object
```

The next stage is to analyse the unique values of columns which contain catgeorical or factor data. Beginning with the type of hotel; the unique types of hotels include: _Resort Hotels_ and _City Hotel_. The data set contains data from all twelve months of the year, which would be expected. 177 countries are represented in this data set. The reserved room types are labeled as 'C', 'A', 'D', 'E', 'G', 'F', 'H', 'L', 'P' and 'B'. The assigned room types are of the same kind, but even more numerous in number. Since these labels make very little sense without metadata of some sort (which was not provided with the data set), it is appropriate to drop them from the data frame. Finally, the deposit type of the booking can be: _No Deposit, Refundable, Non Refund_(Non Refundable).

