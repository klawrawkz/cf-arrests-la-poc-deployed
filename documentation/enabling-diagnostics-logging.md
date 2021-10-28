# Application Insights Diagnostic Logging In Logic App

If your logic app's creation and deployment settings support using Application Insights, you can optionally enable diagnostics logging and tracing for your logic app. You can do so either when you deploy your logic app from Visual Studio Code or after deployment. You need to have an Application Insights instance, but you can create this resource either in advance, when you deploy your logic app, or after deployment.

To enable logging and tracing now, follow these steps:

Select either an existing Application Insights resource or Create new Application Insights resource.

In the Azure portal, go to your Application Insights resource.

On the resource menu, select Overview. Find and copy the Instrumentation Key value.

In Visual Studio Code, in your project's root folder, open the local.settings.json file.

In the Values object, add the APPINSIGHTS_INSTRUMENTATIONKEY property, and set the value to the instrumentation key, for example:

```json
{
   "IsEncrypted": false,
   "Values": {
      "AzureWebJobsStorage": "UseDevelopmentStorage=true",
      "FUNCTIONS_WORKER_RUNTIME": "dotnet",
      "APPINSIGHTS_INSTRUMENTATIONKEY": <instrumentation-key>
   }
}
```

```markdown
    You can check whether the trigger and action names correctly 
appear in your Application Insights instance.
    
    In the Azure portal, go to your Application Insights resource.
    
    On the resource resource menu, under Investigate, 
select Application map.
    
    Review the operation names that appear in the map.
    
    Some inbound requests from built-in triggers might appear as 
duplicates in the Application Map. Rather than use the 
WorkflowName.ActionName format, these duplicates use the 
workflow name as the operation name and originate from the 
Azure Functions host.
```

There you have it.
