---
applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016
schema: 2.0.0
---

# Get-IPBlockListConfig

## SYNOPSIS
!!! Exchange Server 2010

Use the Get-IPBlockListConfig cmdlet to view the configuration information for the IP Block list configuration on a computer that has the Edge Transport server role or the Hub Transport server role installed.

!!! Exchange Server 2013

This cmdlet is available or effective only on Edge Transport servers in on-premises Exchange Server 2013.

Use the Get-IPBlockListConfig cmdlet to view the IP Block list configuration information that's used by the Connection Filtering agent on Edge Transport servers.

!!! Exchange Server 2016

This cmdlet is available or effective only on Edge Transport servers in on-premises Exchange.

Use the Get-IPBlockListConfig cmdlet to view the IP Block list configuration information that's used by the Connection Filtering agent on Edge Transport servers.

## SYNTAX

```
Get-IPBlockListConfig [-DomainController <Fqdn>] [<CommonParameters>]
```

## DESCRIPTION
!!! Exchange Server 2010

The IP Block list configuration is used by the Connection Filter agent. The Connection Filter agent acts on the IP address of the remote server that initiates the SMTP connection to determine what action, if any, to take on an incoming message.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Anti-spam features" entry in the Transport Permissions topic.

!!! Exchange Server 2013

On Edge Transport servers, the Connection Filtering agent acts on the incoming SMTP connection to determine what action, if any, to take on an incoming message.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Anti-spam features - Edge Transport" entry in the Anti-spam and anti-malware permissions topic.

!!! Exchange Server 2016

On Edge Transport servers, the Connection Filtering agent acts on the incoming SMTP connection to determine what action, if any, to take on an incoming message.

On Edge Transport servers, you need to be a member of the local Administrators group to run this cmdlet.

## EXAMPLES

### Example 1 -------------------------- (Exchange Server 2010)
```
Get-IPBlockListConfig | Format-List
```

This example returns detailed information about the IP Block list configuration for the computer on which the command is run.

### Example 1 -------------------------- (Exchange Server 2013)
```
Get-IPBlockListConfig | Format-List
```

This example returns detailed information about the IP Block list configuration on the local Edge Transport server.

### Example 1 -------------------------- (Exchange Server 2016)
```
Get-IPBlockListConfig | Format-List
```

This example returns detailed information about the IP Block list configuration on the local Edge Transport server.

## PARAMETERS

### -DomainController
The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.

The DomainController parameter isn't supported on Edge Transport servers. An Edge Transport server uses the local instance of Active Directory Lightweight Directory Services (AD LDS) to read and write data.

```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  
To see the input types that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Input Type field for a cmdlet is blank, the cmdlet doesn't accept input data.

## OUTPUTS

###  
To see the return types, which are also known as output types, that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Output Type field is blank, the cmdlet doesn't return data.

## NOTES

## RELATED LINKS

[Online Version](https://technet.microsoft.com/library/7c2b9f46-00a0-4303-b19d-dbae010205e0.aspx)

