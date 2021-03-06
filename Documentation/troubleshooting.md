# Troubleshooting Issues with .NET Install Tool for Extension Authors

## Install Script Timeouts

Please note that, depending on your network speed, installing the .NET Core runtime might take some time. By default, the installation terminates unsuccessfully if it takes longer than 2 minutes to finish. If you believe this is too little (or too much) time to allow for the download, you can change the timeout value by setting `dotnetAcquisitionExtension.installTimeoutValue` to a custom value.

Learn more about configuring Visual Studio Code settings [here](https://code.visualstudio.com/docs/getstarted/settings) and see below for an example of a custom timeout in a `settings.json` file. In this example the custom timeout value is 180 seconds, or 3 minutes.

```json
{
    "dotnetAcquisitionExtension.installTimeoutValue": 180
}
```

## Other Issues

Haven't found a solution? Check out our [open issues](https://github.com/dotnet/vscode-dotnet-runtime/issues). If you don't see your issue there, please file a new issue by evoking the `.NET Install Tool: Report an issue with the .NET Install Tool for Extension Authors` command from Visual Studio Code.