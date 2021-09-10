# AWS::RDS::DBInstance

The AWS::RDS::DBInstance resource creates an Amazon RDS DB instance.

## Syntax

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON

<pre>
{
    "Type" : "AWS::RDS::DBInstance",
    "Properties" : {
        "<a href="#allocatedstorage" title="AllocatedStorage">AllocatedStorage</a>" : <i>String</i>,
        "<a href="#allowmajorversionupgrade" title="AllowMajorVersionUpgrade">AllowMajorVersionUpgrade</a>" : <i>Boolean</i>,
        "<a href="#associatedroles" title="AssociatedRoles">AssociatedRoles</a>" : <i>[ <a href="dbinstancerole.md">DBInstanceRole</a>, ... ]</i>,
        "<a href="#autominorversionupgrade" title="AutoMinorVersionUpgrade">AutoMinorVersionUpgrade</a>" : <i>Boolean</i>,
        "<a href="#availabilityzone" title="AvailabilityZone">AvailabilityZone</a>" : <i>String</i>,
        "<a href="#backupretentionperiod" title="BackupRetentionPeriod">BackupRetentionPeriod</a>" : <i>Integer</i>,
        "<a href="#cacertificateidentifier" title="CACertificateIdentifier">CACertificateIdentifier</a>" : <i>String</i>,
        "<a href="#charactersetname" title="CharacterSetName">CharacterSetName</a>" : <i>String</i>,
        "<a href="#copytagstosnapshot" title="CopyTagsToSnapshot">CopyTagsToSnapshot</a>" : <i>Boolean</i>,
        "<a href="#dbclusteridentifier" title="DBClusterIdentifier">DBClusterIdentifier</a>" : <i>String</i>,
        "<a href="#dbinstanceclass" title="DBInstanceClass">DBInstanceClass</a>" : <i>String</i>,
        "<a href="#dbinstanceidentifier" title="DBInstanceIdentifier">DBInstanceIdentifier</a>" : <i>String</i>,
        "<a href="#dbname" title="DBName">DBName</a>" : <i>String</i>,
        "<a href="#dbparametergroupname" title="DBParameterGroupName">DBParameterGroupName</a>" : <i>String</i>,
        "<a href="#dbsecuritygroups" title="DBSecurityGroups">DBSecurityGroups</a>" : <i>[ String, ... ]</i>,
        "<a href="#dbsnapshotidentifier" title="DBSnapshotIdentifier">DBSnapshotIdentifier</a>" : <i>String</i>,
        "<a href="#dbsubnetgroupname" title="DBSubnetGroupName">DBSubnetGroupName</a>" : <i>String</i>,
        "<a href="#deleteautomatedbackups" title="DeleteAutomatedBackups">DeleteAutomatedBackups</a>" : <i>Boolean</i>,
        "<a href="#deletionprotection" title="DeletionProtection">DeletionProtection</a>" : <i>Boolean</i>,
        "<a href="#domain" title="Domain">Domain</a>" : <i>String</i>,
        "<a href="#domainiamrolename" title="DomainIAMRoleName">DomainIAMRoleName</a>" : <i>String</i>,
        "<a href="#enablecloudwatchlogsexports" title="EnableCloudwatchLogsExports">EnableCloudwatchLogsExports</a>" : <i>[ String, ... ]</i>,
        "<a href="#enableiamdatabaseauthentication" title="EnableIAMDatabaseAuthentication">EnableIAMDatabaseAuthentication</a>" : <i>Boolean</i>,
        "<a href="#enableperformanceinsights" title="EnablePerformanceInsights">EnablePerformanceInsights</a>" : <i>Boolean</i>,
        "<a href="#endpoint" title="Endpoint">Endpoint</a>" : <i><a href="endpoint.md">Endpoint</a></i>,
        "<a href="#engine" title="Engine">Engine</a>" : <i>String</i>,
        "<a href="#engineversion" title="EngineVersion">EngineVersion</a>" : <i>String</i>,
        "<a href="#iops" title="Iops">Iops</a>" : <i>Integer</i>,
        "<a href="#kmskeyid" title="KmsKeyId">KmsKeyId</a>" : <i>String</i>,
        "<a href="#licensemodel" title="LicenseModel">LicenseModel</a>" : <i>String</i>,
        "<a href="#masterusername" title="MasterUsername">MasterUsername</a>" : <i>String</i>,
        "<a href="#masteruserpassword" title="MasterUserPassword">MasterUserPassword</a>" : <i>String</i>,
        "<a href="#maxallocatedstorage" title="MaxAllocatedStorage">MaxAllocatedStorage</a>" : <i>Integer</i>,
        "<a href="#monitoringinterval" title="MonitoringInterval">MonitoringInterval</a>" : <i>Integer</i>,
        "<a href="#monitoringrolearn" title="MonitoringRoleArn">MonitoringRoleArn</a>" : <i>String</i>,
        "<a href="#multiaz" title="MultiAZ">MultiAZ</a>" : <i>Boolean</i>,
        "<a href="#optiongroupname" title="OptionGroupName">OptionGroupName</a>" : <i>String</i>,
        "<a href="#performanceinsightskmskeyid" title="PerformanceInsightsKMSKeyId">PerformanceInsightsKMSKeyId</a>" : <i>String</i>,
        "<a href="#performanceinsightsretentionperiod" title="PerformanceInsightsRetentionPeriod">PerformanceInsightsRetentionPeriod</a>" : <i>Integer</i>,
        "<a href="#port" title="Port">Port</a>" : <i>Integer</i>,
        "<a href="#preferredbackupwindow" title="PreferredBackupWindow">PreferredBackupWindow</a>" : <i>String</i>,
        "<a href="#preferredmaintenancewindow" title="PreferredMaintenanceWindow">PreferredMaintenanceWindow</a>" : <i>String</i>,
        "<a href="#processorfeatures" title="ProcessorFeatures">ProcessorFeatures</a>" : <i>[ <a href="processorfeature.md">ProcessorFeature</a>, ... ]</i>,
        "<a href="#promotiontier" title="PromotionTier">PromotionTier</a>" : <i>Integer</i>,
        "<a href="#publiclyaccessible" title="PubliclyAccessible">PubliclyAccessible</a>" : <i>Boolean</i>,
        "<a href="#sourcedbinstanceidentifier" title="SourceDBInstanceIdentifier">SourceDBInstanceIdentifier</a>" : <i>String</i>,
        "<a href="#sourceregion" title="SourceRegion">SourceRegion</a>" : <i>String</i>,
        "<a href="#storageencrypted" title="StorageEncrypted">StorageEncrypted</a>" : <i>Boolean</i>,
        "<a href="#storagetype" title="StorageType">StorageType</a>" : <i>String</i>,
        "<a href="#tags" title="Tags">Tags</a>" : <i>[ <a href="tag.md">Tag</a>, ... ]</i>,
        "<a href="#tdecredentialarn" title="TdeCredentialArn">TdeCredentialArn</a>" : <i>String</i>,
        "<a href="#tdecredentialpassword" title="TdeCredentialPassword">TdeCredentialPassword</a>" : <i>String</i>,
        "<a href="#timezone" title="Timezone">Timezone</a>" : <i>String</i>,
        "<a href="#usedefaultprocessorfeatures" title="UseDefaultProcessorFeatures">UseDefaultProcessorFeatures</a>" : <i>Boolean</i>,
        "<a href="#vpcsecuritygroups" title="VPCSecurityGroups">VPCSecurityGroups</a>" : <i>[ String, ... ]</i>
    }
}
</pre>

