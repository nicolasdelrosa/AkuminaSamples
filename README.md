This sample provides customer to write custom token store for storing graph/SharePoint tokens.

To run this sample download or clone repository, compile the source then copy the assembly Akumina.Samples.TokenStore.dll to your AppManager website bin folder

If you run the sample as it is, then update the UNITY.CONFIG as shown below

 &lt;register type="IRepository[UserToken]" mapTo="AzureTableTokenStore" /&gt;
 
 TO
 
 &lt;register type="IRepository[UserToken]" mapTo="Akumina.Samples.TokenStore.NtFileTokenStore, Akumina.Samples.TokenStore" /&gt;
 
 NOTE:  This sample has path hard coded to c:\\Temp\\ , change this path to your desired path before compilation.
