# Add Calculated Fields

In the next section, you will learn how to add calculated fields for "day of week" and "hour of day" to your dataset and a new scatter plot for these two dependent variables.

1. Click the Add button on the top left and select Add a calculated field.

    ![screenshot](img/29.png)

2. For Calculated field name type “event_day_of_week".

3. For Formula, type `extract("WD",{event_date_time})`.

    > [!NOTE]
    > extract returns a specified portion of a date value. Requesting a time-related portion of a date that doesn't contain time information returns 0. WD: This returns the day of the week as an integer, with Sunday as 1.

1. Click Create.

    ![screenshot](img/30.png)

    > [!DANGER]
    > If you consistently get the error "The syntax of the calculated field expression is incorrect. Correct the syntax and choose Create again", please refresh the browser and then type manually the expression above.

2. Add another calculated field with the following attributes:

    - Calculated field name: "event_hour_of_day".
    - Formula: `extract("HH",{event_date_time})`.

    > [!NOTE]
    > HH returns the hour portion of the date.

    ![screenshot](img/31.png)

3. Click Add button in the top left and choose Add visual.

    ![screenshot](img/32.png)

4. For field type, select the scatter plot.

5. In the Fields list, select and drag the following attributes to the Field wells pane to set the graph attributes:

    - X-axis: "event_hour_of_day"
    - Y-axis: "event_day_of_week"
    - Size: "ticket_price"

    ![screenshot](img/33.png)
