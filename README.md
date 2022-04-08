# phased
A python framework for testing and monitoring with multi-phase test steps

## Running in test mode
In your project directory, run: `phased test`

All tests will execute each phase once, as requirements are met, and will stop running once the final phase has completed.

## Running multi-phase monitoring
In your project directory, run: `phased monitor`

Once each test completes it starts again at the first phase and continues indefinitely. Tests with different schedules or # of steps will cycle independently at their own pace. 
