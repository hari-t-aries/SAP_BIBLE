**==> picture [596 x 420] intentionally omitted <==**

User Guide | PUBLIC Document Version: 1.0 – 2021-09-03 

## **OData Client for Service Layer** 

**==> picture [58 x 29] intentionally omitted <==**

**THE BEST RUN** 

## **Content** 

|**1**|**Introduction. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5**|
|---|---|
|**2**|**Environment Setup. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .6**|
|**3**|**Getting Started with OData Context. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12**|
|3.1|Implementing OData Context. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .12|
|3.2|Using OData Context. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .14|
|**4**|**Authentication. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15**|
|4.1|Login. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15|
|4.2|Logout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .16|
|**5**|**Basic CRUD Operations. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .18**|
|5.1|Creating an Entity. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 18|
|5.2|Retrieving an Entity Set. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19|
|5.3|Retrieve an Individual Entity. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .19|
|5.4|Updating an Entity. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 20|
|5.5|Deleting an Entity. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 21|
|**6**|**Query Options. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22**|
|6.1|LINQ Query Methods. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22|
|6.2|AddQueryOption Method. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .25|
|**7**|**Navigation. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 26**|
|7.1|Eager Loading. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 26|
|7.2|Explicit Loading. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27|
|**8**|**Pagination. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 28**|
|8.1|Server-Driven Paging. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 28|
|8.2|Client-Driven Paging. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .29|
|**9**|**Batch Operations. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 30**|
|9.1|Batch Query. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .30|
|9.2|Batch Modifcation. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 32|
||Update. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .32|
||Create. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 34|
||Delete. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .36|
|**10**|**User-Defned Field (UDF). . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39**|
|10.1|OpenType. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39|



OData Client for Service Layer **Content** 

**2** PUBLIC 

|10.2|Dynamic Properties. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39|
|---|---|
|10.3|UDF Operations. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 40|
|**11**|**User-Defned Object (UDO)/User-Defned Table (UDT). . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 42**|
|**12**|**Function and Action. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44**|
|12.1|Function. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44|
|12.2|Action. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 45|
|**13**|**Stream. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48**|
|13.1|Uploading Images and Texts. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 48|
|13.2|Downloading Images and Texts. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 50|



OData Client for Service Layer **Content** 

PUBLIC 

**3** 

## **Document History** 

The following table provides an overview of the most important document changes. 

|Version|Date|Description|
|---|---|---|
|1.0|2021-09-03|First version|



OData Client for Service Layer **Document History** 

**4** PUBLIC 

## **1 Introduction** 

As of SAP Business One 10.0 FP 2108, Service Layer OData v3 and WCF Data Services Client for OData v1-3 are being deprecated. Accordingly, Service Layer OData v4 will become the preferred option. As an alternative to the WCF Data Services Client, a new OData Client for .Net will be introduced and strongly recommended to customers and partners. 

Acting as a .Net library, this client provides the LINQ-enabled client API for issuing OData queries and consuming OData JSON payloads, and allows you to consume data from and interact with OData services from .Net apps effectively and efficiently. 

In this tutorial we are going to focus on the latter approach, and will walk you through how to connect the Service Layer with this OData client library via OData V4. To have a better understanding of this tutorial, you can download the source code from here. 

OData Client for Service Layer **Introduction** 

PUBLIC 

**5** 

## **2 Environment Setup** 

## **Install .NET Core 2.1** 

Because the project you are going to create depends on .NET Core 2.1 SDK, you need to install it beforehand. You can find the Windows x64 Installer here . 

## **Install Microsoft OData Client** 

The OData client package needs to be installed to interact with the Service Layer. One approach to install it is by using the following command line: 

```
> dotnet add package Microsoft.OData.Client --version 7.9.0
```

For other installation approaches, please see https://www.nuget.org/packages/Microsoft.OData.Client/ . 

## **Service Layer for SAP Business One 10.0 FP 2108** 

As of SAP Business One 10.0 FP 2108, the Service Layer is able to work with this OData client in OData V4. 

## **OData Connected Service** 

The `OData Connected Service` is a Visual Studio extension that generates strongly-type C# client code for an OData service. This extension, acting as a code generation tool, is used to generate a client proxy file for an OData service. It makes use of the OData schema in the metadata to generate the proxy classes, which are not only able to shield the client from the complexities involved in invoking the OData web service, but also contain all the methods and objects exposed by the OData web service. 

In this tutorial we are going to use it to create a client for the Service Layer in the following steps: 

1. Open Visual Studio 2017 and create a new C# .Net Core project `ODataClient4ServiceLayer` . 

2. Go to the _Extensions_ menu, click _Manage Extensions_ , search online for **`OData Connected Service`** and install it. 

OData Client for Service Layer **Environment Setup** 

**6** PUBLIC 

**==> picture [438 x 303] intentionally omitted <==**

3. Restart your Visual Studio to complete the installation. 

4. Right-click your project in the Solution Explorer, from the context menu, click _Add_ and _Connected Service_ . 

OData Client for Service Layer **Environment Setup** 

PUBLIC **7** 

**==> picture [438 x 339] intentionally omitted <==**

5. In the popup _Connected Services_ window, select _OData Connected Service_ to start a wizard where you can configure settings for the service you want to connect to. 

**==> picture [438 x 198] intentionally omitted <==**

6. In the _Configure Endpoint_ window, find the _Service Name_ field, enter **`ServiceLayer`** as the service name. In the _Address_ field, ideally we should enter the URL of the OData V4 metadata endpoint (for example, `https://servicelayerhost/b1s/v2/$metadata` ) . However, this would result in a failure as the Service Layer's metadata needs to be authenticated in order to be accessible (For legacy reasons, the Service layer takes /b1s/v2 as an OData V4 endpoint. Please do not be confused by /b1s/v2). 

OData Client for Service Layer **Environment Setup** 

**8** 

PUBLIC 

To work around this issue, it is suggested that you login to the Service Layer to get the metadata in advance using Postman or other tools, and save it to your local machine, then specify the local metadata location (for example, `C:\Users\Administrators\Documents\metadata.xml` ) in the _Address_ field. 

**==> picture [438 x 300] intentionally omitted <==**

7. On the _Schema Types_ page, accept the default selection. 

OData Client for Service Layer **Environment Setup** 

PUBLIC 

**9** 

**==> picture [438 x 300] intentionally omitted <==**

8. Next, go to the _Function/Action Imports_ page and accept the default selection. 

**==> picture [438 x 300] intentionally omitted <==**

9. Next let's choose a name for the file to be generated. For this example, let's stick with the default "Reference". The advanced settings allow you to configure attributes such as custom namespace, and 

OData Client for Service Layer **Environment Setup** 

**10** PUBLIC 

whether to hide generated classes from external assemblies, etc, but for now, let's stick with the default settings. Click _Finish_ to complete the configuration and generate the client code. 

**==> picture [438 x 300] intentionally omitted <==**

10. Upon successful completion, you should see a _Connected Services_ section under your project in the Solution Explorer. Below this section, you will see a folder for the Service Layer which contains the generated `Reference.cs` file containing the generated C# client code corresponding to your specific OData service . 

**==> picture [276 x 212] intentionally omitted <==**

In this tutorial you have learned how to use the OData Connected Service to generate client code. To learn more about using the client to read and write to the service, check out the following tutorials. 

OData Client for Service Layer **Environment Setup** 

PUBLIC 

**11** 

## **3 Getting Started with OData Context** 

For this library, constructing an OData context is the prerequisite for any OData operations, so let's get started with this OData context. 

## **3.1 Implementing OData Context** 

Derived from `Microsoft.OData.Client.DataServiceContext` , `ServiceLayer` is defined as a partial class in the generated namespace `SAPB1` in `Reference.cs` , acting as an OData context for the OData client to interact with the Service Layer. 

To better adapt to the Service Layer, we cannot use this default OData context implementation and need to extend this partial class for the following specific considerations. 

- By default, the Service Layer provides an HTTPS service. This OData client needs to verify the certificate before the connection is established. In this case, for simplicity, most times especially in the development environment we need to customize the certificate verification logic by accepting self-signed certificates or accepting any certificate. 

- The Service Layer makes use of cookie mechanisms for authentication. This requires the client side to save the cookie on a successful login and send the cookie for subsequent requests. To deal with the cookie in a handy manner, we can customize the request building function `BuildingRequest` and response receiving function `ReceivingResponse` . 

Have a look at the generated classes in `Reference.cs` ; you will notice there is a partial function defined in class `ServiceLayer` as below: 

```
partial void OnContextCreated();
```

which is a perfect place to hold our own context initialization logic. We can create a new file named `ServiceLayer.cs` to hold our partial implementation. It should look like this: 

```
using System.Net;
 using System.Net.Security;
using System.Security.Cryptography.X509Certificates;
// The generated classes are defined in this namespace.
namespace SAPB1
{
    // ServiceLayer is defined as a partial class in the generated classes. Here
we add our own implementation.
    public partial class ServiceLayer
    {
        // Save the cookie in the client side.
        private string m_strCookie = "";
        // An empty implementation for certificate verification.
        private static bool TLSCertificateValidate(object sender,
            X509Certificate cert,
            X509Chain chain,
            SslPolicyErrors ssl)
        {
```

OData Client for Service Layer **Getting Started with OData Context** 

**12** PUBLIC 

```
            return true;
        }
        // Override this function to customize some logic to for the
ServiceLayer context.
        partial void OnContextCreated()
        {
            InitializeContext();
        }
        private void InitializeContext()
        {
            // Get the cookie if the response header containing Set-Cookie.
            this.ReceivingResponse += (sender, eventArgs) =>
            {
                string cookie = eventArgs.ResponseMessage.GetHeader("Set-
Cookie");
                if (!string.IsNullOrEmpty(cookie))
                {
                    if (eventArgs.ResponseMessage.StatusCode ==
(int)HttpStatusCode.OK)
                    {
                        m_strCookie = cookie;
                    }
                }
            };
            // Set the cookie for each request.
            this.BuildingRequest += (sender, eventArgs) =>
            {
                if (m_strCookie != null)
                {
                    eventArgs.Headers.Remove("cookie");
                    eventArgs.Headers.Add("cookie", m_strCookie);
                }
            };
            // Ignore the SSL/TLS certificate check for the HTTPS connection to
Service Layer.
            ServicePointManager.ServerCertificateValidationCallback =
TLSCertificateValidate;
        }
    }
 }
```

