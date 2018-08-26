---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetImageAttribute:
    get:
      summary: Reset Image Attribute
      description: Resets an attribute of an AMI to its default value.
      operationId: resetimageattribute
      x-api-path-slug: actionresetimageattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ProductCode
        description: The product code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image
  /?Action=ResetInstanceAttribute:
    get:
      summary: Reset Instance Attribute
      description: Resets an attribute of an instance to its default value.
      operationId: resetinstanceattribute
      x-api-path-slug: actionresetinstanceattribute-get
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: BlockDeviceMapping.N
        description: The block device mapping
        type: string
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DisableApiTermination
        description: If you set this parameter to true, you cant terminate the instance            using
          the Amazon EC2 console, CLI, or API; otherwise, you can
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EbsOptimized
        description: Indicates whether the instance is optimized for EBS I/O
        type: string
      - in: query
        name: IamInstanceProfile
        description: The IAM instance profile
        type: string
      - in: query
        name: ImageId
        description: The ID of the AMI, which you can get by calling DescribeImages
        type: string
      - in: query
        name: InstanceInitiatedShutdownBehavior
        description: Indicates whether an instance stops or terminates when you initiate
          shutdown from the instance (using the operating system command for system
          shutdown)
        type: string
      - in: query
        name: InstanceType
        description: The instance type
        type: string
      - in: query
        name: Ipv6Address.N
        description: '[EC2-VPC] Specify one or more IPv6 addresses from the range
          of the subnet to            associate with the primary network interface'
        type: string
      - in: query
        name: Ipv6AddressCount
        description: '[EC2-VPC] A number of IPv6 addresses to associate with the primary
          network            interface'
        type: string
      - in: query
        name: KernelId
        description: The ID of the kernel
        type: string
      - in: query
        name: KeyName
        description: The name of the key pair
        type: string
      - in: query
        name: MaxCount
        description: The maximum number of instances to launch
        type: string
      - in: query
        name: MinCount
        description: The minimum number of instances to launch
        type: string
      - in: query
        name: Monitoring
        description: The monitoring for the instance
        type: string
      - in: query
        name: NetworkInterface.N
        description: One or more network interfaces
        type: string
      - in: query
        name: Placement
        description: The placement for the instance
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary IPv4 address'
        type: string
      - in: query
        name: RamdiskId
        description: The ID of the RAM disk
        type: string
      - in: query
        name: SecurityGroup.N
        description: '[EC2-Classic, default VPC] One or more security group names'
        type: string
      - in: query
        name: SecurityGroupId.N
        description: One or more security group IDs
        type: string
      - in: query
        name: SubnetId
        description: '[EC2-VPC] The ID of the subnet to launch the instance into'
        type: string
      - in: query
        name: UserData
        description: The user data to make available to the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=ResetNetworkInterfaceAttribute:
    get:
      summary: Reset Network Interface Attribute
      description: Resets a network interface attribute.
      operationId: resetnetworkinterfaceattribute
      x-api-path-slug: actionresetnetworkinterfaceattribute-get
      parameters:
      - in: query
        name: Ipv6Addresses.N
        description: The IPv6 addresses to unassign from the network interface
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
  /?Action=ResetSnapshotAttribute:
    get:
      summary: Reset Snapshot Attribute
      description: Resets permission settings for the specified snapshot.
      operationId: resetsnapshotattribute
      x-api-path-slug: actionresetsnapshotattribute-get
      parameters:
      - in: query
        name: Domain
        description: Set to vpc to allocate the address for use with instances in
          a VPC
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
---