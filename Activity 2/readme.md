Activity 2

Create Azure queue, create logic app to process message in queue


Step 1: https://www.atomicax.com/article/how-create-azure-service-bus-queue

Creating a Service Bus
======================

First, go to [https://portal.azure.com](https://portal.azure.com/).

Next, search for Service Bus.

[![](/sites/default/files/2023-01-21_21-09-23.png)](/sites/default/files/2023-01-21_21-09-23.png)

Next, click on create.

[![](/sites/default/files/2023-01-21_21-09-35.png)](/sites/default/files/2023-01-21_21-09-35.png)

Next, fill out all of the required fields giving it a namespace name as well as a pricing tier. Standard pricing tier has lots of features but is very low cost.

[![](/sites/default/files/2023-01-21_21-11-44.png)](/sites/default/files/2023-01-21_21-11-44.png)

Click Next.

[![](/sites/default/files/2023-01-21_21-12-03.png)](/sites/default/files/2023-01-21_21-12-03.png)

Click Next.

[![](/sites/default/files/2023-01-21_21-12-12.png)](/sites/default/files/2023-01-21_21-12-12.png)

Click Next. Note that some organizations may provide defaults values here or you may have to provide some depending on policy.

[![](/sites/default/files/2023-01-21_21-12-20.png)](/sites/default/files/2023-01-21_21-12-20.png)

Click Create.

[![](/sites/default/files/2023-01-21_21-12-33.png)](/sites/default/files/2023-01-21_21-12-33.png)

Wait until the resource deploy then click Go To Resource.

[![](/sites/default/files/2023-01-21_21-16-43.png)](/sites/default/files/2023-01-21_21-16-43.png)

Record the Service bus host name in a safe place. This value will be referred to by other articles. Click on Shared Access Policies.

[![](/sites/default/files/2023-01-21_21-17-00.png)](/sites/default/files/2023-01-21_21-17-00.png)

Click on RootManageSharedAccessKey.

[![](/sites/default/files/2023-01-21_21-29-56.png)](/sites/default/files/2023-01-21_21-29-56.png)

Copy the value in Primary Connect String into a safe place. This value will be referred to by other articles. Close out of the SAS Policy.

[![](/sites/default/files/2023-01-21_21-30-08.png)](/sites/default/files/2023-01-21_21-30-08.png)

Create A Queue
==============

To Create a Queue in your Namespace, click on queues, Then click Queue, then give it a name. Record the name in a safe space. This value will be referred to other articles. Next, click Create.

[![](/sites/default/files/2023-01-21_21-25-32.png)](/sites/default/files/2023-01-21_21-25-32.png)

Your queue should look like this.

[![](/sites/default/files/2023-01-26_21-31-12.png)](/sites/default/files/2023-01-26_21-31-12.png)

Next, go to the [Key vault and create a secret for the service bus connection](https://www.atomicax.com/article/how-create-azure-key-vault-fo) string (Data Point 4).

step 2: https://learn.microsoft.com/en-us/azure/connectors/connectors-create-api-servicebus?tabs=consumption#step-1---check-access-to-service-bus-namespace