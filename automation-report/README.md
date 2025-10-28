# Usage

```yaml

jobs:
  run:
    ...
    steps:
      - name: Report State
        if: always()
        uses: mauhlik/actions/automation-report@main
        with:
          callback-url: ${{ inputs.resumeUrl }}

```