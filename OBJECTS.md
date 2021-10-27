# EPP Objects

## Domains

| Name | Type | Description | `<check>` | `<info>` | `<transfer op="query">` | `<create>` | `<delete>` | `<renew>` | `<transfer>` | `<update>` |
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| `name` | Simple | Name | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ 1<br>✅ 1 | ✅ 1<br>✅ 1 | ✅ |
| `reason` | Simple | Reason | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| `authInfo` | Complex | Auth Info | ❌ | ✅ | ✅ | ✅ | ❌ | ❌ | ✅ 0-1<br>❌ |
| `roid` | Simple | Repository ID | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `status` | Simple+ | Status | ❌ | ✅ | ❌ | ❌ | ❌ | | | ✅ | ❌ |
| `registrant` | Simple | Registrant | ❌ | ✅ | ❌ | ✅ | ❌ | ❌ |
| `contact` | Simple | Contact | ❌ | ✅ | ❌ | ✅ | ❌ | ❌ |
| `ns` | Complex | Name Servers | ❌ | ✅ | ❌ | ✅ | ❌ | ❌ |
| `host` | Simple | Host | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `clID` | Simple | Client ID | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `crID` | Simple | Create ID | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `crDate` | Simple | Create Date | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `exDate` | Simple | Expire Date | ❌ | ✅ | ✅ | ❌ | ❌ | ❌<br>✅ 0-1 |
| `upID` | Simple | Update ID | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `upDate` | Simple | Update Date | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `trDate` | Simple | Transaction Date | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| `period` | Simple | Period | ❌ | ❌ | ✅ | ✅ | ❌ | ✅ 0-1<br>❌ | ✅ 0-1/
| `trStatus` | Simple | Transaction Status | ❌ | ❌ | ✅ | ❌ | ❌ | ❌ |
| `reID` | Simple | Request ID | ❌ | ❌ | ✅ | ❌ | ❌ | ❌ |
| `reDate` | Simple | Request Date | ❌ | ❌ | ✅ | ❌ | ❌ | ❌ |
| `acID` | Simple | Act ID | ❌ | ❌ | ✅ | ❌ | ❌ | ❌ |
| `acDate` | Simple | Act Date | ❌ | ❌ | ✅ | ❌ | ❌ | ❌ |
| `curExpDate` | Simple | Current Expiry Date | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ 1<br>❌ |
