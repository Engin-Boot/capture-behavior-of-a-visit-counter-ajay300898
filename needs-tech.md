# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given there is backup mechanism
  When server restarts due to some issues
  Then recovery mechanism runs and the visit-counter is set to previous value.

Scenario: Reconcile counts if the sensor is offline for a while

  Given there is reconcile mechanism and it calculates the offline time.
  When the sensor goes offline for a particular amount of time.
  Then the reconcile mechanism runs and it estimates the number of people
       may pass during that time and adds that number to previous count.