OData Client for Service Layer **Getting Started with OData Context** 

PUBLIC **13** 

Now the Solution Explorer looks like this: 

**==> picture [271 x 267] intentionally omitted <==**

## **3.2 Using OData Context** 

Let's return to the `Program.cs` and invoke the Login and Logout . Now open your `Program.cs` file and add the following `using` statement: 

```
// The generated classes are defined in this namespace.
 using SAPB1;
```

By default, the OData Connected Service generates the relevant classes in the same namespace defined in the OData metadata document. In this case it is `SAPB1` . 

Assuming we have a running Service Layer, let's create an OData context for the Service Layer by passing the Service Layer URI in the following way. 

```
ServiceLayer slContext = new ServiceLayer(new Uri(ServiceLayerURI));
```

With this context, we can invoke the Service Layer API by passing this context. 

OData Client for Service Layer 

**Getting Started with OData Context** 

**14** PUBLIC 

## **4 Authentication** 

With an existing OData context, we can perform various operations, including Login, Logout and CRUD manipulations on business objects. To separate these operations, let's create a `src` folder, in this folder create a file `Authentication.cs` to implement `Login` and `Logout` . 

Now the Solution Explorer looks like this: 

**==> picture [274 x 288] intentionally omitted <==**

## **4.1 Login** 

Login is an OData action and is implemented as a method in the `ServiceLayer` class, which can be directly invoked in the following way. 

```
public static void Login(ServiceLayer slContext,
     string CompanyDB,
    string UserName,
    string Password,
    string language)
{
    B1Session session = slContext.Login(CompanyDB, UserName, Password,
language).GetValue();
    Console.WriteLine("SessionId={0}, Version={1}", session.SessionId,
session.Version);
```

OData Client for Service Layer **Authentication** 

PUBLIC 

**15** 

```
 }
```

Upon success, the Service Layer returns an entity `B1Session` with a valid session Id in the response body. In the meantime, you can also find the session Id in the `'Set-Cookie'` response header. With this cookie, the client is able to interact with the Service Layer to access resources. 

## **4.2 Logout** 

Likewise, Logout is an OData action as well and it is implemented as a method in the `ServiceLayer` class, which can be directly invoked in the following way. 

```
public static void Logout(ServiceLayer slContext)
 {
    OperationResponse operationResponse = slContext.Logout().Execute();
    Console.WriteLine("Logout code = {0}", operationResponse.StatusCode);
 }
```

Upon success, the Service Layer invalidates the session Id by resetting the `'Set-Cookie'` in the response header. As a result, the client is not able to interact with the Service Layer to access further resources. 

The entire code snippet of `Authentication.cs` is as follows: 

```
using System;
 using System.Threading.Tasks;
using Microsoft.OData.Client;
// The generated classes are defined in this namespace.
using SAPB1;
namespace ODataClient4ServiceLayer
{
    class Authentication
    {
        public static void Login(ServiceLayer slContext,
            string CompanyDB,
            string UserName,
            string Password,
            string language)
        {
            B1Session session = slContext.Login(CompanyDB, UserName, Password,
language).GetValue();
            Console.WriteLine("SessionId={0}, Version={1}", session.SessionId,
session.Version);
        }
        public static void Logout(ServiceLayer slContext)
        {
            OperationResponse operationResponse = slContext.Logout().Execute();
            Console.WriteLine("Logout code = {0}", operationResponse.StatusCode);
        }
      }
    }
 }
```

Assume we have an available company and its credentials, and with this context, we can invoke the Login and Logout by passing this context. Now the entire code snippet of `Program.cs` is like below: 

```
using System;
 using System.Collections.Generic;
using System.IO;
```

OData Client for Service Layer **Authentication** 

**16** 

PUBLIC 

```
using System.Threading.Tasks;
using Microsoft.OData;
using Microsoft.OData.Client;
// The generated classes are defined in this namespace.
using SAPB1;
namespace ODataClient4ServiceLayer
{
    class Program
    {
        // Replace the <servicelayerhost> with your service layer host
        static string ServiceLayerURL = "https://
<servicelayerhost>:50000/b1s/v2/";
        static string CompanyDB = "<your schema name>";
        static string UserName = "<your user name>";
        static string Password = "<your password>";
        // We use the default language code.
        static string Language = "3";
        static void Main(string[] args)
        {
            try
            {
                ServiceLayer slContext = new ServiceLayer(new
Uri(ServiceLayerURL));
                Authentication.Login(slContext, CompanyDB, UserName, Password,
Language);
                Authentication.Logout(slContext);
            }
            catch (Exception ex)
            {
                // Client level Exception message
                Console.WriteLine(ex.Message);
                // The InnerException of Exception contains
DataServiceQueryException
                DataServiceQueryException dataServiceQueryException =
ex.InnerException as DataServiceQueryException;
                if (dataServiceQueryException != null)
                {
                    // The InnerException of DataServiceQueryException contains
DataServiceClientException
                    DataServiceClientException dataServiceClientException =
                        dataServiceQueryException.InnerException as
DataServiceClientException;
                    if (dataServiceClientException != null)
                    {
                        // The InnerException of DataServiceClientException
contains ODataErrorException.
                        // You can get ODataErrorException from
dataServiceClientException.InnerException
                        // This object holds Exception as thrown from the
service.
                        ODataErrorException odataErrorException =
                            dataServiceClientException.InnerException as
ODataErrorException;
                        Console.WriteLine(odataErrorException.Error.ToString());
                    }
                }
            }
        }
    }
 }
```

In case an exception occurs in the Service Layer call, we need to handle the potential exceptions as above. 

OData Client for Service Layer **Authentication** 

PUBLIC **17** 

## **5 Basic CRUD Operations** 

Let's take Items as an example to illustrate how to do the CRUD operations on the business objects using the generated classes and an initialized OData context `slContext` for the Service Layer. 

To encapsulate these operations, in this `src` folder, create a file `ItemsTest.cs` to implement the CRUD operations. 

Now the Solution Explorer looks like this: 

**==> picture [244 x 285] intentionally omitted <==**

## **5.1 Creating an Entity** 

```
//Create an Item and add it to the OData context.
 Item item = new Item();
item.ItemCode = "yourItemCode"; // Specify the item code you want to create.
slContext.AddToItems(item);
// Send the request
DataServiceResponse responses = slContext.SaveChanges();
// Get the responses. For this case, there is only one response.
foreach (OperationResponse response in responses)
{
    var changeResponse = response as ChangeOperationResponse;
    var entityDescriptor = changeResponse.Descriptor as EntityDescriptor;
```

OData Client for Service Layer **Basic CRUD Operations** 

**18** 

PUBLIC 

```
    // Get the entity created on the service and check if the entity is as
expected.
```

```
    Item entity = entityDescriptor.Entity as Item;
```

```
    Console.WriteLine("Expected ItemCode={0}, Actual ItemCode={1}", m_itemCode,
entity.ItemCode);
```

```
    // Check if the response code is as expected.
    Console.WriteLine("Expected StatusCode={0}, Actual StatusCode={1}",
(int)HttpStatusCode.Created, response.StatusCode);
 }
```

By capturing the request, you see that all the properties of the entity are sent to the server. Most properties are null, and these null properties are not actually needed, and in some cases would cause unexpected error. To address this issue, a function FilterNullValues that fwill ilter out the null values needs to be defined and applied to the request pipe line as below: 

```
// Filter out the null properties for some cases like entity creation.
 this.Configurations.RequestPipeline.OnEntryStarting((arg) =>
{
    arg.Entry.Properties = FilterNullValues(arg.Entry);
 });
```

Due to the complexity of this function, we will not go into too much detail here. You can find its implementation in `ServiceLayer.cs` . 

## **5.2 Retrieving an Entity Set** 

```
IEnumerable<Item> items = slContext.Items.Execute();
 foreach (var item in items)
{//Add your business logic.
 }
```

The `Execute()` API call will return an `IEnumerable<Item>` . 

## **5.3 Retrieve an Individual Entity** 

The OData client provides several ways to retrieve an individual entity: 

- Use the `Where()` with `First()` or `Single()` API call. 

```
var item = slContext.Items.Where(c => c.ItemCode == "yourItemCode").First();
 var item = slContext.Items.Where(c => c.ItemCode == "yourItemCode").Single();
```

##  Note 

`First()` will return one object, even if the lambda expression matches multiple objects. `Single()` always returns one object and will throw an exception if the lambda expression matches multiple objects. 

Both `First()` and `Single()` will throw exceptions if no Item with ItemCode as yourItemCode exists. 

OData Client for Service Layer **Basic CRUD Operations** 

PUBLIC 

**19** 

- Use the `ByKey()` API 

```
var item = slContext.Items.ByKey(itemCode: m_itemCode).GetValue();
```

## **5.4 Updating an Entity** 

```
// Get an entity
 var items = new DataServiceCollection<Item>(slContext.Items.Where(p =>
p.ItemCode == "yourItemCode"));
// Change its property
items[0].ItemName = "New name";
// Send the request
DataServiceResponse responses = slContext.SaveChanges();
// Get the responses. For this case, there is only one response.
foreach (OperationResponse response in responses)
{
    Console.WriteLine("Expected StatusCode={0}, Actual StatusCode={1}",
(int)HttpStatusCode.NoContent, response.StatusCode);
 }
```

Please note that the request is not sent until you call the `SaveChanges()` API. The `context` will track all the changes you make to the entities attached to it and will send requests for the changes when `SaveChanges` is called. 

The sample above will send a `PATCH` request to the service in which the body is the whole Item containing properties that are unchanged. This is therefore deprecated and we should look for an alternative approach. 

Fortunately, there is also a second way to track the changes on the property level to only send the changed properties in a `PATCH` request in the following way: 

