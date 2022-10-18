---
version: 1.0
submitted_by: greenhsu123
published_date: tbd
category: cloud
tags: 
 - storage
 - role:cloud-engineer
 - size:small
---

# Set Storage Retention Policies

## Description
From an embodied carbon perspective, it's better to have an automated mechanism to delete unused storage resources so we are efficient with hardware and that the storage layer is optimised for the task. 

## Solution
Set a retention policy on storage resources to automate the deletion of unused storage resources. 

## SCI Impact

`SCI = (E * I) + M per R`
[Software Carbon Intensity Spec](https://grnsft.org/sci)

Concerning the SCI equation. Setting retention policy will impact one part:

- `M`: By reducing the total number of storage volumes required, we reduce the total embodied carbon.

## Assumptions
If we choose not to delete *ALL* storage resources because they might be needed in the future, then storing them permanently will take up a lot of unnecessary storage resources. A better solution would be to set a retention policy that automatically deletes and keeps storage resources based on business needs. 

## Considerations
- It may reduce cloud bills, as reducing idle storage resources will cost less. 
- If a retention policy on the storage resources is undefined, there is more overhead for manually deleting idle resources. 

## References
- [Hardware Efficiency Principle](https://learn.greensoftware.foundation/practitioner/hardware-efficiency)