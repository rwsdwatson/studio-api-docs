Deployment
===

This section explains how plug-ins should be deployed and how plug-in deployment can be customized.




Deployment
----
Copy the plug-in manifest and plug-in resources files into the plugins folder, and copy the plug-in assembly into the application directory. There is no central configuration file which needs to be updated.

Customizing Plug-in Deployment
----
By default, plug-in manifest files and plug-in resource files are deployed in a “plugins" subdirectory of the application directory. Where the plug-in manifests and plug-in resources are retrieved from is determined by the plug-in locator, represented by the [IPluginLocator](../../api/core/Sdl.Core.PluginFramework.IPluginLocator.yml) interface.

The plug-in framework provides a standard plug-in locator implementation which loads plug-ins from a directory on the local file system **FileSystemPluginLocator**

When creating a plug-in registry instance, you can pass a custom plug-in locator object, which for instance gets plug-in manifest info from a database or web server.

> [!NOTE]
> 
> This content may be out-of-date. To check the latest information on this topic, inspect the libraries using the Visual Studio Object Browser.