### YAML

<pre>
Type: AWS::RDS::DBInstance
Properties:
    <a href="#allocatedstorage" title="AllocatedStorage">AllocatedStorage</a>: <i>String</i>
    <a href="#allowmajorversionupgrade" title="AllowMajorVersionUpgrade">AllowMajorVersionUpgrade</a>: <i>Boolean</i>
    <a href="#associatedroles" title="AssociatedRoles">AssociatedRoles</a>: <i>
      - <a href="dbinstancerole.md">DBInstanceRole</a></i>
    <a href="#autominorversionupgrade" title="AutoMinorVersionUpgrade">AutoMinorVersionUpgrade</a>: <i>Boolean</i>
    <a href="#availabilityzone" title="AvailabilityZone">AvailabilityZone</a>: <i>String</i>
    <a href="#backupretentionperiod" title="BackupRetentionPeriod">BackupRetentionPeriod</a>: <i>Integer</i>
    <a href="#cacertificateidentifier" title="CACertificateIdentifier">CACertificateIdentifier</a>: <i>String</i>
    <a href="#charactersetname" title="CharacterSetName">CharacterSetName</a>: <i>String</i>
    <a href="#copytagstosnapshot" title="CopyTagsToSnapshot">CopyTagsToSnapshot</a>: <i>Boolean</i>
    <a href="#dbclusteridentifier" title="DBClusterIdentifier">DBClusterIdentifier</a>: <i>String</i>
    <a href="#dbinstanceclass" title="DBInstanceClass">DBInstanceClass</a>: <i>String</i>
    <a href="#dbinstanceidentifier" title="DBInstanceIdentifier">DBInstanceIdentifier</a>: <i>String</i>
    <a href="#dbname" title="DBName">DBName</a>: <i>String</i>
    <a href="#dbparametergroupname" title="DBParameterGroupName">DBParameterGroupName</a>: <i>String</i>
    <a href="#dbsecuritygroups" title="DBSecurityGroups">DBSecurityGroups</a>: <i>
      - String</i>
    <a href="#dbsnapshotidentifier" title="DBSnapshotIdentifier">DBSnapshotIdentifier</a>: <i>String</i>
    <a href="#dbsubnetgroupname" title="DBSubnetGroupName">DBSubnetGroupName</a>: <i>String</i>
    <a href="#deleteautomatedbackups" title="DeleteAutomatedBackups">DeleteAutomatedBackups</a>: <i>Boolean</i>
    <a href="#deletionprotection" title="DeletionProtection">DeletionProtection</a>: <i>Boolean</i>
    <a href="#domain" title="Domain">Domain</a>: <i>String</i>
    <a href="#domainiamrolename" title="DomainIAMRoleName">DomainIAMRoleName</a>: <i>String</i>
    <a href="#enablecloudwatchlogsexports" title="EnableCloudwatchLogsExports">EnableCloudwatchLogsExports</a>: <i>
      - String</i>
    <a href="#enableiamdatabaseauthentication" title="EnableIAMDatabaseAuthentication">EnableIAMDatabaseAuthentication</a>: <i>Boolean</i>
    <a href="#enableperformanceinsights" title="EnablePerformanceInsights">EnablePerformanceInsights</a>: <i>Boolean</i>
    <a href="#endpoint" title="Endpoint">Endpoint</a>: <i><a href="endpoint.md">Endpoint</a></i>
    <a href="#engine" title="Engine">Engine</a>: <i>String</i>
    <a href="#engineversion" title="EngineVersion">EngineVersion</a>: <i>String</i>
    <a href="#iops" title="Iops">Iops</a>: <i>Integer</i>
    <a href="#kmskeyid" title="KmsKeyId">KmsKeyId</a>: <i>String</i>
    <a href="#licensemodel" title="LicenseModel">LicenseModel</a>: <i>String</i>
    <a href="#masterusername" title="MasterUsername">MasterUsername</a>: <i>String</i>
    <a href="#masteruserpassword" title="MasterUserPassword">MasterUserPassword</a>: <i>String</i>
    <a href="#maxallocatedstorage" title="MaxAllocatedStorage">MaxAllocatedStorage</a>: <i>Integer</i>
    <a href="#monitoringinterval" title="MonitoringInterval">MonitoringInterval</a>: <i>Integer</i>
    <a href="#monitoringrolearn" title="MonitoringRoleArn">MonitoringRoleArn</a>: <i>String</i>
    <a href="#multiaz" title="MultiAZ">MultiAZ</a>: <i>Boolean</i>
    <a href="#optiongroupname" title="OptionGroupName">OptionGroupName</a>: <i>String</i>
    <a href="#performanceinsightskmskeyid" title="PerformanceInsightsKMSKeyId">PerformanceInsightsKMSKeyId</a>: <i>String</i>
    <a href="#performanceinsightsretentionperiod" title="PerformanceInsightsRetentionPeriod">PerformanceInsightsRetentionPeriod</a>: <i>Integer</i>
    <a href="#port" title="Port">Port</a>: <i>Integer</i>
    <a href="#preferredbackupwindow" title="PreferredBackupWindow">PreferredBackupWindow</a>: <i>String</i>
    <a href="#preferredmaintenancewindow" title="PreferredMaintenanceWindow">PreferredMaintenanceWindow</a>: <i>String</i>
    <a href="#processorfeatures" title="ProcessorFeatures">ProcessorFeatures</a>: <i>
      - <a href="processorfeature.md">ProcessorFeature</a></i>
    <a href="#promotiontier" title="PromotionTier">PromotionTier</a>: <i>Integer</i>
    <a href="#publiclyaccessible" title="PubliclyAccessible">PubliclyAccessible</a>: <i>Boolean</i>
    <a href="#sourcedbinstanceidentifier" title="SourceDBInstanceIdentifier">SourceDBInstanceIdentifier</a>: <i>String</i>
    <a href="#sourceregion" title="SourceRegion">SourceRegion</a>: <i>String</i>
    <a href="#storageencrypted" title="StorageEncrypted">StorageEncrypted</a>: <i>Boolean</i>
    <a href="#storagetype" title="StorageType">StorageType</a>: <i>String</i>
    <a href="#tags" title="Tags">Tags</a>: <i>
      - <a href="tag.md">Tag</a></i>
    <a href="#tdecredentialarn" title="TdeCredentialArn">TdeCredentialArn</a>: <i>String</i>
    <a href="#tdecredentialpassword" title="TdeCredentialPassword">TdeCredentialPassword</a>: <i>String</i>
    <a href="#timezone" title="Timezone">Timezone</a>: <i>String</i>
    <a href="#usedefaultprocessorfeatures" title="UseDefaultProcessorFeatures">UseDefaultProcessorFeatures</a>: <i>Boolean</i>
    <a href="#vpcsecuritygroups" title="VPCSecurityGroups">VPCSecurityGroups</a>: <i>
      - String</i>
