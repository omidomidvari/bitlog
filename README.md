# bitlog

[![GitHub Action](https://shields.io)](https://github.com)
[![License: GNU](https://shields.io)](https://opensource.org)

**bitlog** is a lightweight GitHub Action for logging data from a js file.

## 🚀 Features

*   **Native Integration:** Works seamlessly within any GitHub Actions workflow.
*   **Lightweight:** Minimal overhead for fast execution.
*   **Configurable:** Supports custom inputs defined in `action.yml`.


```yaml
jobs:
  log_data:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v4

      - name: Run bitlog
        uses: omidomidvari/bitlog@main
        with:
          # Replace these with actual inputs from your action.yml
          input_name: "value" 
