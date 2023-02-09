# Email Template (puqMinIOS3 service Suspension Notification disk limit)

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-minio-s3) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/) | [Forum](https://forum.puqcloud.com/viewforum.php?f=3)

##### Create an email template for customer notifications.

```
System Settings->Email Templates->Create New Email Template
```

- **Email Type:** Product/service
- **Unique Name:** puqMinIOS3 service Suspension Notification disk limit

[![image-1660046825751.png](https://doc.puq.info/uploads/images/gallery/2022-08/scaled-1680-/image-1660046825751.png)](https://doc.puq.info/uploads/images/gallery/2022-08/image-1660046825751.png)

**Subject:**

```PHP
Suspension Information - {$username}
```

**Body:**

```PHP
Dear {$client_name},

This email informs you that the S3 account has been disabled due to running out of free space.

It is also possible to upgrade to a package with more space.

Product/Service: {$service_product_name}
Due Date: {$service_next_due_date}

Username: {$username}

Disk limit: {$disk_limit_bytes*$unit_coefficient} {$unit}
Disk used: {$disk_used_unit} {$unit} ({$disk_used_percentage} %)
Disk free: {$disk_free_unit} {$unit} ({$disk_free_percentage} %)

{$signature}
```

[![image-1660046885278.png](https://doc.puq.info/uploads/images/gallery/2022-08/scaled-1680-/image-1660046885278.png)](https://doc.puq.info/uploads/images/gallery/2022-08/image-1660046885278.png)