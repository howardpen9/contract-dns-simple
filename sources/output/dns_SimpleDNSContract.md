# TACT Compilation Report
Contract: SimpleDNSContract
BOC Size: 2523 bytes

# Types
Total Types: 14

## StateInit
TLB: `_ code:^cell data:^cell = StateInit`
Signature: `StateInit{code:^cell,data:^cell}`

## Context
TLB: `_ bounced:bool sender:address value:int257 raw:^slice = Context`
Signature: `Context{bounced:bool,sender:address,value:int257,raw:^slice}`

## SendParameters
TLB: `_ bounce:bool to:address value:int257 mode:int257 body:Maybe ^cell code:Maybe ^cell data:Maybe ^cell = SendParameters`
Signature: `SendParameters{bounce:bool,to:address,value:int257,mode:int257,body:Maybe ^cell,code:Maybe ^cell,data:Maybe ^cell}`

## Deploy
TLB: `deploy#946a98b6 queryId:uint64 = Deploy`
Signature: `Deploy{queryId:uint64}`

## DeployOk
TLB: `deploy_ok#aff90f57 queryId:uint64 = DeployOk`
Signature: `DeployOk{queryId:uint64}`

## ChangeOwner
TLB: `change_owner#0f474d03 newOwner:address = ChangeOwner`
Signature: `ChangeOwner{newOwner:address}`

## DNSResolveResult
TLB: `_ prefix:int257 record:Maybe ^cell = DNSResolveResult`
Signature: `DNSResolveResult{prefix:int257,record:Maybe ^cell}`

## UpdateRecord
TLB: `update_record#d294b726 domain:^string category:int257 record:Maybe ^cell = UpdateRecord`
Signature: `UpdateRecord{domain:^string,category:int257,record:Maybe ^cell}`

## EventPermissionsUpdated
TLB: `event_permissions_updated#6cd59be6 permissions:Permissions{canAdd:bool,canRemove:bool,canReplace:bool} = EventPermissionsUpdated`
Signature: `EventPermissionsUpdated{permissions:Permissions{canAdd:bool,canRemove:bool,canReplace:bool}}`

## EventRecordAdded
TLB: `event_record_added#a61ddcfd domain:^string category:int257 record:^cell = EventRecordAdded`
Signature: `EventRecordAdded{domain:^string,category:int257,record:^cell}`

## EventRecordUpdated
TLB: `event_record_updated#ef2db883 domain:^string category:int257 oldRecord:^cell newRecord:^cell = EventRecordUpdated`
Signature: `EventRecordUpdated{domain:^string,category:int257,oldRecord:^cell,newRecord:^cell}`

## EventRecordRemoved
TLB: `event_record_removed#ff9494f1 domain:^string category:int257 = EventRecordRemoved`
Signature: `EventRecordRemoved{domain:^string,category:int257}`

## DNSRecord
TLB: `_ name:^string categories:dict<int, ^cell> = DNSRecord`
Signature: `DNSRecord{name:^string,categories:dict<int, ^cell>}`

## Permissions
TLB: `_ canAdd:bool canRemove:bool canReplace:bool = Permissions`
Signature: `Permissions{canAdd:bool,canRemove:bool,canReplace:bool}`

# Get Methods
Total Get Methods: 4

## records

## permissions

## owner

## dnsresolve
Argument: subdomain
Argument: category

# Error Codes
2: Stack undeflow
3: Stack overflow
4: Integer overflow
5: Integer out of expected range
6: Invalid opcode
7: Type check error
8: Cell overflow
9: Cell underflow
10: Dictionary error
13: Out of gas error
32: Method ID not found
34: Action is invalid or not supported
37: Not enough TON
38: Not enough extra-currencies
128: Null reference exception
129: Invalid serialization prefix
130: Invalid incoming message
131: Constraints error
132: Access denied
133: Contract stopped
134: Invalid argument
135: Code of a contract was not found
136: Invalid address
137: Masterchain support is not enabled for this contract
21519: Can't remove records
22696: Invalid domain
24161: Invalid DNS name
26438: Fuse already burned
43961: Can't add records
55590: Can't replace records