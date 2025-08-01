# land-grants-performance-tests

This is the performance test suite for grants-ui and land-grants-api application journeys maintained by Land grants team.

## grants-ui(find-funding-for-land-or-farms) performance tests:
There are tests for grants-ui(find-funding-for-land-or-farms) end-to-end application submission journey that:
- Runs for 60 seconds
- Ramps up to 10 threads
- Asserts that all requests receive an HTTP 200 Ok response
- Asserts that the average response time is under 3000 ms
- Asserts that no single response is greater that 3000 ms

## land-grants-api performance tests:
There is a single test for land-grants-api that:
- Runs for 60 seconds
- Ramps up to 10 threads
- Asserts that all requests receive an HTTP 200 Ok response
- Asserts that the average response time is under 3000 ms
- Asserts that no single response is greater that 3000 ms

## Running locally

Use JMeter GUI. Set the `Server Name` in `HTTP Request Defaults` to an instance of service `land-grants`, either hosted or local, and use JMeter to run the test. 

## Running on CDP Portal

The performance test suites are designed to be run from the CDP Portal.
The CDP Platform runs test suites in much the same way it runs any other service, it takes a docker image and runs it as an ECS task, automatically provisioning infrastructure as required.

## Licence

THIS INFORMATION IS LICENSED UNDER THE CONDITIONS OF THE OPEN GOVERNMENT LICENCE found at:

<http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3>

The following attribution statement MUST be cited in your products and applications when using this information.

> Contains public sector information licensed under the Open Government licence v3

### About the licence

The Open Government Licence (OGL) was developed by the Controller of Her Majesty's Stationery Office (HMSO) to enable
information providers in the public sector to license the use and re-use of their information under a common open
licence.

It is designed to encourage use and re-use of information freely and flexibly, with only a few conditions.