```
// Get an entity
 var item = slContext.Items.ByKey(itemCode: "yourItemCode").GetValue();
// Change its property
item.ItemName = "New name2";
// Create an update request
slContext.UpdateObject(item);
// Send the request
DataServiceResponse responses = slContext.SaveChanges();
// Get the responses. For this case, there is only one response.
foreach (OperationResponse response in responses)
{
    Console.WriteLine("Expected StatusCode={0}, Actual StatusCode={1}",
(int)HttpStatusCode.NoContent, response.StatusCode);
 }
```

The second way is strongly recommended, because it follows the `PATCH` semantics, and is also beneficial for the performance in the meantime. 

OData Client for Service Layer **Basic CRUD Operations** 

**20** PUBLIC 

## **5.5 Deleting an Entity** 

```
Item item = slContext.Items.ByKey(itemCode: "yourItemCode").GetValue();
 // Create a delete request
slContext.DeleteObject(item);
// Send the request
DataServiceResponse responses = slContext.SaveChanges();
// Get the responses. For this case, there is only one response.
foreach (OperationResponse response in responses)
{
    Console.WriteLine("Expected StatusCode={0}, Actual StatusCode={1}",
(int)HttpStatusCode.NoContent, response.StatusCode);
 }
```

Upon success, the Service Layer returns the status code 204, indicating `No Content` in the response body. 

OData Client for Service Layer **Basic CRUD Operations** 

PUBLIC **21** 

## **6 Query Options** 

There are two main ways to add Query Options to a `DataServiceQuery` . 

- Using strongly typed C# LINQ query methods. 

- Using the `AddQueryOption` method. 

## **Related Information** 

LINQ Query Methods [page 22] AddQueryOption Method [page 25] 

## **6.1 LINQ Query Methods** 

In the example below we are creating a Linq query expression that only returns Items with ItemsGroupCode = 100, ordered by ItemName. We skip the first result, get the top 2 records, and then specify which columns should be returned. 

```
// GET /b1s/v2/Items?$filter=ItemsGroupCode eq 100&$orderby=ItemName
desc&$skip=1&$top=2&$select=ItemName,ItemCode,ItemsGroupCode,ItemType HTTP/1.1
 var query = slContext.Items.Where(p => p.ItemsGroupCode == 100)
    .OrderByDescending(p => p.ItemName)
    .Skip(1)
    .Take(2)
    .Select(p => new { p.ItemName, p.ItemCode, p.ItemsGroupCode, p.ItemType });
foreach (var item in query)
{
    Console.WriteLine($"ItemName: {item.ItemName} ItemCode: {item.ItemCode}
ItemsGroupCode: {item.ItemsGroupCode}");
 }
```

Since the DataServiceQuery class implements the IQueryable interface (System.Linq), the OData client library is able to translate Linq queries against entity sets into URIs executed against a data service resource. 

The examples below demonstrate various kinds of LINQ queries that can be used to create various query options. 

## **$filter** 

For `GET /b1s/v2/Items?$filter=ItemsGroupCode eq 100 HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.ItemsGroupCode == 100).ToList();
```

OData Client for Service Layer **Query Options** 

**22** 

PUBLIC 

For `GET /b1s/v2/Items?$filter=endswith(ItemName,'abc') HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.ItemName.EndsWith("abc")).ToList();
```

For `GET /b1s/v2/Items?$filter=startswith(ItemName,'item') HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.ItemName.StartsWith("item")).ToList();
```

For `GET /b1s/v2/Items?$filter=contains(ItemName,'i') HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.ItemName.Contains("i")).ToList()
```

For `GET /b1s/v2/Items?$filter=ItemCode ne 'i001' HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.ItemCode != "i001").ToList();
```

For `GET /b1s/v2/Items?$filter=ItemName eq null and ItemCode ne 'i001' HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.ItemName == null && c.ItemCode !=
"i001").ToList();
```

For `GET /b1s/v2/Items?$filter=PurchaseItem eq SAPB1.BoYesNoEnum'tYES' HTTP/1.1` : 

```
var query = slContext.Items.Where(c => c.PurchaseItem ==
BoYesNoEnum.TYES).ToList();
```

## **$count** 

For `GET /b1s/v2/Items/$count HTTP/1.1` : 

```
var count = slContext.Items.Count()
```

For `GET /b1s/v2/Items?$count=true HTTP/1.1` , we have two ways of making this request: 

```
var query = slContext.Items.IncludeCount().ToList()
```

```
var query2 = slContext.Items.IncludeCount(true).ToList();
```

For `GET /b1s/v2/Items?$count=false HTTP/1.1` : 

```
var query = slContext.Items.IncludeCount(false).ToList();
```

## **$orderby** 

For `GET /b1s/v2/Items?$orderby=ItemCode HTTP/1.1` : 

```
var query = slContext.Items.OrderBy(c => c.ItemCode).ToList();
```

OData Client for Service Layer **Query Options** 

PUBLIC **23** 

For `GET /b1s/v2/Items?$orderby=ItemCode desc HTTP/1.1` : 

```
query = slContext.Items.OrderByDescending(c => c.ItemCode).ToList();
```

## **$skip** 

For `GET https://host/service/People?$skip=3 HTTP/1.1` : 

```
var people = context.People.Skip(3);
```

## **$top** 

For `GET https://host/service/People?$top=3 HTTP/1.1` : 

```
var people = context.People.Take(3);
```

## **$expand** 

For `GET /b1s/v2/Orders?$expand=BusinessPartner HTTP/1.1` : 

```
var query = slContext.Orders.Expand(c => c.BusinessPartner).ToList();
```

For `GET /b1s/v2/Orders(1)?$expand=BusinessPartner HTTP/1.1` : 

```
var query2 = slContext.Orders.Expand(c => c.BusinessPartner).Where(c =>
c.DocEntry == 1).ToList();
```

## **$select** 

For `GET /b1s/v2/Items HTTP/1.1 or GET /b1s/v2/Items?$select=*` : 

```
var query = slContext.Items.ToList();
```

For `GET /b1s/v2/Items?$select=ItemCode,ItemName HTTP/1.1` : 

```
var query = slContext.Items.Select(c => new { c.ItemCode, c.ItemName }).ToList();
```

For `GET /b1s/v2/Orders?$select=DocEntry,DocumentLines HTTP/1.1` : 

```
var query2 = slContext.Orders.Select(c => new { c.DocEntry,
c.DocumentLines }).ToList();
```

OData Client for Service Layer **Query Options** 

**24** PUBLIC 

Combining the above query options, we can construct complicated queries. For `GET /b1s/v2/Orders? $filter=DocEntry gt 1&$orderby=DocNum&$skip=1&$top=2&$expand=BusinessPartner HTTP/ 1.1:` 

```
var query = slContext.Orders
  .Expand(p => p.BusinessPartner)
 .Where(p => p.DocEntry > 1)
 .OrderBy(p => p.DocNum)
 .Skip(1)
 .Take(2);
foreach (var order in query)
{
 Console.WriteLine($"DocEntry: {order.DocEntry} DocNum: {order.DocNum} DocDate:
{order.DocDate}");
 }
```

The order of the query options matters. 

## **6.2 AddQueryOption Method** 

The following example shows how to use the `AddQueryOption` method to create a DataServiceQuery class, which implements the IQueryable . 

```
// GET /b1s/v2/Items?$filter=ItemsGroupCode eq 100&$orderby=ItemName
desc&$skip=1&$top=2&$select=ItemName,ItemCode,ItemsGroupCode,ItemType HTTP/1.1
 DataServiceQuery query = slContext.Items
    .AddQueryOption("$filter", "ItemsGroupCode eq 100")
    .AddQueryOption("$orderby", "ItemName desc")
    .AddQueryOption("$skip", "1")
    .AddQueryOption("$top", "2")
    .AddQueryOption("$select", "ItemName,ItemCode,ItemsGroupCode,ItemType");
foreach (Item item in query)
{
    Console.WriteLine($"ItemName: {item.ItemName} ItemCode: {item.ItemCode}
ItemsGroupCode: {item.ItemsGroupCode}");
 }
```

In the case above, the URI that is generated by the OData client includes the requested entity set, together with the added query options. 

OData Client for Service Layer **Query Options** 

PUBLIC **25** 

## **7 Navigation** 

When you execute a query, only entities in the addressed entity set are returned. For example, when a query against the Service Layer returns `Orders` entities, by default the related `BusinessPartners` entities are not returned, even though there is a relationship between `Orders` and `BusinessPartners` . 

There are two ways to load related entities: 

- Eager Loading 

- Explicit Loading 

## **Related Information** 

Eager Loading [page 26] Explicit Loading [page 27] 

## **7.1 Eager Loading** 

You can use the `$expand` query option to request that the response include related entities of the entity set requested. 

In the OData client you can use the Expand method of DataServiceQuery to add the `$expand` query option to the request that is sent to the data service. You can request multiple related entity sets by separating them using a comma, as shown in the example below. All entities requested by the query are returned in a single response. The following example returns `BusinessPartner` along with the `Orders` entity set: 

```
// GET /b1s/v2/Orders?$expand=BusinessPartner&$top=2 HTTP/1.1
 var query = slContext.Orders.Expand(c => c.BusinessPartner).Take(2);
foreach (Document order in query)
{
    // Explicitly load the Trips for each person.
    Console.WriteLine($"CardCode: {order.BusinessPartner.CardCode}, CardName:
{order.BusinessPartner.CardCode}");
}
// GET /b1s/v2/Orders(1)?$expand=BusinessPartner HTTP/1.1
var query2 = slContext.Orders.Expand(c => c.BusinessPartner).Where(c =>
c.DocEntry == 1);
foreach (Document order in query2)
{
    // Explicitly load the Trips for each person.
    Console.WriteLine($"CardCode: {order.BusinessPartner.CardCode}, CardName:
{order.BusinessPartner.CardCode}");
 }
```

OData Client for Service Layer **Navigation** 

**26** 

PUBLIC 

## **7.2 Explicit Loading** 