</pre>

## Properties

#### AllocatedStorage

The amount of storage (in gigabytes) to be initially allocated for the database instance.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### AllowMajorVersionUpgrade

A value that indicates whether major version upgrades are allowed. Changing this parameter doesn't result in an outage and the change is asynchronously applied as soon as possible.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### AssociatedRoles

The AWS Identity and Access Management (IAM) roles associated with the DB instance.

_Required_: No

_Type_: List of <a href="dbinstancerole.md">DBInstanceRole</a>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### AutoMinorVersionUpgrade

A value that indicates whether minor engine upgrades are applied automatically to the DB instance during the maintenance window. By default, minor engine upgrades are applied automatically.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### AvailabilityZone

The Availability Zone (AZ) where the database will be created. For information on AWS Regions and Availability Zones.

_Required_: No

_Type_: String

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### BackupRetentionPeriod

The number of days for which automated backups are retained. Setting this parameter to a positive number enables backups. Setting this parameter to 0 disables automated backups.

_Required_: No

_Type_: Integer

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### CACertificateIdentifier

The identifier of the CA certificate for this DB instance.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### CharacterSetName

For supported engines, indicates that the DB instance should be associated with the specified character set.

_Required_: No

_Type_: String

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### CopyTagsToSnapshot

A value that indicates whether to copy tags from the DB instance to snapshots of the DB instance. By default, tags are not copied.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### DBClusterIdentifier

