### Create new domain cycle:
* First, call the `DomainController::store` function to store the domain information in the central database, 
and the following is an explanation of the creation process.
    - Check ftp by `DomainOperationController::checkFtp` function and database connection by `DomainOperationController::checkDB` function.
    - Store domain information.
    - Complete the rest of construction into `DomainOperationController::createNewWebsite` function.
* Within `DomainOperationController::createNewWebsite` function The index file is uploaded and then the rest of the processes are inside `DomainOperationController::RemainingCreateNewWebsiteOperations`.
* Within `DomainOperationController::RemainingCreateNewWebsiteOperations` The rest of the files are uploaded.
* When all files are uploaded, the new domain is created and redirect to it.

  
### Edit domain:
* First, call `DomainController::update` function that check database connection and call `DomainOperationController::editWebsite`.
* Within `DomainOperationController::editWebsite` function, the site's modules are modified by addition and deletion.

### Delete domain:
* When you delete a domain, it is deleted from the central database and sent to the trash or delete it completely.
* The actual site and files are not deleted.



