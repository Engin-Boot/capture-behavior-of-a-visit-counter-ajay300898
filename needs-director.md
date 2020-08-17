# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given Everyone who enters hospital has data entry card with
        there information uploaded and the system able to distinguish
        between different kinds of people enter the hospital and
        notes down the day of entry.
  When The system generates the report of patient visits
       during working days and holidays
  Then the software shows number of patients visited on working days
       and holidays in a pie chart and provides facility to check
       results for individual patient and also gives option to choose
       the dates from and to, to calculate the results.

Scenario: Compute parking slots to reserve for visiting specialists

  Given There is a facility to identify specialists by scanning there
        vehicle tag at the entrance and the parking slot reservation
        system works fine and there is always some empty slots for
        parking.
  When specialists vehicle is recognised at the entrance and it reached
       parking area
  Then the system automatically reserves a parking slot which is nearer
       to exit and the location to be parked is sent to both the system
       in parking area and the specialist.
