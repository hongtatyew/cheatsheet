## Validation

### Method 1

```csharp
public record OpenFgaOptions
{
    public const string Position = "OpenFga";
    public string ApiHost { get; set; } = string.Empty;
}

var openFgaOptions = configuration
  .GetSection(OpenFgaOptions.Position)
  .Get<OpenFgaOptions>() ?? new OpenFgaOptions();

ArgumentException.ThrowIfNullOrEmpty(openFgaOptions.ApiHost);
```

### Method 2

```csharp
public record OpenFgaOptions
{
    public const string Position = "OpenFga";
    [Required(AllowEmptyStrings = false)]
    public string ApiScheme { get; set; } = "http";
    [Required(AllowEmptyStrings = false)]
    public string ApiHost { get; set; } = string.Empty;
    [Required(AllowEmptyStrings = false)]
    public string StoreId { get; set; } = string.Empty;
}
```

```csharp
var openFgaConfigurationSection = configuration.GetSection(OpenFgaOptions.Position);
services
    .AddOptions<OpenFgaOptions>()
    .Bind(openFgaConfigurationSection)
    .ValidateDataAnnotations()
    .ValidateOnStart();

var openFgaOptions = openFgaConfigurationSection.Get<OpenFgaOptions>() ?? new OpenFgaOptions();
```

### Method 3

Available in dotnet 8
To do: Study how to use this

https://github.com/dotnet/apireviews/blob/01c4d04906878e32cda367c95af96e55469f40c6/2023/07-25-quick-reviews/README.md#add-extensions-to-create-an-optionsbuilder-with-validateonstart-support

```csharp
services
  .AddOptionsWithValidateOnStart<HttpTracingOptions, HttpTracingOptionsValidator>()
  .Bind(section)
```