In explicit loading, we call the LoadProperty method on the DataServiceContext instance to explicitly load related entities. Each call to the `LoadProperty` method makes a separate request to the data service. 

The following example shows how to explicitly load the `BusinessPartner` that is related to each returned `Orders` instance. 

```
// GET /b1s/v2/Orders?$top=2
 foreach (Document order in slContext.Orders.Take(2))
{
    // Explicitly BusinessPartner the Trips for each order.
    // GET /b1s/v2/Orders(docEntry)/BusinessPartner HTTP/1.1
    slContext.LoadProperty(order, "BusinessPartner");
    Console.WriteLine($"CardCode: {order.BusinessPartner.CardCode}, CardName:
{order.BusinessPartner.CardCode}");
}
foreach (Document order in slContext.Orders.Where(c => c.DocEntry == 1))
{
    // Explicitly BusinessPartner the Trips for each order.
    // GET /b1s/v2/Orders(1)/BusinessPartner HTTP/1.1
    slContext.LoadProperty(order, "BusinessPartner");
    Console.WriteLine($"CardCode: {order.BusinessPartner.CardCode}, CardName:
{order.BusinessPartner.CardCode}");
 }
```

##  Note 

When you consider which option to use, understand that there is a tradeoff between the number of requests to the data service and the amount of data that is returned in a single response. Use eager loading when your application requires associated objects and you want to avoid the added latency of additional requests to explicitly retrieve them. However, if there are cases when the application only needs the data for specific related entity instances, you should consider explicitly loading those entities by calling the `LoadProperty` method. 

OData Client for Service Layer **Navigation** 

PUBLIC **27** 

## **8 Pagination** 

Loading large datasets can be slow. Services often rely on pagination to load the data incrementally to improve the response times and the user experience. The pagination mechanism is implemented via top and skip. It allows the data to be fetched chunk by chunk. Paging can be server-driven or client-driven. 

One Example of pagination when selecting all orders is as follows: 

```
GET /Orders
```

The service returns: 

```
HTTP/1.1 200 OK
 {
    "value": [
        {"DocEntry": 7,"DocNum": 2,...},
        {"DocEntry": 8,"DocNum": 3,...},
        ...
        {"DocEntry": 26,"DocNum": 21,...}
    ],
    "@odata.nextLink": "Orders?$skip=20"
 }
```

Annotation `odata.nextLink` is contained in the body for the link of the next chunk. 

## **8.1 Server-Driven Paging** 

In Server-driven paging, the server returns the first page of results. If the total number of results is greater than the page size, the server returns the first page along with a nextlink that can be used to fetch the next page of results. 

The OData Client deals with server-driven paging with the help of DataServiceQueryContinuation and DataServiceQueryContinuation . These classes contain the `nextLink` of the partial set of items. 

```
// DataServiceQueryContinuation<T> contains the next link
 DataServiceQueryContinuation<Item> nextLink = null;
// Get the first page
QueryOperationResponse<Item> response = slContext.Items.Execute() as
QueryOperationResponse<Item>;
int pageCount = 0;
do
{
    Console.WriteLine($"Page {++pageCount}");
    if (nextLink != null)
    {
        response = slContext.Execute<Item>(nextLink) as
QueryOperationResponse<Item>;
    }
    // You must enumerate the response before calling GetContinuation below.
    foreach (Item item in response)
    {
```

OData Client for Service Layer **Pagination** 

**28** PUBLIC 

```
        Console.WriteLine($"\tItem Name: {item.ItemCode}");
    }
}
// Loop if there is a next link
 while ((nextLink = response.GetContinuation()) != null);
```

## **8.2 Client-Driven Paging** 

In client-driven paging, we request the server to return the specified number of results. There is no `nextLink` that is returned. 

The OData Client deals with client-driven paging using `$skip` and `$top` query options. 

The `$top` query option requests the number of items in the queried collection to be included in the result. 

The `$skip` query option requests the number of items in the queried collection that are to be skipped and not included in the result. 

For `GET https://host/service/Items?$skip=3&$top=5` : 

```
IQueryable<Item> query =
     slContext.Items
        .Skip(3)
        .Take(5);
foreach (Item item in query)
{
    Console.WriteLine($"{item.ItemName},{item.ItemtName}");
 }
```

##  Note 

- The default page size is 20. It can be customized by specifying the following request header: 

```
GET /Orders
 Prefer:odata.maxpagesize=10
 ... (other headers)
```

In the response, the HTTP header `Preference-Appliedis` is included to indicate whether and how the request is accepted like this: 

```
HTTP/1.1 200 OK
 Preference-Applied: odata.maxpagesize=10
 ...
```

• If `odata.maxpagesize` is set to 0, the pagination mechanism is turned off (no paging). Accordingly, for handy usage of this mechanism, a property `PageSize` is exposed to operate the page size. 

```
int oldPageSize = slContext.PageSize;
 slContext.PageSize = 10;
// to fetch the data chunk by chunk
 slContext.PageSize = oldPageSize;
```

OData Client for Service Layer **Pagination** 

PUBLIC 

**29** 

## **9 Batch Operations** 

OData Client for .NET supports batch processing of requests to an OData service and the Service Layer is able to process the batch requests. This ensures that all operations in the batch are sent to the Service Layer in a single HTTP request, which enables the server to process the operations automatically and reduces the number of round trips to the service. 

However, OData Client for .NET does not support sending both a query and a change in one batch request. As such, you need to do the batch query and batch modifications separately. 

## **9.1 Batch Query** 

To execute multiple queries in a single batch, you must create each query in the batch as a separate instance of the `DataServiceRequest<TElement>` class. The batched query requests are sent to the data service when the `ExecuteBatch` method is called. It contains the query request objects. 

This method accepts an array of `DataServiceRequest` as parameters. It returns a `DataServiceResponse` object, which is a collection of `QueryOperationResponse<T>` objects that represent responses to individual queries in the batch, each of which contains either a collection of objects returned by the query or error information. When any single query operation in the batch fails, error information is returned in the `QueryOperationResponse<T>` object for the operation that failed and the remaining operations are still executed. 

```
// Items Query
 DataServiceQuery<Item> itemQuery = slContext.Items;
// BusinessPartners Query
DataServiceQuery<BusinessPartner> businessPartnerQuery =
slContext.BusinessPartners;
// Send the request
DataServiceResponse batchResponse = slContext.ExecuteBatch(itemQuery,
businessPartnerQuery);
foreach (OperationResponse r in batchResponse)
{
    QueryOperationResponse<Item> items = r as QueryOperationResponse<Item>;
    if (items != null)
    {
        foreach (Item item in items)
        {
            Console.WriteLine($"Item Code: {item.ItemCode}");
        }
    }
    QueryOperationResponse<BusinessPartner> businessPartners = r as
QueryOperationResponse<BusinessPartner>;
    if (businessPartners != null)
    {
        foreach (BusinessPartner businessPartner in businessPartners)
        {
            Console.WriteLine($"BusinessPartner Code:
{businessPartner.CardCode}");
        }
    }
```

OData Client for Service Layer **Batch Operations** 

**30** PUBLIC 

```
 }
```

`ExecuteBatch` will send a `POST` request to `https://servicelayerhost:50000/b1s/v2/$batch` . Each internal request contains its own http method `GET` . 

In .NetCore we can also use the `await` / `async` syntax as follows: 

```
DataServiceResponse batchResponse = await slContext.ExecuteBatchAsync(itemQuery,
businessPartnerQuery);
```

The payload of the request is as follows: 

```
POST https://servicelayerhost:50000/b1s/v2/$batch HTTP/1.1
 OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: multipart/mixed
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
Connection: Keep-Alive
Content-Type: multipart/mixed; boundary=batch_4a22f153-6e6c-42f7-8110-
bd343e9a341c
Content-Length: 851
Host: servicelayerhost:50000
--batch_4a22f153-6e6c-42f7-8110-bd343e9a341c
Content-Type: application/http
Content-Transfer-Encoding: binary
GET https://servicelayerhost:50000/b1s/v2/Items HTTP/1.1
OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
--batch_4a22f153-6e6c-42f7-8110-bd343e9a341c
Content-Type: application/http
Content-Transfer-Encoding: binary
GET https://servicelayerhost:50000/b1s/v2/BusinessPartners HTTP/1.1
OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
 --batch_4a22f153-6e6c-42f7-8110-bd343e9a341c--
```

The corresponding response is as follows: 

```
HTTP/1.1 200 OK
 Date: Wed, 23 Jun 2021 01:56:59 GMT
Server: Apache
OData-Version: 4.0
Content-Length: 469978
Keep-Alive: timeout=5, max=92
Connection: Keep-Alive
Content-Type: multipart/mixed;boundary=batchresponse_Q7pItIuj-iAPp-004m-
V9tP-7NfcDPUFItCC
--batchresponse_Q7pItIuj-iAPp-004m-V9tP-7NfcDPUFItCC
Content-Type: application/http
Content-Transfer-Encoding: binary
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;charset=utf-8
Content-Length: 407210
OData-Version: 4.0
{
```

OData Client for Service Layer **Batch Operations** 

PUBLIC 

**31** 

```
  "@odata.context": "https://servicelayerhost:50000/b1s/v2/$metadata#Items",
  "value": [
    {
      "@odata.etag": "W/\"9E6A55B6B4563E652A23BE9D623CA5055C356940\"",
      "ItemCode": "i001",
      "ItemName": "Updated Name",
      "ForeignName": null,
      ...
    }
  ]
}
--batchresponse_Q7pItIuj-iAPp-004m-V9tP-7NfcDPUFItCC
Content-Type: application/http
Content-Transfer-Encoding: binary
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;charset=utf-8
Content-Length: 62203
OData-Version: 4.0
{
  "@odata.context": "https://
servicelayerhost:50000/b1s/v2/$metadata#BusinessPartners",
  "value": [
    {
      "@odata.etag": "W/\"12C6FC06C99A462375EEB3F43DFD832B08CA9E17\"",
      "CardCode": "c001",
       ...
    }
  ]
} --batchresponse_Q7pItIuj-iAPp-004m-V9tP-7NfcDPUFItCC--
```

