# Anjo.GoogleAndroid.Libraries.Identity.GoogleId
 
GoogleAndroid Libraries Identity GoogleId SDK for .NET for Android (formerly Xamarin.Android) Binding Library - Wael Anjo
---------------------------------

[![NuGet](https://buildstats.info/nuget/Anjo.GoogleAndroid.Libraries.Identity.GoogleId)](https://www.nuget.org/packages/Anjo.GoogleAndroid.Libraries.Identity.GoogleId)
[![License](https://img.shields.io/github/license/mhdwaelanjo/Anjo.GoogleAndroid.Libraries.Identity.GoogleId)](https://github.com/mhdwaelanjo/Anjo.GoogleAndroid.Libraries.Identity.GoogleId/blob/master/LICENSE)
 
---------------------------------
### How To Use
  
```c#
private string ClientId = "";
private ICredentialManagerCallback Callback;

GetGoogleIdOption googleIdOption = new GetGoogleIdOption.Builder()
    .SetFilterByAuthorizedAccounts(false)
    .SetServerClientId(ClientId)
    .SetAutoSelectEnabled(false)
    .Build();

GetCredentialRequest request = new GetCredentialRequest.Builder()
    .AddCredentialOption(googleIdOption)
    .Build();

CancellationSignal cancellationSignal = new CancellationSignal();
CredentialManager ??= ICredentialManager.Create(context);
IExecutor executor = ContextCompat.GetMainExecutor(context);

CredentialManager.GetCredentialAsync(context, request, cancellationSignal, executor, Callback);
```

Star on Github if this project helps you: https://github.com/mhdwaelanjo/Anjo.GoogleAndroid.Libraries.Identity.GoogleId
 
---------------------------------
### Help & Feedback:
- You can subscribe to the channel on the telegram [Anjo Help & Feedback](https://t.me/mhwaelanjo) to learn about the latest updates to my packages on [Nuget.com](https://www.nuget.org/profiles/MHWAELANJO)

### SUPPORT:
- ☕ Buy me a coffee: [By PayPal](https://www.paypal.com/paypalme/mhwaelanjo)