The identifier of the DB cluster that the instance will belong to.

_Required_: No

_Type_: String

_Pattern_: <code>^[a-zA-Z]{1}(?:-?[a-zA-Z0-9]){0,62}$</code>

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### DBInstanceClass

The compute and memory capacity of the DB instance, for example, db.m4.large. Not all DB instance classes are available in all AWS Regions, or for all database engines.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### DBInstanceIdentifier

A name for the DB instance. If you specify a name, AWS CloudFormation converts it to lowercase. If you don't specify a name, AWS CloudFormation generates a unique physical ID and uses that ID for the DB instance.

_Required_: No

_Type_: String

_Pattern_: <code>^[a-zA-Z]{1}(?:-?[a-zA-Z0-9]){0,62}$</code>

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### DBName

The meaning of this parameter differs according to the database engine you use.

_Required_: No

_Type_: String

_Pattern_: <code>^[_a-zA-Z][a-zA-Z0-9]{0,63}$</code>

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### DBParameterGroupName

The name of an existing DB parameter group or a reference to an AWS::RDS::DBParameterGroup resource created in the template.

_Required_: No

_Type_: String

_Pattern_: <code>^[a-zA-Z]{1}(?:-?[a-zA-Z0-9\.]){0,254}$</code>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### DBSecurityGroups

