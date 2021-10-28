The 'Function' connection defaults to '__Failed__' after logic app depoloyment 

Log Output:
```armasm
Connecting to log stream...
2021-10-28T18:44:33  Welcome, you are now connected to log-streaming service. The default timeout is 2 hours. Change the timeout with the App Setting SCM_LOGSTREAM_TIMEOUT (in seconds). 
2021-10-28T18:44:41.396 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:44:41.396 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:44:41.396 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200

2021-10-28T18:44:42.277 [Debug] Initiating background SyncTriggers operation
2021-10-28T18:44:42.278 [Information] Loading functions metadata
2021-10-28T18:44:42.281 [Debug] Workflow Debug: operationName='WorkflowDefinitionProvider.GetWorkflowDispatcherMetadata', message='Registering the workflow dispatcher metadata function', exception='', extensionVersion='1.0.0.0', siteName='arrestsMonitored', slotName='Production', activityId='30ca30ee-0174-40cb-bb79-02e4c63ae4dd'.
2021-10-28T18:44:42.298 [Error] Workflow Error: operationName='WorkflowDefinitionProvider.GetFunctionMetadataAsync', message='Workflow processing failed, the response exception is 'The 'functionConnections' property in connection.json has a value that cannot be parsed.'', exception='Microsoft.Azure.Workflows.Common.ErrorResponses.ErrorResponseMessageException: The 'functionConnections' property in connection.json has a value that cannot be parsed.
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.GetResolvedFunctionConnections(InsensitiveDictionary`1 functionConnections, InsensitiveDictionary`1 parameters)
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.LoadEdgeConnectionDetails(InsensitiveDictionary`1 parameters)
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.ProcessWorkflowFiles()
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.GetFunctionMetadataAsync()', extensionVersion='1.0.0.0', siteName='arrestsMonitored', slotName='Production', activityId='00000000-0000-0000-0000-000000000000'.
2021-10-28T18:44:41.397 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,3,0,0), AvgCpuLoad=1, MaxCpuLoad=3
2021-10-28T18:44:41.398 [Debug] [HostMonitor] Host aggregate CPU load 1
2021-10-28T18:44:41.398 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:44:42.335 [Information] 0 functions loaded
2021-10-28T18:44:42.336 [Information] Loading functions metadata
2021-10-28T18:44:42.337 [Debug] Workflow Debug: operationName='WorkflowDefinitionProvider.GetWorkflowDispatcherMetadata', message='Registering the workflow dispatcher metadata function', exception='', extensionVersion='1.0.0.0', siteName='arrestsMonitored', slotName='Production', activityId='d8b30e74-73e0-4d6c-9a77-dc804e59fcb6'.
2021-10-28T18:44:42.353 [Error] Workflow Error: operationName='WorkflowDefinitionProvider.GetFunctionMetadataAsync', message='Workflow processing failed, the response exception is 'The 'functionConnections' property in connection.json has a value that cannot be parsed.'', exception='Microsoft.Azure.Workflows.Common.ErrorResponses.ErrorResponseMessageException: The 'functionConnections' property in connection.json has a value that cannot be parsed.
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.GetResolvedFunctionConnections(InsensitiveDictionary`1 functionConnections, InsensitiveDictionary`1 parameters)
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.LoadEdgeConnectionDetails(InsensitiveDictionary`1 parameters)
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.ProcessWorkflowFiles()
   at Microsoft.Azure.Workflows.WebJobs.Extensions.Initialization.WorkflowFunctionDefinitionProvider.GetFunctionMetadataAsync()', extensionVersion='1.0.0.0', siteName='arrestsMonitored', slotName='Production', activityId='00000000-0000-0000-0000-000000000000'.
2021-10-28T18:44:42.403 [Information] 0 functions loaded
2021-10-28T18:44:54.514 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:44:54.528 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:44:54.528 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:44:54.512 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:44:54.512 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:44:54.512 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:07.564 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(3,0,0,0,0), AvgCpuLoad=1, MaxCpuLoad=3
2021-10-28T18:45:07.565 [Debug] [HostMonitor] Host aggregate CPU load 1
2021-10-28T18:45:07.565 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:07.566 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:07.567 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:07.567 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:20.645 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:20.646 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:20.646 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:20.647 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:20.647 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:20.647 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:33.735 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:33.736 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:33.736 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:33.736 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:33.737 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:33.737 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:33.967 [Information] Host Status: {
  "id": "arrestsmonitored",
  "state": "Running",
  "version": "3.3.1.0",
  "versionDetails": "3.3.1 Commit hash: bd2b318013cee8d608c88203ec4ee3516d2a9961",
  "platformVersion": "95.0.7.554",
  "instanceId": "3b1d2929579dc746e8a60d1181e922aa2b44d7f4f1c028d87f5c4d71ed23d871",
  "computerName": "PD0SDWK0000PG",
  "processUptime": 111868
}
2021-10-28T18:45:46.820 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:46.820 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:46.820 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:46.820 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:46.820 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:46.821 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:59.916 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:59.916 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:59.916 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:45:59.918 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:45:59.918 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:45:59.918 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:13.016 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:13.016 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:13.016 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:13.017 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:13.017 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:13.017 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:26.087 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:26.087 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:26.087 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:26.088 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:26.088 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:26.089 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:33.803 [Information] Host Status: {
  "id": "arrestsmonitored",
  "state": "Running",
  "version": "3.3.1.0",
  "versionDetails": "3.3.1 Commit hash: bd2b318013cee8d608c88203ec4ee3516d2a9961",
  "platformVersion": "95.0.7.554",
  "instanceId": "3b1d2929579dc746e8a60d1181e922aa2b44d7f4f1c028d87f5c4d71ed23d871",
  "computerName": "PD0SDWK0000PG",
  "processUptime": 171704
}

2021-10-28T18:46:39.166 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(2,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=2
2021-10-28T18:46:39.166 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:39.167 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:39.167 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:39.167 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:39.167 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:52.248 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:52.248 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:52.249 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:46:52.249 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:46:52.250 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:46:52.250 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:05.325 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:05.325 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:05.325 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:05.326 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:05.326 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:05.327 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:18.419 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:18.419 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:18.419 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:18.417 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:18.417 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:18.417 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:31.511 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:31.511 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:31.511 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:31.509 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:31.509 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:31.509 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:33.739 [Information] Host Status: {
  "id": "arrestsmonitored",
  "state": "Running",
  "version": "3.3.1.0",
  "versionDetails": "3.3.1 Commit hash: bd2b318013cee8d608c88203ec4ee3516d2a9961",
  "platformVersion": "95.0.7.554",
  "instanceId": "3b1d2929579dc746e8a60d1181e922aa2b44d7f4f1c028d87f5c4d71ed23d871",
  "computerName": "PD0SDWK0000PG",
  "processUptime": 231641
}
2021-10-28T18:47:44.573 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:44.573 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:44.574 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:44.575 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:44.575 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:44.576 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:57.647 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:57.648 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:57.648 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:47:57.649 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:47:57.650 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:47:57.650 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:10.743 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:10.744 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:10.744 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:10.745 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:10.746 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:10.746 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:23.833 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:23.834 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:23.834 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:23.834 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:23.834 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:23.834 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:33.724 [Information] Host Status: {
  "id": "arrestsmonitored",
  "state": "Running",
  "version": "3.3.1.0",
  "versionDetails": "3.3.1 Commit hash: bd2b318013cee8d608c88203ec4ee3516d2a9961",
  "platformVersion": "95.0.7.554",
  "instanceId": "3b1d2929579dc746e8a60d1181e922aa2b44d7f4f1c028d87f5c4d71ed23d871",
  "computerName": "PD0SDWK0000PG",
  "processUptime": 291626
}

2021-10-28T18:48:36.926 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:36.926 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:36.927 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:36.929 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:36.930 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:36.930 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:50.016 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:50.017 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:50.017 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:48:50.017 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:48:50.017 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:48:50.017 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:49:03.093 [Debug] [HostMonitor] Host process CPU stats (PID 2660): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:49:03.094 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:49:03.094 [Information] Executing HttpStatusCodeResult, setting HTTP status code 200
2021-10-28T18:49:03.095 [Debug] [HostMonitor] Host process CPU stats (PID 2036): History=(0,0,0,0,0), AvgCpuLoad=0, MaxCpuLoad=0
2021-10-28T18:49:03.096 [Debug] [HostMonitor] Host aggregate CPU load 0
2021-10-28T18:49:03.096 [
```
