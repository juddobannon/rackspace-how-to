---
permalink: permissions-matrix-for-cloud-block-storage/
audit_date:
title: Permissions matrix for Cloud Block Storage
type: article
created_date: '2013-04-10'
created_by: Renee Rendon
last_modified_date: '2016-06-06'
last_modified_by: Nate Archer
product: Cloud Block Storage
product_url: cloud-block-storage
---

The following permissions matrix displays specific permissions for the roles in Cloud Block Storage. The matrix displays the method names, their corresponding RESTful API commands, and the roles that are supported.

#### As of February 7, 2013

Method | API Action | Role | Description
:---: | :---: | :---: | :---:
**VOLUMES** |
Create Volume | <code>POST /volumes</code> | **Creator, Admin** | Creates the volume.
List Volumes | <code>GET /volumes</code> | **Observer, Creator, Admin** | Lists summary information for all block storage volumes that the tenant who submits the request can access.
List Volumes (Detailed) | <code>GET /volumes/detail</code> | **Observer, Creator & Admin** | Lists detailed information for all Block Storage volumes that the tenant who submits the request can access.
Show Volume | <code>GET /volumes/{volume_id}</code> | **Observer, Creator, Admin** | View all information about a single volume.
Rename Volume | <code>PUT /volumes/{volume_id}</code> | **Observer, Creator, Admin** | Updates a volume's display name and display description.
Delete Volume | <code>DELETE /volumes/{volume_id}</code> | **Admin only** | Deletes a single volume.
**VOLUME TYPES** |
List Volume Types | <code>GET /types</code> | **Observer, Creator, Admin** | Requests a list of volume types.
Describe Volume Type | <code>GET /types/{volume_type_id}</code> | **Creator, Admin** | Requests a single volume type.
**SNAPSHOTS** |
Create Snapshot</td> | <code>POST /snapshots</code> | **Creator, Admin** | Creates a snapshot.
List Snapshots | <code>GET /snapshots</code> | **Observer, Creator, Admin** | Lists summary information for all Block Storage snapshots that the tenant who submits the request can access.
List Snapshots (Detailed) | <code>GET /snapshots/detail</code> | **Observer, Creator, Admin** | Lists detailed information for all Block Storage snapshots that the tenant who submits the request can access.
Show Snapshot | <code>GET /snapshots/{snapshot_id}</code> | **Observer, Creator, Admin** | View all information about a single snapshot.
Delete Snapshot | <code>DELETE /snapshots/{snapshot_id}</code> | **Admin only** | Deletes a single snapshot.

[**Permissions matrix for Role-Based Access Control**](/how-to/permissions-matrix-for-role-based-access-control-rbac)
