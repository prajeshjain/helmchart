# DevOps Assignment - 3
## Helm Chart
This is the helm chart created for the assignment using nginx image. All environments variables can be provided throught ConfigMaps and rest configurations can be provided through 'values.yml' file.

## Installing the chart
First we need to clone this repo, after switching to it, we need to execute following command to create the chart,
```
helm install <release-name> pwachart
````
## Uninstalling the chart
To uninstall the installed chart, execute following command,
```
helm uninstall <release-name>
```
## Upgrading the Chart
The chart can be upgraded to a newer release using following command,
```
helm upgrade -i <release-name> pwachart
```
### NOTE
Check the node affinity in values.yml so as to label the nodes accordingly.