## **9.2 Batch Modification** 

In order to batch a set of changes to the server, `DataServiceContext` provides the following two options when `SaveChanges` is called. 

- `SaveChangesOptions.BatchWithSingleChangeset` 

   - This option is used to save changes in a single change set in a batch request. If one request in the batch fails, all requests fail. 

- `SaveChangesOptions.BatchWithIndependentOperations` 

   - This option is used to save each change independently in a batch request. If one request in the batch fails, the other requests are not affected. 

To get more details about whether requests should be contained in one change set or not, please refer to odata v4.0 batch . 

## **9.2.1  Update** 

The following is a sample code snippet for the update case: 

```
slContext.MergeOption = MergeOption.PreserveChanges;
 // Find an Item and a businessPartner
```

OData Client for Service Layer **Batch Operations** 

**32** 

PUBLIC 

```
Item item = slContext.Items.First();
BusinessPartner businessPartner = slContext.BusinessPartners.First();
// Update the name properties.
item.ItemName = "Updated Name";
businessPartner.CardName = "Updated Name";
slContext.UpdateObject(item);
slContext.UpdateObject(businessPartner);
// Send the request
DataServiceResponse batchResponse =
slContext.SaveChanges(SaveChangesOptions.BatchWithSingleChangeset);
Console.WriteLine($"Updated ItemName: {item.ItemName}");
Console.WriteLine($"Updated CardName: {businessPartner.CardName}");
foreach (OperationResponse r in batchResponse)
{
    Console.WriteLine($"Status Code: {r.StatusCode}");
 }
```

Actually, we can also use the `await` / `async` syntax as follows. 

```
await dsc.SaveChangesAsync(SaveChangesOptions.BatchWithSingleChangeset);
```

No matter which approach, this will generate a request with a full URL like 

```
https://servicelayerhost:50000/b1s/v2/$batch
```

Please note the following request headers, which are a typical indication for a batch request. 

```
Content-Type: multipart/mixed; boundary=batch_6d467cae-0ab7-4efc-
bba7-311feb4fa816
 Accept: multipart/mixed
```

The entire request payload is like the following: 

```
POST https://servicelayerhost:50000/b1s/v2/$batch HTTP/1.1
 OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: multipart/mixed
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
Connection: Keep-Alive
Content-Type: multipart/mixed; boundary=batch_6d467cae-0ab7-4efc-
bba7-311feb4fa816
Content-Length: 26783
Host: servicelayerhost:50000
--batch_6d467cae-0ab7-4efc-bba7-311feb4fa816
Content-Type: multipart/mixed;
boundary=changeset_f8b8364a-4a3f-4dc8-8c9c-8b07dcc47a55
--changeset_f8b8364a-4a3f-4dc8-8c9c-8b07dcc47a55
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 4
PATCH https://servicelayerhost:50000/b1s/v2/Items('i%2B1') HTTP/1.1
OData-Version: 4.0
OData-MaxVersion: 4.0
Content-Type: application/json;odata.metadata=minimal
If-Match: W/"0716D9708D321FFB6A00818614779E779925365C"
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
{"@odata.type":"#SAPB1.Item","ItemName":"Updated Name", ...}
--changeset_f8b8364a-4a3f-4dc8-8c9c-8b07dcc47a55
Content-Type: application/http
Content-Transfer-Encoding: binary
```

OData Client for Service Layer **Batch Operations** 

PUBLIC **33** 

## `Content-ID: 5` 

```
PATCH https://servicelayerhost:50000/b1s/v2/BusinessPartners('c001') HTTP/1.1
OData-Version: 4.0
OData-MaxVersion: 4.0
Content-Type: application/json;odata.metadata=minimal
If-Match: W/"472B07B9FCF2C2451E8781E944BF5F77CD8457C8"
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
{"@odata.type":"#SAPB1.BusinessPartner","CardName":"Updated Name", ...}
--changeset_f8b8364a-4a3f-4dc8-8c9c-8b07dcc47a55--
--batch_6d467cae-0ab7-4efc-bba7-311feb4fa816--
```

Upon success, the corresponding response is like the following: 

```
HTTP/1.1 200 OK
 Date: Wed, 23 Jun 2021 01:56:54 GMT
Server: Apache
OData-Version: 4.0
Content-Length: 650
Keep-Alive: timeout=5, max=97
Connection: Keep-Alive
Content-Type: multipart/mixed;boundary=batchresponse_zlicGyun-Awhy-Rko0-
kz2Z-0tmxMppahpOU
--batchresponse_zlicGyun-Awhy-Rko0-kz2Z-0tmxMppahpOU
Content-Type: multipart/mixed; boundary=changesetresponse_zlicGyun-Awhy-Rko0-
kz2Z-0tmxMppahpOU
--changesetresponse_zlicGyun-Awhy-Rko0-kz2Z-0tmxMppahpOU
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 4
HTTP/1.1 204 No Content
OData-Version: 4.0
--changesetresponse_zlicGyun-Awhy-Rko0-kz2Z-0tmxMppahpOU
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 5
HTTP/1.1 204 No Content
OData-Version: 4.0
--changesetresponse_zlicGyun-Awhy-Rko0-kz2Z-0tmxMppahpOU--
 --batchresponse_zlicGyun-Awhy-Rko0-kz2Z-0tmxMppahpOU--
```

## **9.2.2  Create** 

Similar to the batch update request, the following is a sample code snippet for the batch creation case: 

```
slContext.MergeOption = MergeOption.PreserveChanges;
 // Create an Item and add it to the OData context.
Item item = new Item();
item.ItemCode = "FirstItem";
slContext.AddToItems(item);
// Create another Item and add it to the OData context.
Item item2 = new Item();
item2.ItemCode = "SecondItem";
slContext.AddToItems(item2);
// Send the request
DataServiceResponse batchResponse =
slContext.SaveChanges(SaveChangesOptions.BatchWithSingleChangeset);
foreach (OperationResponse response in batchResponse)
{
```

OData Client for Service Layer **Batch Operations** 

PUBLIC 

**34** 

```
    Console.WriteLine($"Status Code: {response.StatusCode}");
```

```
    var changeResponse = response as ChangeOperationResponse;
    var entityDescriptor = changeResponse.Descriptor as EntityDescriptor;
    // Get the entity created on the service and check if the entity is as
expected.
    Item entity = entityDescriptor.Entity as Item;
    Console.WriteLine("Created ItemCode={0}", entity.ItemCode);
 }
```

The request payload is as follows: 

```
POST https://servicelayerhost:50000/b1s/v2/$batch HTTP/1.1
 OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: multipart/mixed
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
Connection: Keep-Alive
Content-Type: multipart/mixed; boundary=batch_8e382096-4ffd-470b-bfd5-
eaa6c6fb30e6
Content-Length: 3549
Host: servicelayerhost:50000
--batch_8e382096-4ffd-470b-bfd5-eaa6c6fb30e6
Content-Type: multipart/mixed; boundary=changeset_46829707-7cb0-4cbc-94a2-
f627457b6b4d
--changeset_46829707-7cb0-4cbc-94a2-f627457b6b4d
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 6
POST https://servicelayerhost:50000/b1s/v2/Items HTTP/1.1
OData-Version: 4.0
OData-MaxVersion: 4.0
Content-Type: application/json;odata.metadata=minimal
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
{"@odata.type":"#SAPB1.Item","ItemCode":"FirstItem", ...}
--changeset_46829707-7cb0-4cbc-94a2-f627457b6b4d
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 7
POST https://servicelayerhost:50000/b1s/v2/Items HTTP/1.1
OData-Version: 4.0
OData-MaxVersion: 4.0
Content-Type: application/json;odata.metadata=minimal
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
{"@odata.type":"#SAPB1.Item","ItemCode":"SecondItem", ...}
--changeset_46829707-7cb0-4cbc-94a2-f627457b6b4d--
--batch_8e382096-4ffd-470b-bfd5-eaa6c6fb30e6--
```

Upon success, the corresponding response is as follows: 

```
HTTP/1.1 200 OK
 Date: Wed, 23 Jun 2021 01:56:57 GMT
Server: Apache
OData-Version: 4.0
Content-Length: 35193
Keep-Alive: timeout=5, max=96
Connection: Keep-Alive
```

OData Client for Service Layer **Batch Operations** 

PUBLIC **35** 

```
Content-Type: multipart/mixed;boundary=batchresponse_DbUNxTGa-q8ZD-NsWF-
ebd9-1Q3hrcOyYIMx
--batchresponse_DbUNxTGa-q8ZD-NsWF-ebd9-1Q3hrcOyYIMx
Content-Type: multipart/mixed; boundary=changesetresponse_DbUNxTGa-q8ZD-NsWF-
ebd9-1Q3hrcOyYIMx
--changesetresponse_DbUNxTGa-q8ZD-NsWF-ebd9-1Q3hrcOyYIMx
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 6
HTTP/1.1 201 Created
Content-Type: application/json;odata.metadata=minimal;charset=utf-8
Content-Length: 17067
ETag: W/"356A192B7913B04C54574D18C28D46E6395428AB"
Location: https://servicelayerhost:50000/b1s/v2/Items('FirstItem')
OData-Version: 4.0
{
   "@odata.context" : "https://servicelayerhost:50000/b1s/v2/$metadata#Items/
$entity",
   "@odata.etag" : "W/\"356A192B7913B04C54574D18C28D46E6395428AB\"",
   "ItemCode" : "FirstItem",
   "ItemName" : null,
   "ForeignName" : null,
   "ItemsGroupCode" : 100,
   "CustomsGroupCode" : -1,
   "SalesVATGroup" : null,
    ...
}
--changesetresponse_DbUNxTGa-q8ZD-NsWF-ebd9-1Q3hrcOyYIMx
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 7
HTTP/1.1 201 Created
Content-Type: application/json;odata.metadata=minimal;charset=utf-8
Content-Length: 17071
ETag: W/"356A192B7913B04C54574D18C28D46E6395428AB"
Location: https://servicelayerhost:50000/b1s/v2/Items('SecondItem')
OData-Version: 4.0
{
   "@odata.context" : "https://servicelayerhost:50000/b1s/v2/$metadata#Items/
$entity",
   "@odata.etag" : "W/\"356A192B7913B04C54574D18C28D46E6395428AB\"",
   "ItemCode" : "SecondItem",
   "ItemName" : null,
   "ForeignName" : null,
   ...
}
--changesetresponse_DbUNxTGa-q8ZD-NsWF-ebd9-1Q3hrcOyYIMx--
 --batchresponse_DbUNxTGa-q8ZD-NsWF-ebd9-1Q3hrcOyYIMx--
```