A list of the DB security groups to assign to the DB instance. The list can include both the name of existing DB security groups or references to AWS::RDS::DBSecurityGroup resources created in the template.

_Required_: No

_Type_: List of String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### DBSnapshotIdentifier

The name or Amazon Resource Name (ARN) of the DB snapshot that's used to restore the DB instance. If you're restoring from a shared manual DB snapshot, you must specify the ARN of the snapshot.

_Required_: No

_Type_: String

_Pattern_: <code>^[a-zA-Z]{1}(?:-?[a-zA-Z0-9]){0,254}$</code>

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### DBSubnetGroupName

A DB subnet group to associate with the DB instance. If you update this value, the new subnet group must be a subnet group in a new VPC.

_Required_: No

_Type_: String

_Pattern_: <code>^[a-zA-Z]{1}(?:-?[a-zA-Z0-9]){0,254}$</code>

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### DeleteAutomatedBackups

A value that indicates whether to remove automated backups immediately after the DB instance is deleted. This parameter isn't case-sensitive. The default is to remove automated backups immediately after the DB instance is deleted.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### DeletionProtection

A value that indicates whether the DB instance has deletion protection enabled. The database can't be deleted when deletion protection is enabled. By default, deletion protection is disabled.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Domain

The Active Directory directory ID to create the DB instance in. Currently, only MySQL, Microsoft SQL Server, Oracle, and PostgreSQL DB instances can be created in an Active Directory Domain.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### DomainIAMRoleName

Specify the name of the IAM role to be used when making API calls to the Directory Service.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### EnableCloudwatchLogsExports

The list of log types that need to be enabled for exporting to CloudWatch Logs. The values in the list depend on the DB engine being used.

_Required_: No

_Type_: List of String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### EnableIAMDatabaseAuthentication

A value that indicates whether to enable mapping of AWS Identity and Access Management (IAM) accounts to database accounts. By default, mapping is disabled.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### EnablePerformanceInsights

A value that indicates whether to enable Performance Insights for the DB instance.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Endpoint

_Required_: No

_Type_: <a href="endpoint.md">Endpoint</a>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Engine

The name of the database engine that you want to use for this DB instance.

_Required_: No

_Type_: String

_Allowed Values_: <code>aurora</code> | <code>aurora-mysql</code> | <code>aurora-postgresql</code> | <code>mariadb</code> | <code>mysql</code> | <code>oracle-ee</code> | <code>oracle-se2</code> | <code>oracle-se1</code> | <code>oracle-se</code> | <code>postgres</code> | <code>postgresql-license</code> | <code>sqlserver-ee</code> | <code>sqlserver-se</code> | <code>sqlserver-ex</code> | <code>sqlserver-web</code>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### EngineVersion

The version number of the database engine to use.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Iops

The number of I/O operations per second (IOPS) that the database provisions. The value must be equal to or greater than 1000.

_Required_: No

_Type_: Integer

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### KmsKeyId

The ARN of the AWS Key Management Service (AWS KMS) master key that's used to encrypt the DB instance.

_Required_: No

_Type_: String

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### LicenseModel

License model information for this DB instance.

_Required_: No

_Type_: String

_Allowed Values_: <code>bring-your-own-license</code> | <code>general-public-license</code> | <code>license-included</code> | <code>postgresql-license</code>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### MasterUsername

The master user name for the DB instance.

_Required_: No

_Type_: String

_Pattern_: <code>^[a-zA-Z][a-zA-Z0-9]{0,15}$</code>

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### MasterUserPassword

The password for the master user.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### MaxAllocatedStorage

The upper limit to which Amazon RDS can automatically scale the storage of the DB instance.

_Required_: No

_Type_: Integer

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### MonitoringInterval

The interval, in seconds, between points when Enhanced Monitoring metrics are collected for the DB instance. To disable collecting Enhanced Monitoring metrics, specify 0. The default is 0.

