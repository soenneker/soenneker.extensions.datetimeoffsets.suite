[![](https://img.shields.io/nuget/v/soenneker.extensions.datetimeoffsets.suite.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.extensions.datetimeoffsets.suite/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.extensions.datetimeoffsets.suite/publish-package.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.extensions.datetimeoffsets.suite/actions/workflows/publish-package.yml)
[![](https://img.shields.io/nuget/dt/soenneker.extensions.datetimeoffsets.suite.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.extensions.datetimeoffsets.suite/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.extensions.datetimeoffsets.suite/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.extensions.datetimeoffsets.suite/actions/workflows/codeql.yml)

# ![](https://user-images.githubusercontent.com/4441470/224455560-91ed3ee7-f510-4041-a8d2-3fc093025112.png) Soenneker.Extensions.DateTimeOffsets.Suite

One package reference for the Soenneker `DateTimeOffset` calendar-boundary extensions.

## Installation

```bash
dotnet add package Soenneker.Extensions.DateTimeOffsets.Suite
```

## Included packages

- `Soenneker.Extensions.DateTimeOffsets.DayOfWeeks`
- `Soenneker.Extensions.DateTimeOffsets.Hours`
- `Soenneker.Extensions.DateTimeOffsets.Months`
- `Soenneker.Extensions.DateTimeOffsets.Quarters`
- `Soenneker.Extensions.DateTimeOffsets.Weeks`
- `Soenneker.Extensions.DateTimeOffsets.Years`

This is a meta-package: it adds the packages above and does not define extension methods of its own. Install it when an application uses several boundary groups; install an individual package when only one group is needed.

Each included package supplies its own namespace and usage documentation. Depending on the operation, methods either preserve the input's existing offset or calculate a local calendar boundary in a supplied `TimeZoneInfo` and return the corresponding UTC instant.
