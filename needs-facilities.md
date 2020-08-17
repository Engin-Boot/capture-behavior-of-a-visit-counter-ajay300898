# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given Everyone who enters hospital has data entry card with
        there information uploaded and the system able to distinguish
        between different kinds of people enter the hospital and
        notes down the day of entry.
  When system generates report at the end of week
  Then the Facilities Manager able to see number of visitors on
       each day of week in the form of a graph according to the
       categories like all, patients, visitors, doctors etc.

Scenario: Alert when seating capacity is full

  Given There are limited seats and the seats occupied are marked as
        occupied in the system and number of empty seats are updated
        accordingly.
  When there are less than 10 percent seats are free and someone try
       to occupy an empty seat.
  Then an alert is shown that seating capacity is full.
