# Usage

```yaml

jobs:
  run:
    permissions:
      id-token: write
    ...
    steps:
      - name: Report State
        if: always()
        uses: mauhlik/actions/automation-report@main
        with:
          callback-url: ${{ inputs.resumeUrl }}

```