## **9.2.3  Delete** 

Similar to the batch update request, the following is a sample code snippet for the batch delete case: 

```
slContext.MergeOption = MergeOption.PreserveChanges;
 // Create a delete request
Item item = slContext.Items.ByKey(itemCode: "FirstItem").GetValue();
slContext.DeleteObject(item);
// Create another delete request
Item item2 = slContext.Items.ByKey(itemCode: "SecondItem").GetValue();
slContext.DeleteObject(item2);
// Send the request
DataServiceResponse batchResponse =
slContext.SaveChanges(SaveChangesOptions.BatchWithSingleChangeset);
```

OData Client for Service Layer **Batch Operations** 

**36** 

PUBLIC 

```
foreach (OperationResponse response in batchResponse)
{
    Console.WriteLine($"Status Code: {response.StatusCode}");
 }
```

The request payload is as follows: 

```
POST https://servicelayerhost:50000/b1s/v2/$batch HTTP/1.1
 OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: multipart/mixed
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
Connection: Keep-Alive
Content-Type: multipart/mixed;
boundary=batch_f24f7b01-3201-45e7-95b9-39871e238f33
Content-Length: 1211
Host: servicelayerhost:50000
--batch_f24f7b01-3201-45e7-95b9-39871e238f33
Content-Type: multipart/mixed;
boundary=changeset_c133dd73-304b-404f-94d6-9cd36d8e31a6
--changeset_c133dd73-304b-404f-94d6-9cd36d8e31a6
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 8
DELETE https://servicelayerhost:50000/b1s/v2/Items('FirstItem') HTTP/1.1
If-Match: W/"356A192B7913B04C54574D18C28D46E6395428AB"
OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
--changeset_c133dd73-304b-404f-94d6-9cd36d8e31a6
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 9
DELETE https://servicelayerhost:50000/b1s/v2/Items('SecondItem') HTTP/1.1
If-Match: W/"356A192B7913B04C54574D18C28D46E6395428AB"
OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
cookie: B1SESSION=3ebbb5dc-d3c6-11eb-8dcf-0a0027000008;HttpOnly;
--changeset_c133dd73-304b-404f-94d6-9cd36d8e31a6--
 --batch_f24f7b01-3201-45e7-95b9-39871e238f33--
```

Upn success, the corresponding response is as follows: 

```
HTTP/1.1 200 OK
 Date: Wed, 23 Jun 2021 01:56:59 GMT
Server: Apache
OData-Version: 4.0
Content-Length: 650
Keep-Alive: timeout=5, max=93
Connection: Keep-Alive
Content-Type: multipart/mixed;boundary=batchresponse_Gy3oTITX-gKHc-d6YR-FiUO-
ydeuCtdX92eH
--batchresponse_Gy3oTITX-gKHc-d6YR-FiUO-ydeuCtdX92eH
Content-Type: multipart/mixed; boundary=changesetresponse_Gy3oTITX-gKHc-d6YR-
FiUO-ydeuCtdX92eH
--changesetresponse_Gy3oTITX-gKHc-d6YR-FiUO-ydeuCtdX92eH
Content-Type: application/http
Content-Transfer-Encoding: binary
```

OData Client for Service Layer **Batch Operations** 

PUBLIC 

**37** 

```
Content-ID: 8
HTTP/1.1 204 No Content
OData-Version: 4.0
--changesetresponse_Gy3oTITX-gKHc-d6YR-FiUO-ydeuCtdX92eH
Content-Type: application/http
Content-Transfer-Encoding: binary
Content-ID: 9
HTTP/1.1 204 No Content
OData-Version: 4.0
--changesetresponse_Gy3oTITX-gKHc-d6YR-FiUO-ydeuCtdX92eH--
 --batchresponse_Gy3oTITX-gKHc-d6YR-FiUO-ydeuCtdX92eH--
```

OData Client for Service Layer **Batch Operations** 

**38** PUBLIC 

## **10 User-Defined Field (UDF)** 

## **10.1 OpenType** 

In OData V4, an open type is a structured type that contains dynamic properties, in addition to any properties that are declared in the type definition. Open types let you add flexibility to your data models. 

In SAP Business One, lots of business objects support user-defined fields (UDFs), which means partners are allowed to create additional fields dynamically on an existing entity in order to extend their application. 

Therefore, open type can be perfectly suited to UDFs. 

By checking the Service Layer metadata, you will find some entity types declared with the attribute `OpenType="true"` in the following way: 

```
<EntityType Name="Item" OpenType="true">
     <Key>
        <PropertyRef Name="ItemCode"/>
    </Key>
    <Property Name="ItemCode" Nullable="false" Type="Edm.String"/>
    <Property Name="ItemName" Type="Edm.String"/>
    <Property Name="ForeignName" Type="Edm.String"/>
    <Property Name="ItemsGroupCode" Type="Edm.Int32"/>
    <Property Name="CustomsGroupCode" Type="Edm.Int32"/>
    ...
 </EntityType>
```

This indicates the entity Item is of a dynamic type and is able to support UDFs. 

## **10.2 Dynamic Properties** 

In support of this, OData Connected Service release 0.10.0 introduced support for emitting the dynamic properties container property for open types on the client. The emitted property looks like this in C#: 

```
[global::Microsoft.OData.Client.OriginalNameAttribute("DynamicProperties")]
 [global::Microsoft.OData.Client.ContainerProperty]
public virtual global::System.Collections.Generic.IDictionary<string, object>
DynamicProperties
{
    get
    {
        return this._DynamicProperties;
    }
    set
    {
        this.OnDynamicPropertiesChanging(value);
        this._DynamicProperties = value;
        this.OnDynamicPropertiesChanged();
        this.OnPropertyChanged("DynamicProperties");
```

OData Client for Service Layer **User-Defined Field (UDF)** 

PUBLIC 

**39** 

```
    }
}
[global::System.CodeDom.Compiler.GeneratedCodeAttribute("Microsoft.OData.Client.D
esign.T4", "#VersionNumber#")]
```

```
private global::System.Collections.Generic.IDictionary<string, object>
_DynamicProperties = new global::System.Collections.Generic.Dictionary<string,
object>();
partial void
OnDynamicPropertiesChanging(global::System.Collections.Generic.IDictionary<string
, object> value);
 partial void OnDynamicPropertiesChanged();
```

In the following part, let's assume for Items, we create a UDF named `U_item_udf1` that is going to do the CRUD operations. 

For the Item itself, at runtime, you would find there is a container member `DynamicProperties` from an item instance: 

**==> picture [455 x 170] intentionally omitted <==**

## **10.3 UDF Operations** 

## **UDF Create** 

```
//Create an Item with UDF and add it to the OData context.
 Item item = new Item();
item.ItemCode = "yourItemCode";
//Set the UDF
item.DynamicProperties = new Dictionary<string, object>
{
    { "U_item_udf1", "123"}
};
slContext.AddToItems(item);
// Send the request
 DataServiceResponse responses = slContext.SaveChanges();
```

OData Client for Service Layer **User-Defined Field (UDF)** 

**40** 

PUBLIC 

## **UDF Retrieve** 

```
object udf1;
```

```
 var item = slContext.Items.Where(c => c.ItemCode == "yourItemCode").Single();
// Get the UDF
if(item.DynamicProperties.TryGetValue("U_item_udf1", out udf1))
{
    Console.WriteLine("ItemCode={0},ItemName={1},udf1={2}", item.ItemCode,
item.ItemName, udf1);
}
var item2 = slContext.Items.Where(c => c.ItemCode == "yourItemCode").First();
// Get the UDF
if (item2.DynamicProperties.TryGetValue("U_item_udf1", out udf1))
{
    Console.WriteLine("ItemCode={0},ItemName={1},udf1={2}", item2.ItemCode,
item2.ItemName, udf1);
 }
```

## **UDF Update** 

```
var items = new DataServiceCollection<Item>(slContext.Items.Where(p =>
p.ItemCode == "yourItemCode"));
 // Change its property
items[0].ItemName = "New name";
// Update the UDF
items[0].DynamicProperties = new Dictionary<string, object>
{
    { "U_item_udf1", "456"}
};
// Send the request
 DataServiceResponse responses = slContext.SaveChanges();
```

## **UDF Delete** 

```
Item item = slContext.Items.ByKey(itemCode: "yourItemCode").GetValue();
 // Create a delete request
slContext.DeleteObject(item);
// Send the request
 DataServiceResponse responses = slContext.SaveChanges();
```

OData Client for Service Layer **User-Defined Field (UDF)** 

PUBLIC **41** 

## **11 User-Defined Object (UDO)/User-Defined Table (UDT)** 

For UDOs/UDTs, as they are dynamic objects, any new UDO/UDT would cause a change to the metadata structure. In this case, there is no better solution than regenerating the source code according to the modified metadata. Once the source code is changed the whole project needs to recompiled, therefore just treat the UDO/UDT as a System object, and its CRUD operations are basically the same. 

Assume you have an UDO named MyOrder, with the following metadata information. 

