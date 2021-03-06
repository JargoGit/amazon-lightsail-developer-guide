# Create a snapshot of your Linux/Unix\-based instance in Lightsail<a name="lightsail-how-to-create-a-snapshot-of-your-instance"></a>

*Last updated: June 28, 2018*

You can create snapshots of your Linux/Unix\-based Lightsail instances\. An *instance snapshot* is a copy of the system disk and matches the original machine configuration \(memory, CPU, disk size, and data transfer rate\)\. If you've attached block storage disks to your instance, Lightsail copies those additional disks as part of your snapshot\. For more information, see [Instance snapshots in Amazon Lightsail](understanding-instance-snapshots-in-amazon-lightsail.md)\.

**Note**  
The steps to create a snapshot of a Windows Server\-based Lightsail instance are different\. For more information, see [Creating a snapshot of your Windows Server instance in Amazon Lightsail](prepare-windows-based-instance-and-create-snapshot.md)\.

You must already have an instance in Lightsail to create a snapshot of it\. After you have an instance, follow these steps to create a snapshot:

1. On the Lightsail home page, choose your instance\. Or choose **Manage** on the shortcut menu\.  
![\[Manage instance menu\]](https://d9yljz1nd5001.cloudfront.net/en_us/b380b072d417d05346bbc87239d4fd76/images/linux-instance-manage-instance-from-shortcut-menu-home-page.gif)

1. Choose **Snapshots**\.

1. If needed, change the name of your snapshot, and then choose **Create snapshot**\.

   You can see the snapshot you just created in the **Recent snapshots** section\. It will show up as **In progress\.\.\.**\.

   Once the snapshot is finished, you can [create another instance based on this snapshot](lightsail-how-to-create-instance-from-snapshot.md)\. For example, you may want to create a larger size bundle than you had previously\.

**Important**  
When you create a new instance from a snapshot, Lightsail lets you create an instance bundle that is either the same size or larger size\. We do not currently support creating a *smaller* instance size from a snapshot\. The smaller options will be grayed out when you create a new instance from a snapshot\.

To create a larger instance size from a snapshot, you can use the Lightsail console, the **create\-instances\-from\-snapshot** CLI command\. or the **CreateInstancesFromSnapshot** API operation\. [Learn how to create an instance from a snapshot](lightsail-how-to-create-instance-from-snapshot.md)\.

For more information about Lightsail bundles, see [Lightsail Pricing](https://amazonlightsail.com/pricing/)\.