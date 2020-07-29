# Release 3.0.1
- fixed [nuget package](https://www.nuget.org/packages/linq2db.LINQPad) fo LINQPad 6

# Release 3.0.0

- [linqpad] added support for LINQPad 6 including new [nuget package](https://www.nuget.org/packages/linq2db.LINQPad)  ([#29](https://github.com/linq2db/linq2db.LINQPad/issues/29))
- [tools] driver updated to use recent linq2db 3.0.1 release
- [tools] switched to [Humanizer.Core](https://www.nuget.org/packages/Humanizer.Core) for model pluralization
- [providers] removed ODP.NET Native Oracle provider (we still support the managed provider, which doesn't require client installation)
- [providers] added support for MS Access ODBC provider
- [providers] replaced MySql.Data provider with [MySqlConnector](https://www.nuget.org/packages/MySqlConnector) provider
- [providers] replaced native SAP/Sybase ASE provider with managed [AdoNetCore.AseClient](https://www.nuget.org/packages/AdoNetCore.AseClient) provider
- [providers] removed IBM DB2 iSeries support temporarily because required [provider](https://github.com/LinqToDB4iSeries/Linq2DB4iSeries) lacks linq2db v3 support
- [providers] added SAP HANA ODBC provider
- [providers] IBM Informix provider switched to use [IBM.Data.DB](https://www.nuget.org/packages/IBM.Data.DB2.Core/) IDS provider (SQLI provider could be added on request)
- [providers] there is no need to pre-install client for IBM Informix anymore
- [providers] there is no need to pre-install client for IBM DB LUW/zOS anymore
- [providers] there is no need to pre-install client for SAP/Sybase ASE anymore ([#33](https://github.com/linq2db/linq2db.LINQPad/issues/33))
- [providers] fixed multiple issues with provider-specific types support
- [providers] added support for array and dictionary types (e.g. PostgreSQL array and hstore types)
- [ui] fixed database tree to not create duplicate/unnecessary schema nodes
- [ui] fixed connection dialog aligment issues
- [ui] tables without columns not shown anymore (e.g. Access system tables without read permissions)
- [ui] added provider path setting for SqlCe and SAP HANA Native providers for LINQPad 6 version
- [ui] fixed non-xml characters rendering in custom formatter
- [ui] always use custom formatters for provider-specific types
- [misc] added license file (MIT) to repository
- [misc] copyrights updated to include major contributors
- [misc] migrated to Azure Pipelines from Appveyor for builds
- [misc] codebase updated to C# 8.0 with nullable reference types