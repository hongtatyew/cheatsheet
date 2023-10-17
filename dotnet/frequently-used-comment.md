# Dotnet
## Program.cs 
### Class
```csharp
/// <summary>
/// This is the main class of the program, which serves as the entry point and starting point for the program's logic.
/// </summary>
```

### Main
```csharp
/// <summary>
/// This is the entry point of the program, which is executed when the program is started.
/// </summary>
/// <param name="args">The <see cref="args"/>.</param>
/// <returns>A task representing the asynchronous operation.</returns>
```

# Carrier
## EventHandler
### Constructor
```csharp
/// <summary>
/// Create an instance of <see cref="TokenRevocationRequestedEventHandler"/>.
/// </summary>
/// <param name="logger">The <see cref="ILogger&lt;TokenRevocationRequestedEventHandler&gt;"/></param>
/// <param name="tokenRepository">The <see cref="ITokenRepository"/></param>
/// <param name="successEventPublisher">The <see cref="IEventPublisher&lt;RevokeTokenSuccessIntegrationEvent&gt;"/></param>
/// <param name="failureEventPublisher">The <see cref="IEventPublisher&lt;RevokeTokenFailureIntegrationEvent&gt;"/></param>
```

### HandleAsync
```csharp
/// <summary>
/// A method to handle events that are raised when a token revocation is requested.
/// </summary>
/// <param name="event">An instance of the <see cref="TokenRevocationRequestedEvent"/> class, which contains information about the token revocation request.</param>
/// <param name="cancellationToken">The <see cref="CancellationToken"/>.</param>
/// <returns>A task representing the asynchronous operation.</returns>
```
