# EPP Objects

## Domains

| Name | Type | Description | `<check>` | `<info>` | `<transfer op="query">` | `<create>` | `<delete>` | `<renew>` | `<transfer>` | `<update>` |
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| `name` | Simple | Name | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| `reason` | Simple | Reason | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| `authInfo` | Complex | Auth Info | ❌ | ✅ |
| `roid` | Simple | Repository ID | ❌ | ✅ | | | | | | |
| `status` | Simple+ | Status | ❌ | ✅ | | | | | | ✅ |
| `registrant` | Simple | Registrant | ❌ |
| `contact` | Simple | Contact | ❌ |
| `ns` | Complex | Name Servers | ❌
| `host` | Simple | Host | ❌ | ✅ |
| `clID` | Simple | Client ID | ❌ | ✅ |
| `crID` | Simple | Create ID | ❌ | ✅ |
| `crDate` | Simple | Create Date | ❌ | ✅ |
| `exDate` | Simple | Expire Date | ❌ |
| `upID` | Simple | Update ID | ❌ |
| `upDate` | Simple | Update Date | ❌ |
| `trDate` | Simple | Transaction Date | ❌ |