```
 <ComplexType Name="MyOrderLines" OpenType="true">
      <Property Name="DocEntry" Type="Edm.Int32"/>
     <Property Name="LineId" Type="Edm.Int32"/>
     <Property Name="VisOrder" Type="Edm.Int32"/>
     <Property Name="Object" Type="Edm.String"/>
     <Property Name="LogInst" Type="Edm.Int32"/>
     <Property Name="U_ItemName" Type="Edm.String"/>
     <Property Name="U_Price" Type="Edm.Double"/>
     <Property Name="U_Quantity" Type="Edm.Double"/>
</ComplexType>
<EntityType Name="MyOrder" OpenType="true">
    <Key>
        <PropertyRef Name="DocEntry"/>
    </Key>
    <Property Name="DocNum" Type="Edm.Int32"/>
    <Property Name="Period" Type="Edm.Int32"/>
    <Property Name="Instance" Type="Edm.Int32"/>
    <Property Name="Series" Type="Edm.Int32"/>
    <Property Name="Handwrtten" Type="Edm.String"/>
    <Property Name="Status" Type="Edm.String"/>
    <Property Name="RequestStatus" Type="Edm.String"/>
    <Property Name="Creator" Type="Edm.String"/>
    <Property Name="Remark" Type="Edm.String"/>
    <Property Name="DocEntry" Nullable="false" Type="Edm.Int32"/>
    <Property Name="Canceled" Type="Edm.String"/>
    <Property Name="Object" Type="Edm.String"/>
    <Property Name="LogInst" Type="Edm.Int32"/>
    <Property Name="UserSign" Type="Edm.Int32"/>
    <Property Name="Transfered" Type="Edm.String"/>
    <Property Name="CreateDate" Type="Edm.DateTimeOffset"/>
    <Property Name="CreateTime" Type="Edm.TimeOfDay"/>
    <Property Name="UpdateDate" Type="Edm.DateTimeOffset"/>
    <Property Name="UpdateTime" Type="Edm.TimeOfDay"/>
    <Property Name="DataSource" Type="Edm.String"/>
    <Property Name="U_CustomerName" Type="Edm.String"/>
    <Property Name="U_DocTotal" Type="Edm.Double"/>
    <Property Name="MyOrderLinesCollection"
Type="Collection(SAPB1.MyOrderLines)"/>
</EntityType>
  <EntitySet EntityType="SAPB1.MyOrder" Name="MyOrder"/>
```

Let's do the CRUD operations on this UDO. 

OData Client for Service Layer **User-Defined Object (UDO)/User-Defined Table (UDT)** 

**42** 

PUBLIC 

## **UDO Create** 

```
//Create an UDO and add it to the OData context.
 MyOrder order = new MyOrder();
order.U_CustomerName = m_cardCode;
order.U_DocTotal = 620;
MyOrderLines line = new MyOrderLines();
line.U_ItemName = m_itemCode;
line.U_Price = 10;
line.U_Quantity = 5;
order.MyOrderLinesCollection.Add(line);
slContext.AddToMyOrder(order);
// Send the request
 DataServiceResponse responses = slContext.SaveChanges();
```

## **UDO Retrieve** 

```
var order = slContext.MyOrder.Where(c => c.DocEntry == m_docEntry).Single();
 Console.WriteLine("DocEntry={0},DocNum={1}", order.DocEntry, order.DocNum);
var order2 = slContext.MyOrder.Where(c => c.DocEntry == m_docEntry).First();
 Console.WriteLine("DocEntry={0},DocNum={1}", order2.DocEntry, order2.DocNum);
```

## **UDO Update** 

```
// Get an entity
 var orders = new DataServiceCollection<MyOrder>(slContext.MyOrder.Where(p =>
p.DocEntry == m_docEntry));
// Change its property
orders[0].Remark= "Updated from OData Client.";
// Send the request
 DataServiceResponse responses = slContext.SaveChanges();
```

## **UDO Delete** 

Unlike the system object `Orders` , `MyOrder` is allowed to be removed. 

```
MyOrder myOrder = slContext.MyOrder.ByKey(docEntry: m_docEntry).GetValue();
 // Create a delete request
slContext.DeleteObject(myOrder);
// Send the request
 DataServiceResponse responses = slContext.SaveChanges();
```

OData Client for Service Layer **User-Defined Object (UDO)/User-Defined Table (UDT)** 

PUBLIC 

**43** 

## **12 Function and Action** 

In OData, actions and functions are a way to add server-side behaviors that are not easily defined as CRUD operations on entities. While both actions and functions can return data, the difference between them is that the former can have side effects but the latter do not. An action or function can target a single entity or a collection. In OData terminology, this is the binding. You can also have "unbound" actions/functions, which are called as static operations on the service. 

## **Related Information** 

Function [page 44] Action [page 45] 

## **12.1 Function** 

Functions are useful for returning information that does not correspond directly to an entity or collection. Let's see some examples. 

## **Example 1: CompanyService_GetAdminInfo** 

```
// GET /b1s/v2/CompanyService_GetAdminInfo HTTP/1.1
 AdminInfo adminInfo = slContext.CompanyService_GetAdminInfo().GetValue();
 Console.WriteLine("CompanyName={0},Country={1}", adminInfo.CompanyName,
adminInfo.Country);
```

For the response, let's check the content as below and you will find it is an exact JSON representation of an instance of class `AdminInfo` , except for the OData annotation @odata.context. 

```
{     "@odata.context": "https://
servicelayerhost:50000/b1s/v2/$metadata#SAPB1.AdminInfo",
    "Code": 1,
    "CompanyName": "US1112",
    "Address": null,
    "Country": "US",
    "PrintingHeader": null,
    "PhoneNumber1": null,
    "PhoneNumber2": null,
    "FaxNumber": null,
    "eMail": null,
```

OData Client for Service Layer **Function and Action** 

PUBLIC 

**44** 

```
    "ManagingDirector": null,
    "ChartofAccountsTemplate": "C",
    "LocalCurrency": "$",
    "SystemCurrency": "$",
    "CreditBalancewithMinusSign": "tYES",
    "StandardUnitofLength": 5,
    ...
 }
```

## **Example 2: CompanyService_GetPathAdmin** 

```
// GET /b1s/v2/CompanyService_GetPathAdmin HTTP/1.1
 PathAdmin pathAdmin = slContext.CompanyService_GetPathAdmin().GetValue();
 Console.WriteLine("AttachmentsFolderPath={0},PicturesFolderPath={1}",
pathAdmin.AttachmentsFolderPath, pathAdmin.PicturesFolderPath);
```

For the response, let's check the content as below and you will find it is an exact JSON representation of an instance of class `PathAdmin` , except for the OData annotation @odata.context. 

```
{     "@odata.context": "https://
servicelayerhost:50000/b1s/v2/$metadata#SAPB1.PathAdmin",
    "WordTemplateFolderPath": null,
    "PicturesFolderPath": "C:\\Users\\administrator\\Pictures\\pic\\",
    "AttachmentsFolderPath": "C:\\Users\\administrator\\Documents\\attach\\",
    "ExtensionsFolderPath": null,
    "PrintId": "US11"
 }
```

## **Example 3: SBOBobService_GetSystemCurrency** 

```
// GET /b1s/v2/SBOBobService_GetSystemCurrency HTTP/1.1
 string currency = slContext.SBOBobService_GetSystemCurrency().GetValue();
 Console.WriteLine("SystemCurrency={0}", currency);
```

For the response, it simply returns `$` , which is of a primitive string. 

## **12.2 Action** 

Some typical user cases for actions include: 

- Complex transactions 

- Manipulating several entities at once 

- Only allowing updates to certain properties of an entity 

- Sending data that is not an entity 

Let's see some examples. 

OData Client for Service Layer **Function and Action** 

PUBLIC 

**45** 

## **Example 1: CompanyService_UpdateAdminInfo** 

```
// GET /b1s/v2/CompanyService_GetPathAdmin HTTP/1.1
 PathAdmin pathAdmin = slContext.CompanyService_GetPathAdmin().GetValue();
Console.WriteLine("AttachmentsFolderPath={0},PicturesFolderPath={1}",
pathAdmin.AttachmentsFolderPath, pathAdmin.PicturesFolderPath);
// POST /b1s/v2/CompanyService_UpdatePathAdmin HTTP/1.1
// Update the PicturesFolderPath
string oldPath = pathAdmin.PicturesFolderPath;
pathAdmin.PicturesFolderPath = "/Users"; //Ensure this path is valid.
OperationResponse operationResponse =
slContext.CompanyService_UpdatePathAdmin(pathAdmin).Execute();
 Console.WriteLine("Expected StatusCode={0}, Actual StatusCode={1}",
(int)HttpStatusCode.NoContent, operationResponse.StatusCode);
```

This example illustrates how to get the path admin, modify one property and then send the update request. For the update request, check the payload as below and we will find that the `PicturesFolderPath` property is updated. 

```
POST https://servicelayerhost:50000/b1s/v2/CompanyService_UpdatePathAdmin
HTTP/1.1
 OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=3898d42e-de0b-11eb-8000-0a0027000008;HttpOnly;
Connection: Keep-Alive
Content-Type: application/json; odata.metadata=minimal
Content-Length: 219
{
  "PathAdmin": {
    "@odata.type": "#SAPB1.PathAdmin",
    "AttachmentsFolderPath": "C:\\Users\\administrator\\Documents\\attach\\",
    "ExtensionsFolderPath": null,
    "PicturesFolderPath": "/Users",
    "PrintId": "US11",
    "WordTemplateFolderPath": null
  }
 }
```

## **Example 2: Orders(id)/Cancel** 

```
int docEntry = 1;
 var order = slContext.Orders.Where(c => c.DocEntry == docEntry).Single();
OperationResponse operationResponse = order.Cancel().Execute();
 Console.WriteLine("Expected StatusCode={0}, Actual StatusCode={1}",
(int)HttpStatusCode.NoContent, operationResponse.StatusCode);
```

This example assumes you have an existing order that you would like to cancel. Corresponding to the above code snippet, the OData Client library triggers a request like below: 

```
POST https://servicelayerhost:50000/b1s/v2/Orders(16)/SAPB1.Cancel HTTP/1.1
 OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=a1a82a88-de14-11eb-8000-0a0027000008;HttpOnly;
```

OData Client for Service Layer **Function and Action** 

**46** 

PUBLIC 

```
Connection: Keep-Alive
 Content-Length: 0
```

##  Note 

Take notice of the URI `Orders(16)/SAPB1.Cancel` , there is also a namespace prefix `SAPB1` . For the Service Layer, both `Orders(16)/Cancel` and `Orders(16)/SAPB1.Cancel` are supported. 

