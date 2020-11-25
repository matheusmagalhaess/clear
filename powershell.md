TCP: 

    Get-Process -Id (Get-NetTCPConnection -LocalPort YourPortNumberHere).OwningProcess

UDP:

    Get-Process -Id (Get-NetUDPEndpoint -LocalPort YourPortNumberHere).OwningProcess