_Required_: No

_Type_: Integer

_Allowed Values_: <code>0</code> | <code>1</code> | <code>5</code> | <code>10</code> | <code>15</code> | <code>30</code> | <code>60</code>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### MonitoringRoleArn

The ARN for the IAM role that permits RDS to send enhanced monitoring metrics to Amazon CloudWatch Logs.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### MultiAZ

Specifies whether the database instance is a multiple Availability Zone deployment.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### OptionGroupName

Indicates that the DB instance should be associated with the specified option group.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### PerformanceInsightsKMSKeyId

The AWS KMS key identifier for encryption of Performance Insights data. The KMS key ID is the Amazon Resource Name (ARN), KMS key identifier, or the KMS key alias for the KMS encryption key.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### PerformanceInsightsRetentionPeriod

The amount of time, in days, to retain Performance Insights data. Valid values are 7 or 731 (2 years).

_Required_: No

_Type_: Integer

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Port

The port number on which the database accepts connections.

_Required_: No

_Type_: Integer

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### PreferredBackupWindow

The daily time range during which automated backups are created if automated backups are enabled, using the BackupRetentionPeriod parameter.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### PreferredMaintenanceWindow

he weekly time range during which system maintenance can occur, in Universal Coordinated Time (UTC).

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### ProcessorFeatures

The number of CPU cores and the number of threads per core for the DB instance class of the DB instance.

_Required_: No

_Type_: List of <a href="processorfeature.md">ProcessorFeature</a>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### PromotionTier

A value that specifies the order in which an Aurora Replica is promoted to the primary instance after a failure of the existing primary instance.

_Required_: No

_Type_: Integer

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### PubliclyAccessible

Indicates whether the DB instance is an internet-facing instance. If you specify true, AWS CloudFormation creates an instance with a publicly resolvable DNS name, which resolves to a public IP address. If you specify false, AWS CloudFormation creates an internal instance with a DNS name that resolves to a private IP address.

_Required_: No

_Type_: Boolean

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### SourceDBInstanceIdentifier

If you want to create a Read Replica DB instance, specify the ID of the source DB instance. Each DB instance can have a limited number of Read Replicas.

_Required_: No

_Type_: String

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### SourceRegion

The ID of the region that contains the source DB instance for the Read Replica.

_Required_: No

_Type_: String

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### StorageEncrypted

A value that indicates whether the DB instance is encrypted. By default, it isn't encrypted.

_Required_: No

_Type_: Boolean

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### StorageType

Specifies the storage type to be associated with the DB instance.

_Required_: No

_Type_: String

_Allowed Values_: <code>standard</code> | <code>gp2</code> | <code>io1</code>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Tags

Tags to assign to the DB instance.

_Required_: No

_Type_: List of <a href="tag.md">Tag</a>

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### TdeCredentialArn

The ARN from the key store with which to associate the instance for TDE encryption.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### TdeCredentialPassword

The password for the given ARN from the key store in order to access the device.

_Required_: No

_Type_: String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### Timezone

The time zone of the DB instance. The time zone parameter is currently supported only by Microsoft SQL Server.

_Required_: No

_Type_: String

_Update requires_: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

#### UseDefaultProcessorFeatures

A value that indicates whether the DB instance class of the DB instance uses its default processor features.

_Required_: No

_Type_: Boolean

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

#### VPCSecurityGroups

A list of the VPC security group IDs to assign to the DB instance. The list can include both the physical IDs of existing VPC security groups and references to AWS::EC2::SecurityGroup resources created in the template.

_Required_: No

_Type_: List of String

_Update requires_: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

## Return Values

### Ref

When you pass the logical ID of this resource to the intrinsic `Ref` function, Ref returns the DBInstanceIdentifier.

### Fn::GetAtt

The `Fn::GetAtt` intrinsic function returns a value for a specified attribute of this type. The following are the available attributes and sample return values.

For more information about using the `Fn::GetAtt` intrinsic function, see [Fn::GetAtt](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-getatt.html).

#### Address

Returns the <code>Address</code> value.

#### Port

Returns the <code>Port</code> value.

#### HostedZoneId

Returns the <code>HostedZoneId</code> value.