OData Client for Service Layer **Function and Action** 

PUBLIC **47** 

## **13 Stream** 

In this section, we will show you how to use the OData client library to access binary data exposed by an OData feed, as well as how to upload binary data to the data service. For more information on streaming, see the relevant OData spec . 

In the Service Layer, the entities with streaming capabilities are in the following list: 

- Attachments2 

- Pictures 

- ItemImages 

- EmployeeImage 

If you look at its metadata you will see such streaming entities have a special attribute `HasStream="true"` , which means that the entity type is a media entity and represents a media stream, such as a photo. 

```
<EntityType HasStream="true" Name="Attachments2" OpenType="true">
     <Key>
        <PropertyRef Name="AbsoluteEntry"/>
    </Key>
    <Property Name="AbsoluteEntry" Nullable="false" Type="Edm.Int32"/>
    <Property Name="Attachments2_Lines"
Type="Collection(SAPB1.Attachments2_Line)"/>
 </EntityType>
```

The following part will take Attachments2 as an example in order to demonstrate how to do the stream upload and download. 

## **Related Information** 

Uploading Images and Texts [page 48] 

Downloading Images and Texts [page 50] 

## **13.1 Uploading Images and Texts** 

`DataServiceContext` provides `SetSaveStream` to support the setting of a binary data stream that belongs to the specified entity, with the specified Content-Type and `Slug` headers in the request message. 

`Slug` is an HTTP entity-header whose presence in a POST to a Collection constitutes a request by the client to use the header's value as part of any URIs that would normally be used to retrieve the to-be-created Entry or Media Resources. For information about Slug, please see here . 

OData Client for Service Layer **Stream** 

**48** PUBLIC 

## **Image Upload** 

```
// POST /b1s/v2/Attachments2
 Attachments2 attachment = new Attachments2();
slContext.AddToAttachments2(attachment);
string path = Path.GetDirectoryName(Assembly.GetExecutingAssembly().Location);
string imageFile = path + @"\..\..\..\stream\images\SAP-logo.jpg";
// Open an image file and save it as a stream.
FileStream imageStream = new FileStream(imageFile, FileMode.Open);
slContext.SetSaveStream(attachment, imageStream, true, "image/jpeg",
"SAP.jpg");// image/jpeg => jpeg jpg jpe
// Upload the file and get the response.
ChangeOperationResponse changeResponse =
slContext.SaveChanges().FirstOrDefault() as ChangeOperationResponse;
// Get the entity created on the service and check if the entity is as expected.
var entityDescriptor = changeResponse.Descriptor as EntityDescriptor;
Uri editLink = entityDescriptor.EditLink;
Regex regex = new Regex(@"/b1s/v2/attachments2\((?<entry>\d+)\)",
RegexOptions.IgnoreCase);
Match match = regex.Match(editLink.LocalPath);
 return match.Success ? Convert.ToInt32(match.Groups["entry"].Value) : 0;
```

Capture the request and you will find that the Slug header is there to indicate the file name. 

```
POST https://servicelayerhost:50000/b1s/v2/Attachments2 HTTP/1.1
 Slug: images2.jpg
OData-Version: 4.0
OData-MaxVersion: 4.0
Accept: application/json;odata.metadata=minimal;
Accept-Charset: UTF-8
User-Agent: Microsoft.OData.Client/7.9.0
Cookie: B1SESSION=3a8f8e84-e1f4-11eb-8000-0a0027000008;HttpOnly;
Connection: Keep-Alive
Content-Type: image/jpeg
Host: servicelayerhost:50000
Content-Length: 6315
 <the binary content of an image>
```

## **Text Upload** 

```
// POST /b1s/v2/Attachments2
 Attachments2 attachment = new Attachments2();
slContext.AddToAttachments2(attachment);
// Open a text file and save it as a stream
string path = Path.GetDirectoryName(Assembly.GetExecutingAssembly().Location);
string textFile = path + @"\..\..\..\stream\text\test.txt";
FileStream textStream = new FileStream(textFile, FileMode.Open);
slContext.SetSaveStream(attachment, textStream, true, "text/plain",
"testAlias.txt");
// Upload the file and get the response.
ChangeOperationResponse changeResponse =
slContext.SaveChanges().FirstOrDefault() as ChangeOperationResponse;
// Get the entity created on the service and check if the entity is as expected.
var entityDescriptor = changeResponse.Descriptor as EntityDescriptor;
Uri editLink = entityDescriptor.EditLink;
Regex regex = new Regex(@"/b1s/v2/attachments2\((?<entry>\d+)\)",
RegexOptions.IgnoreCase);
Match match = regex.Match(editLink.LocalPath);
 return match.Success ? Convert.ToInt32(match.Groups["entry"].Value) : 0;
```

OData Client for Service Layer **Stream** 

PUBLIC **49** 

## **13.2 Downloading Images and Texts** 

`DataServiceContext` provides `GetReadStream` to support requesting the binary data stream that belongs to the requested entity. 

## **Image Download** 

```
// GET /b1s/v2/Attachments2(entry)
 var attachment = slContext.Attachments2.Where(c => c.AbsoluteEntry ==
entry).Single();
// GET /b1s/v2/Attachments2(entry)/$value
DataServiceStreamResponse dataServiceStreamResponse  =
slContext.GetReadStream(attachment);
string contentDisposition = dataServiceStreamResponse.ContentDisposition;
Console.Out.WriteLine(contentDisposition);
```

```
// Assume AbsoluteEntry = entry is an attachment with image type, save it to a
local file.
```

```
using (Stream outStream = File.OpenWrite("picture.jpg"))
{
```

```
    dataServiceStreamResponse.Stream.CopyTo(outStream);
 }
```

## **Text Download** 

```
// GET /b1s/v2/Attachments2(entry)
 var attachment = slContext.Attachments2.Where(c => c.AbsoluteEntry ==
entry).Single();
// GET /b1s/v2/Attachments2(entry)/$value
DataServiceStreamResponse dataServiceStreamResponse =
slContext.GetReadStream(attachment);
string contentDisposition = dataServiceStreamResponse.ContentDisposition;
Console.Out.WriteLine(contentDisposition);
// Assume AbsoluteEntry = entry is an attachment with text type.
StreamReader reader = new StreamReader(dataServiceStreamResponse.Stream, true);
var content = reader.ReadToEnd();
Console.WriteLine(content);
// Save it to a local file
byte[] bytes = Encoding.UTF8.GetBytes(content);
 File.WriteAllBytes("text.txt", bytes);
```

OData Client for Service Layer **Stream** 

PUBLIC 

**50** 

## **Important Disclaimers and Legal Information** 

## **Hyperlinks** 

Some links are classified by an icon and/or a mouseover text. These links provide additional information. About the icons: 

- Links with the icon : You are entering a Web site that is not hosted by SAP. By using such links, you agree (unless expressly stated otherwise in your agreements with SAP) to this: 

   - The content of the linked-to site is not SAP documentation. You may not infer any product claims against SAP based on this information. 

   - SAP does not agree or disagree with the content on the linked-to site, nor does SAP warrant the availability and correctness. SAP shall not be liable for any damages caused by the use of such content unless damages have been caused by SAP's gross negligence or willful misconduct. 

- Links with the icon : You are leaving the documentation for that particular SAP product or service and are entering an SAP-hosted Web site. By using such links, you agree that (unless expressly stated otherwise in your agreements with SAP) you may not infer any product claims against SAP based on this information. 

## **Videos Hosted on External Platforms** 

Some videos may point to third-party video hosting platforms. SAP cannot guarantee the future availability of videos stored on these platforms. Furthermore, any advertisements or other content hosted on these platforms (for example, suggested videos or by navigating to other videos hosted on the same site), are not within the control or responsibility of SAP. 

## **Beta and Other Experimental Features** 

Experimental features are not part of the officially delivered scope that SAP guarantees for future releases. This means that experimental features may be changed by SAP at any time for any reason without notice. Experimental features are not for productive use. You may not demonstrate, test, examine, evaluate or otherwise use the experimental features in a live operating environment or with data that has not been sufficiently backed up. 

The purpose of experimental features is to get feedback early on, allowing customers and partners to influence the future product accordingly. By providing your feedback (e.g. in the SAP Community), you accept that intellectual property rights of the contributions or derivative works shall remain the exclusive property of SAP. 

## **Example Code** 

Any software coding and/or code snippets are examples. They are not for productive use. The example code is only intended to better explain and visualize the syntax and phrasing rules. SAP does not warrant the correctness and completeness of the example code. SAP shall not be liable for errors or damages caused by the use of example code unless damages have been caused by SAP's gross negligence or willful misconduct. 

## **Bias-Free Language** 

SAP supports a culture of diversity and inclusion. Whenever possible, we use unbiased language in our documentation to refer to people of all cultures, ethnicities, genders, and abilities. 

OData Client for Service Layer **Important Disclaimers and Legal Information** 

PUBLIC **51** 

www.sap.com/contactsap 

© 2024 SAP SE or an SAP affiliate company. All rights reserved. 

No part of this publication may be reproduced or transmitted in any form or for any purpose without the express permission of SAP SE or an SAP affiliate company. The information contained herein may be changed without prior notice. 

Some software products marketed by SAP SE and its distributors contain proprietary software components of other software vendors. National product specifications may vary. 

These materials are provided by SAP SE or an SAP affiliate company for informational purposes only, without representation or warranty of any kind, and SAP or its affiliated companies shall not be liable for errors or omissions with respect to the materials. The only warranties for SAP or SAP affiliate company products and services are those that are set forth in the express warranty statements accompanying such products and services, if any. Nothing herein should be construed as constituting an additional warranty. 

SAP and other SAP products and services mentioned herein as well as their respective logos are trademarks or registered trademarks of SAP SE (or an SAP affiliate company) in Germany and other countries. All other product and service names mentioned are the trademarks of their respective companies. 

Please see https://www.sap.com/about/legal/trademark.html for additional trademark information and notices. 

**==> picture [58 x 29] intentionally omitted <==**

**THE BEST RUN** 

