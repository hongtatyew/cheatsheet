1. Create enum with different string value:

```csharp
public enum CredentialsMethod {
    /// <summary>
    /// None - no auth required
    /// </summary>
    [EnumMember(Value = "none")] None,

    /// <summary>
    /// API Bearer Token header required
    /// </summary>
    [EnumMember(Value = "api_token")] ApiToken,

    /// <summary>
    /// Client ID, Secret, API Token Issuer and Audience for client credential flow required
    /// </summary>
    [EnumMember(Value = "client_credentials")] ClientCredentials,
}
```