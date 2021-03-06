# Change Log

## [Master](https://github.com/arangodb/go-driver/tree/HEAD)

**Closed issues:**

- Structs with key specified don't read the key [\#138](https://github.com/arangodb/go-driver/issues/138)
- Edge document with user provided key is inserted as many times as the number of shards [\#137](https://github.com/arangodb/go-driver/issues/137)
- Query "return null" make the panic: runtime error [\#117](https://github.com/arangodb/go-driver/issues/117)
- driver does not seem to decode numeric timestamps to time.Time [\#102](https://github.com/arangodb/go-driver/issues/102)
- stable and full feature? [\#100](https://github.com/arangodb/go-driver/issues/100)
- collection with "Wait for sync:" setting, Create-/UpdateDocument return: ArangoError: Code 0, ErrorNum 0 [\#96](https://github.com/arangodb/go-driver/issues/96)
- Error when connecting to ArangoDB with SSL enabled [\#95](https://github.com/arangodb/go-driver/issues/95)
- Possible concurrency issues, using VST connection [\#86](https://github.com/arangodb/go-driver/issues/86)
- An example of a transactional request [\#84](https://github.com/arangodb/go-driver/issues/84)
- Multi-tenancy connection management [\#83](https://github.com/arangodb/go-driver/issues/83)
- Cursor returned from a query with empty Count [\#82](https://github.com/arangodb/go-driver/issues/82)
- CONTRIBUTING.md [\#79](https://github.com/arangodb/go-driver/issues/79)
- Querying documents + [\#76](https://github.com/arangodb/go-driver/issues/76)
- Is there an ArangoDB-Object on Struct? [\#75](https://github.com/arangodb/go-driver/issues/75)
- DB Session [\#73](https://github.com/arangodb/go-driver/issues/73)
- correct way to get multiple documents ? [\#70](https://github.com/arangodb/go-driver/issues/70)
- Revalidate whether workaround can be removed [\#68](https://github.com/arangodb/go-driver/issues/68)
- Makefile `SWTSECRET` vs `JWTSECRET` [\#66](https://github.com/arangodb/go-driver/issues/66)
- Implement transactions [\#56](https://github.com/arangodb/go-driver/issues/56)
- bulk import API [\#55](https://github.com/arangodb/go-driver/issues/55)
- Question: how to write auto-inc feild? [\#51](https://github.com/arangodb/go-driver/issues/51)
- add index attribute for new feature in arangodb3.2 [\#48](https://github.com/arangodb/go-driver/issues/48)
- Unable to connect to server in macos [\#41](https://github.com/arangodb/go-driver/issues/41)
- Handle 401 status code before checking content type. [\#38](https://github.com/arangodb/go-driver/issues/38)
- Support for raw string in query return [\#37](https://github.com/arangodb/go-driver/issues/37)
- \[ArangoDB Server 3.1.6\] Unsupported content type: client.DatabaseExists when Database already exists [\#36](https://github.com/arangodb/go-driver/issues/36)
- Can't connect because of 'Unsupported content type'? [\#35](https://github.com/arangodb/go-driver/issues/35)
- cursor implementation when running queries with non-Document return values [\#20](https://github.com/arangodb/go-driver/issues/20)
- Make failover with cursors more explicit [\#16](https://github.com/arangodb/go-driver/issues/16)
- Add non-context version of method calls [\#7](https://github.com/arangodb/go-driver/issues/7)

**Merged pull requests:**

- Properly closing idle VST connections [\#139](https://github.com/arangodb/go-driver/pull/139)
- Improving performance of reading the body of large responses [\#134](https://github.com/arangodb/go-driver/pull/134)
- Added Collection.ReadDocuments [\#133](https://github.com/arangodb/go-driver/pull/133)
- Added support for fetching job ID in CleanoutServer [\#131](https://github.com/arangodb/go-driver/pull/131)
- Exclude high load test on VST+3.2 [\#129](https://github.com/arangodb/go-driver/pull/129)
- Test/prevent concurrent vst read write [\#128](https://github.com/arangodb/go-driver/pull/128)
- Added single+ssl tests. All tests now use starter [\#127](https://github.com/arangodb/go-driver/pull/127)
- Bugfix/read chunk loop [\#126](https://github.com/arangodb/go-driver/pull/126)
- Prevent possible endless read chunk look in in VST connection [\#125](https://github.com/arangodb/go-driver/pull/125)
- Fixing Query\(return nul\) resulting in panic [\#124](https://github.com/arangodb/go-driver/pull/124)
- Added WithAllowNoLeader [\#123](https://github.com/arangodb/go-driver/pull/123)
- Added Cluster.RemoveServer [\#122](https://github.com/arangodb/go-driver/pull/122)
- Added mutex guarding message chunks. [\#121](https://github.com/arangodb/go-driver/pull/121)
- Documentation/go refactor [\#120](https://github.com/arangodb/go-driver/pull/120)
- VST stream cursor test fixes & VST fail-quick fix [\#119](https://github.com/arangodb/go-driver/pull/119)
- Prevent a VST connection from being used before its configuration callback has finished [\#118](https://github.com/arangodb/go-driver/pull/118)
- Fixed AgencyConnection in the context of authentication [\#116](https://github.com/arangodb/go-driver/pull/116)
- Adding timeout for streaming cursor test [\#115](https://github.com/arangodb/go-driver/pull/115)
- Added package level docs [\#114](https://github.com/arangodb/go-driver/pull/114)
- Close the connection when the initial onCreatedCallback fails [\#113](https://github.com/arangodb/go-driver/pull/113)
- Adding extra concurrency-safety for VST [\#112](https://github.com/arangodb/go-driver/pull/112)
- Added upper limit to the number of concurrent requests to a single server. [\#111](https://github.com/arangodb/go-driver/pull/111)
- Added support for multiple VST connections per server [\#110](https://github.com/arangodb/go-driver/pull/110)
- Fixed expected status code for operations on collections that have waitForSync enabled [\#109](https://github.com/arangodb/go-driver/pull/109)
- Added helper to determine agency health [\#108](https://github.com/arangodb/go-driver/pull/108)
- Added ServerID function [\#107](https://github.com/arangodb/go-driver/pull/107)
- Added exclusive lock using agency [\#106](https://github.com/arangodb/go-driver/pull/106)
- Added helper for JWT secret based authentication [\#105](https://github.com/arangodb/go-driver/pull/105)
- Added Agency API [\#104](https://github.com/arangodb/go-driver/pull/104)
- Added option to not follow redirects and return the original response [\#103](https://github.com/arangodb/go-driver/pull/103)
- Add support for stream query cursor [\#101](https://github.com/arangodb/go-driver/pull/101)
- Active-Failover with Velocystream [\#99](https://github.com/arangodb/go-driver/pull/99)
- Added API functions for shutting down a server and cleaning it out [\#98](https://github.com/arangodb/go-driver/pull/98)
- Skip replication test on cluster [\#94](https://github.com/arangodb/go-driver/pull/94)
- Documented behavior for custom http.Transport wrt MaxIdleConnsPerHost field [\#93](https://github.com/arangodb/go-driver/pull/93)
- Fix ReturnOld/New for edge/vertex operations. [\#92](https://github.com/arangodb/go-driver/pull/92)
- Database.Info\(\) added [\#91](https://github.com/arangodb/go-driver/pull/91)
- Replication interface added. [\#90](https://github.com/arangodb/go-driver/pull/90)
- Grouping server specific info calls in ClientServerInfo, exposing ServerRole API [\#89](https://github.com/arangodb/go-driver/pull/89)
- Added `ReplicationFactor` to `SetCollectionPropertiesOptions` [\#88](https://github.com/arangodb/go-driver/pull/88)
- Allow for some time to reach intended status [\#87](https://github.com/arangodb/go-driver/pull/87)
- Fixing SWTSECRET -\> JWTSECRET [\#85](https://github.com/arangodb/go-driver/pull/85)
- Added CONTRIBUTING.md [\#80](https://github.com/arangodb/go-driver/pull/80)
- Resilientsingle support [\#77](https://github.com/arangodb/go-driver/pull/77)
- Adding cluster specific operations [\#72](https://github.com/arangodb/go-driver/pull/72)
- Added IsSmart, SmartGraphAttribute attributes to CreateCollectionOptions [\#71](https://github.com/arangodb/go-driver/pull/71)
- Adding Response.Header\(string\) & tests [\#69](https://github.com/arangodb/go-driver/pull/69)
- Server mode \(get/set\) [\#65](https://github.com/arangodb/go-driver/pull/65)
- Adding `WithConfigured` [\#64](https://github.com/arangodb/go-driver/pull/64)
- Added DistributeShardsLike field to CreateCollectionOptions [\#62](https://github.com/arangodb/go-driver/pull/62)
- Added WithEnforceReplicationFactor [\#61](https://github.com/arangodb/go-driver/pull/61)
- Added `WithIsSystem` [\#60](https://github.com/arangodb/go-driver/pull/60)
- Support synchronising endpoints on resilient single server mode [\#59](https://github.com/arangodb/go-driver/pull/59)
- Added `WithIgnoreRevisions` [\#58](https://github.com/arangodb/go-driver/pull/58)
- Basic transaction implementation [\#57](https://github.com/arangodb/go-driver/pull/57)
- Support `x-arango-dump` content type [\#54](https://github.com/arangodb/go-driver/pull/54)
- Added WithIsRestore \(not internal for normal client use!!!!\) [\#53](https://github.com/arangodb/go-driver/pull/53)
- Raw authentication [\#52](https://github.com/arangodb/go-driver/pull/52)
- Include travis tests for arangodb 3.1 [\#50](https://github.com/arangodb/go-driver/pull/50)
- Added NoDeduplicate field for hash & skiplist index options [\#49](https://github.com/arangodb/go-driver/pull/49)
- Supporting additional user access functions [\#47](https://github.com/arangodb/go-driver/pull/47)
- ftKnox - fix sprintf conversions [\#42](https://github.com/arangodb/go-driver/pull/42)
- Convert 401 text/plain response to proper ArangoError [\#39](https://github.com/arangodb/go-driver/pull/39)
- Adding Storage engine detection [\#34](https://github.com/arangodb/go-driver/pull/34)
- Starter update [\#33](https://github.com/arangodb/go-driver/pull/33)
- Fix reading the response body to ensure keep-alive [\#32](https://github.com/arangodb/go-driver/pull/32)
- Velocy stream support \(wip\) [\#31](https://github.com/arangodb/go-driver/pull/31)
- Supporting Velocypack content-type \(instead of JSON\) \(wip\) [\#29](https://github.com/arangodb/go-driver/pull/29)
- Fixed Cursor.ReadDocument for queries returning non-documents [\#27](https://github.com/arangodb/go-driver/pull/27)
- Added Collection.Statistics [\#25](https://github.com/arangodb/go-driver/pull/25)
- Adding Database.ValidateQuery [\#24](https://github.com/arangodb/go-driver/pull/24)
- Added Collection.DocumentExists [\#23](https://github.com/arangodb/go-driver/pull/23)
- Added `Database.Remove\(\)` [\#22](https://github.com/arangodb/go-driver/pull/22)
- Changing graph API to introduce VertexConstraints [\#21](https://github.com/arangodb/go-driver/pull/21)
- Endpoint reconfiguration [\#19](https://github.com/arangodb/go-driver/pull/19)
- Allow custom http.RoundTripper [\#18](https://github.com/arangodb/go-driver/pull/18)
- Added WithEndpoint, used to force a specific endpoint for a request.  [\#17](https://github.com/arangodb/go-driver/pull/17)
- Adding failover tests [\#15](https://github.com/arangodb/go-driver/pull/15)
- Adding simple performance benchmarks [\#14](https://github.com/arangodb/go-driver/pull/14)
- Cluster tests [\#12](https://github.com/arangodb/go-driver/pull/12)
- ImportDocuments [\#11](https://github.com/arangodb/go-driver/pull/11)
- Adding Graph support \(wip\) [\#10](https://github.com/arangodb/go-driver/pull/10)
- Added collection status,count,rename,load,unload,truncate,properties [\#9](https://github.com/arangodb/go-driver/pull/9)
- Adding user API [\#8](https://github.com/arangodb/go-driver/pull/8)
- Adding index support [\#6](https://github.com/arangodb/go-driver/pull/6)
- Added Cursor support [\#5](https://github.com/arangodb/go-driver/pull/5)
- Adding multi document requests [\#4](https://github.com/arangodb/go-driver/pull/4)
- Creating interface. \(WIP\) [\#3](https://github.com/arangodb/go-driver/pull/3)
- Revert "Creating interface" [\#2](https://github.com/arangodb/go-driver/pull/2)
- Creating interface [\#1](https://github.com/arangodb/go-driver/pull/1)



\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*