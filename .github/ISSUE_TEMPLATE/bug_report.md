name: Bug Report
description: Report a bug
title: "[Bug]: "
labels: "Bug"
body:
  - type: textarea
    attributes:
      label: Describe the bug
      description: A clear and concise description of what the bug is.
    validations:
      required: true
  - type: textarea
    attributes:
      label: Expected Behavior
      description: A clear and concise description of what you expected to happen.
    validations:
      required: true
  - type: textarea
    attributes:
      label: Actual Behavior
      description: A clear description of what actually happens.
    validations:
      required: true
  - type: textarea
    attributes:
      label: Screenshots
      description: If applicable, add screenshots to help explain your problem.
    validations:
      required: false
  - type: input
    attributes:
      label: Medusa Version
      description: What version of Medusa are you using?
      placeholder: c65ca2
    validations:
      required: true
  - type: dropdown
    attributes:
      label: What branch are you on?
      options:
        - master
        - develop
        - Other (specify below)
    validations:
      required: true
  - type: dropdown
    attributes:
      label: What operating system are you using?
      options:
        - Windows
        - macOS
        - Ubuntu
        - Other Linux
        - Other (specify below)
    validations:
      required: true
  - type: input
    attributes:
      label: Operating System Version
      description: What operating system version are you using? On Windows, click Start button > Settings > System > About. On macOS, click the Apple Menu > About This Mac. On Linux, use lsb_release or uname -a.
      placeholder: "e.g. Windows 10 version 1909, macOS Catalina 10.15.7, or Ubuntu 20.04"
    validations:
      required: true
  - type: dropdown
    attributes:
      label: What Python version are you using?
      options:
        - 2.7.1
        - 3.6.8
        - Other (specify below)
    validations:
      required: true
  - type: textarea
    attributes:
      label: Debug logs (at least 50 lines)
      description: General > Advanced Settings > Enable debug
    validations:
      required: false
  - type: input
    attributes:
      label: Testcase Gist URL
      description: If you can reproduce the issue in a standalone test case, please create one and to publish it as a [GitHub gist](https://gist.github.com) and put the gist URL here. This is **the best way** to ensure this issue is triaged quickly.
      placeholder: https://gist.github.com/...
  - type: textarea
    attributes:
      label: Additional Information
      description: If your problem needs further explanation, or if the issue you're seeing cannot be reproduced in a gist, please add more information here.
