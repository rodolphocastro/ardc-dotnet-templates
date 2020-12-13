# 🆕 ARDC Templates

## ❓ What is ARDC Templates?

`ARDC.Commons.Templates` is a collection for common files for a coding project.

Currently the following templates are available:

1. README.md (A simple readme written in Markdown)
2. MIT License (A LICENSE file containing the MIT License)
3. GNU GPL v3 License (A LICENSE file containing the GNU GPL v3 License)

## ⚡ Getting Started

In order to install run the following command on your shell:

```
dotnet new --install ARDC.Commons.Templates
```

This command will download and install the templates contained in this repository.

Finally, to scaffold a file based on one of those templates, run `dotnet new TEMPLATE-NAME`.

### ❌ Uninstalling

In case you wish to uninstall these templates run the following command on your shell:

```
dotnet new --uninstall ARDC.Commons.Templates
```

## 🔧 Building and Running

### 🔨 Build the Project

Since this is a template project all you need to do is run `dotnet new -i .\src\` on the root of this project and all the templates will be installed locally for you to use and test.

When you're done you can run `dotnet new --debug:reinit` to remove those packages from the templates you've installed for `dotnet new`.

### 📦 Publishing to NuGet

Simply run `dotnet pack --configuration Release -o ./pkgs/` to create a NuGet package (`.nupkg` file) in the `./pkgs/` directory.

Then run `dotnet nuget push "**/*.nupkg" --api-key yourApiKey --source https://api.nuget.org/v3/index.json` to push the packages into [NuGet.org](https://www.nuget.org/).

## 🙏 Thanks

### Choose a License

License files are based on the great work done by [Choose a License](https://choosealicense.com/).

## 🤝 Collaborate with ARDC Templates

Read-up on Microsoft's docs for creating templates for `dotnet new`, available [here](https://docs.microsoft.com/en-us/dotnet/core/tools/custom-templates).

Then all you need to do is fork this repository, create your template and submit a pull request 🙂.