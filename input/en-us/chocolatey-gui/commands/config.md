---
Order: 10
xref: gui-config-command
Title: Config
Description: Usage instructions on how to list/get/set/unset Chocolatey GUI config settings.
---

Chocolatey GUI will allow you to interact with the config settings.

## Usage

```powershell
chocolateyguicli config [list]|get|set|unset [<options/switches]
```

## Examples

```powershell
chocolateyguicli config
chocolateyguicli config list
chocolateyguicli config get --name="'outdatedPackagesCacheDurationInMinutes'"
chocolateyguicli config set --name="'outdatedPackagesCacheDurationInMinutes'" --value="'60'"
chocolateyguicli config unset --name="'outdatedPackagesCacheDurationInMinutes'"
```

## Exit Codes

Exit codes that normally result from running this command.

Normal:

- 0: operation was successful, no issues detected
- -1 or 1: an error has occurred

## Options and Switches

```powershell
-?, --help, -h
     Prints out the help menu.

-r, --limitoutput, --limit-output
     Limit the output to essential information

    --name=VALUE
     Name - the name of the config setting. Required with some actions.

    --value=VALUE
     Value - the value of the config setting.  Required with some actions.

-g, --global
     Should the command be applied to the global (machine) level?  Defaults
       to false.
```

## Resources

Below is a short video which shows this in action:

## Configuration Options

The available items that can be configured are:

<?! Include "../../../shared/available-settings.txt" /?>
