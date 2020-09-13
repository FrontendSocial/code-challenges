Think about an events calendar component which needs to show events using minimum number of rows. The calendar needs to show an event beside other events if there is available space. If the duration of the event overlaps with other events and there is no available space to show the entire event in that row, only then the event should be added to the next row in the calendar. This will allow to show events in calendar with minimum vertical space thereby avoiding a vertical scroll bar in the calendar view.

#
Write a JavaScript method `showEventsSideBySide(calendarEvents) {}` that will take the following array as input and return the output array as given below. 

#
Winner of this challenge will be decided by accuracy of the algorithm to pass all edge cases and in efficiency of execution.

## input
```
const calendarEvents = [
    { id: 1, title: 'Event 1', startDate: '2020-08-10', endDate: '2020-08-15'},
    { id: 2, title: 'Event 2', startDate: '2020-08-26', endDate: '2020-08-28'},
    { id: 3, title: 'Event 3', startDate: '2020-08-12', endDate: '2020-09-17'},
    { id: 4, title: 'Event 4', startDate: '2020-08-16', endDate: '2020-08-20'},
    { id: 5, title: 'Event 5', startDate: '2020-09-03', endDate: '2020-09-05'},
    { id: 6, title: 'Event 6', startDate: '2020-08-31', endDate: '2020-09-03'}
]
```

![Input](https://raw.githubusercontent.com/FrontendSocial/code-challenges/master/01-events-calendar/input.png)


## output
```
{
    totalEvents: 6,
    rows: [
      [    
        { id: 1, title: 'Event 1', startDate: '2020-08-10', endDate: '2020-08-15'},
        { id: 4, title: 'Event 4', startDate: '2020-08-16', endDate: '2020-08-20'},
        { id: 2, title: 'Event 2', startDate: '2020-08-26', endDate: '2020-08-28'},
        { id: 5, title: 'Event 5', startDate: '2020-09-03', endDate: '2020-09-05'}
      ],
      [
        { id: 3, title: 'Event 3', startDate: '2020-08-12', endDate: '2020-09-17'},
        { id: 6, title: 'Event 6', startDate: '2020-08-31', endDate: '2020-09-03'}
      ]
    ]
}
```

![Output](https://raw.githubusercontent.com/FrontendSocial/code-challenges/master/01-events-calendar/output.png)
