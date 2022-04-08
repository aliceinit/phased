# phased
A python framework for reliable e2e-testing and monitoring of systems using multi-phase tests 

## Running in 'test' mode
In your project directory, run: `phased test`

All tests will execute each phase once, as requirements are met, and will stop running once the final phase has completed. It will also stop running if it hits a failure state instead of completing.

## Running in 'monitor' mode
In your project directory, run: `phased monitor`

Once each test completes it starts again at the first phase and continues indefinitely. Tests with different schedules or # of steps will cycle independently at their own pace. 

If a test fails (and no retries or recovery steps are configured), it will start again at the first phase.
