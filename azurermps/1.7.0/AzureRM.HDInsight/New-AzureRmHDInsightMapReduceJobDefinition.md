---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/New-AzureRmHDInsightMapReduceJobDefinition.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/New-AzureRmHDInsightMapReduceJobDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: hdinsight
---

# New-AzureRmHDInsightMapReduceJobDefinition

## SYNOPSIS
Creates a MapReduce job object.

## SYNTAX

```
New-AzureRmHDInsightMapReduceJobDefinition [-Arguments <String[]>] [-Files <String[]>] [-StatusFolder <String>]
 -ClassName <String> [-Defines <Hashtable>] -JarFile <String> [-JobName <String>] [-LibJars <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The New-AzureRmHDInsightMapReduceJobDefinition cmdlet defines a new MapReduce job for use with an Azure HDInsight cluster.

## EXAMPLES

### --------------------------  Example 1: Create a MapReduce job definition  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\&gt; # Cluster info
        $clusterName = "your-hadoop-001"
        $clusterCreds = Get-Credential

        New-AzureRmHDInsightMapReduceJobDefinition -StatusFolder $statusFolder `
            -ClassName $className `
            -JarFile $jarFilePath `
        | Start-AzureRmHDInsightJob 
            -ClusterName $clusterName `
            -ClusterCredential $clusterCreds
```

This command creates a MapReduce job definition.

## PARAMETERS

### -Arguments
Specifies an array of arguments for the job.
The arguments are passed as command-line arguments to each task.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClassName
Specifies the job class in the JAR file.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Defines
Specifies Hadoop configuration values to set for when the job runs.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Files
Specifies a collection of files that are associated with a Hive job.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JarFile
Specifies the JAR file to use for the jobDetails.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobName
Specifies the name of the job.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LibJars
Specifies the lib JARS for the job.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StatusFolder
Specifies the location of the folder that contains standard outputs and error outputs for a job.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, hadoop, hdinsight, hd, insight

## RELATED LINKS

[Start-AzureRmHDInsightJob]()

