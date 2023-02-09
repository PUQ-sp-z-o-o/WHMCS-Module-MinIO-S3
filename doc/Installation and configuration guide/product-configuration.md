# Product Configuration

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-minio-s3) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-MinIO-S3/) | [Forum](https://forum.puqcloud.com/viewforum.php?f=3)

##### Add new product to WHMCS

```
System Settings->Products/Services->Create a New Product
```

In the **Module settings** section, select the **"PUQ MinIOS3"** module

[![image-1660047236549.png](https://doc.puq.info/uploads/images/gallery/2022-08/scaled-1680-/image-1660047236549.png)](https://doc.puq.info/uploads/images/gallery/2022-08/image-1660047236549.png)

- **License key:** A pre-purchased license key for the **"PUQ MinIOS3"** module. For the module to work correctly, the key must be active
- **Unit:** Packet disk space units
- **Disk space size:** Disk size in this product
- **Notification disk limit email template:** Email template that will be sent when the disk quota is exceeded in %
- **Notification, used disk space X %:** Sets a percentage parameter, after exceeding this parameter a notification will be sent to the user
- **Username prefix/Username suffix:** Necessary in order to generate a username for the service, in the format: **prefix&lt;cliet\_id&gt;-&lt;service\_id&gt;suffix**
- **Group:** The group that will be assigned to the user on the server side of the **MinIO S3**
- **Raw Policy:** The policy that is assigned to the user during creation on the server

<p class="callout info"> Example:</p>

<p class="callout warning">**In the given policy example. The user has the right to create buckets with a name starting with the username.**</p>

```JSON
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                "admin:Heal",
                "admin:SetBucketTarget",
                "admin:TopLocksInfo",
                "admin:DataUsageInfo",
                "admin:GetBucketQuota",
                "admin:GetBucketTarget"
            ],
            "Resource": [
                "arn:aws:s3:::<USER_ID>*"
            ]
        },
        {
            "Effect": "Allow",
            "Action": [
                "s3:*"
            ],
            "Resource": [
                "arn:aws:s3:::<USER_ID>*"
            ]
        }
    ]
}
```

- **Suspend exceeding disk limit email template:** The template of the letter that will be sent to the client if his disk limit is 100% or less 100%
- **Save usage history (days):** The number of days it takes to save user disk usage statistics
- **Link to instruction:** Link to the instruction, if filled out, it will be reflected in the client area