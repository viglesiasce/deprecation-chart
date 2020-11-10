# deprecation-chart

This chart is used to point users in the right direction when the Helm Charts repo is turned down.

It requires a value that is not set, thus failing to install but printing a useful error message.

## Example output

```shell
 $  helm install . --generate-name
Error: template: deprecation/templates/NOTES.txt:10:3: executing "deprecation/templates/NOTES.txt" at <fail "\n*******************************************************\n* This chart location is deprecated. Learn more here: *\n* https://helm.sh/blog/charts-repo-deprecation/       *\n*******************************************************\n">: error calling fail:
*******************************************************
* This chart location is depreacted. Learn more here: *
* https://helm.sh/blog/charts-repo-deprecation/       *
*******************************************************
```
