name: Bug report
description: File a bug report.
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report a bug! Please fill out the bug report below as best you can.

        If you need support ASAP/email support, email me [here](mailto:aqplemine@proton.me).

        For security vulnerabilities, please report them DIRECTLY to me [here](mailto:aqplemine@proton.me).

        IMPORTANT NOTE: It would be nice if you could ALSO make a [jam.dev](https://jam.dev) report, along with this issue. Make a jam report [here](https://normalmath.vercel.app/jam.html)

        If you're making a jam report, you do NOT need to attach it to this issue. I will see the report in the backend, just tell me you made one, and I can see it. (:
  - type: textarea
    id: bug-description
    attributes:
      label: Describe the bug
      description: |
        A clear and concise description of what the bug is. The more information you can provide, the easier it will be for us to investigate and fix the issue.
      placeholder: "When I click a game launch button, nothing happens."
    validations:
      required: true
  - type: upload
    id: screenshots
    attributes:
      label: Screenshots or screen recordings
      description: |
        If applicable, please upload any screenshots or screen recordings that show the bug. This can help us understand the issue better and speed up the investigation. You can also make a jam report, just let me know if you made one. No need to attach it here.
  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to reproduce
      description: A clear and concise list of steps to reproduce the behavior.
      placeholder: |
        1. Go to '...'
        2. Click on '....'
        3. Scroll down to '....'
        4. See error
  - type: dropdown
    id: browsers
    attributes:
      label: What browsers are you seeing the problem on (if applicable)?
      description: You may select multiple browsers if the issue occurs on more than one.
      multiple: true
      options:
        - Firefox
        - Chrome
        - Safari
        - Microsoft Edge
        - Other (type the name somewhere else in here.)
  - type: textarea
    id: backtrace
    attributes:
      label: Backtrace
      description: |
        If you have a backtrace from a server error, please copy and paste it here.
        This will be automatically formatted into code, so no need for backticks.
        If you make a jam report, I can see the browser's developer log output.
      render: text
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: |
        Please copy and paste any relevant log output.
        Logs could include browser console logs, server logs, or any error messages you see.
        This will be automatically formatted into code, so no need for backticks.
        If you make a jam report, I can see the browser's developer log output.
      render: text
