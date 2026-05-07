name: Feature Request
description: File a feature request.
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to request a feature! Please fill out the feature info below as best you can.

        If you need support ASAP/email support, email me [here](mailto:aqplemine@proton.me).

        For security vulnerabilities, please report them DIRECTLY to me [here](mailto:aqplemine@proton.me).

        IMPORTANT NOTE: It would be nice if you could ALSO make a [jam.dev](https://jam.dev) report, along with this issue. Make a jam report [here](https://normalmath.vercel.app/jam.html)

        If you're making a jam report, you do NOT need to attach it to this issue. I will see the report in the backend, just tell me you made one, and I can see it. (:
  - type: textarea
    id: feature-description
    attributes:
      label: Describe the feature
      description: |
        A clear and concise description of what you want adde. The more information you can provide, the easier it will be for us to think about adding it.
      placeholder: "Add more themes."
    validations:
      required: true
  - type: upload
    id: screenshots
    attributes:
      label: Screenshots or screen recordings
      description: |
        If applicable, please upload any screenshots or screen recordings that show where you want this added. This can help us understand where you want this feature to be added. You can also make a jam report, just let me know if you made one. No need to attach it here.
  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to reproduce, where you want it added
      description: A clear and concise list of steps to find where you'd like this added.
      placeholder: |
        1. Go to '...'
        2. Click on '....'
        3. Scroll down to '....'
        4. See something that could be added.
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
        If you have a backtrace from a server log, please copy and paste it here.
        This will be automatically formatted into code, so no need for backticks.
        If you make a jam report, I can see the browser's developer log output.
      render: text
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: |
        Please copy and paste any relevant log output.
        Logs could include browser console logs, server logs, or any general messages you see.
        This will be automatically formatted into code, so no need for backticks.
        If you make a jam report, I can see the browser's developer log output.
      render: text
