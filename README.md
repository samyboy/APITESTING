# APITESTING


I wnt to add following feature file in the framework where as I tried to create new step defination for this feature file but as soon as I run the test runner it gives me an error saying duplicate step definition is present. 

Feature: Validating Common Family test (CF2/CF3) cases

Scenario: Verify if the Acums is being successfully added using AddTransactionsAPI in Common family cases
	
	Given Add Accums transaction payload for common family sceanrio from .csv file
	When user calls "AddTransaction" with "Post" http request
	Then API call should be successful with code 200
	And "ServiceStatus" in response  body is "PASS"
