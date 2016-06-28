# mochawesome-screenshots
This is a fork of Mochawesome Screenshots which was a fork of Mochawesome(MochawesomePlusPlus) reporter. Original Mochawesome Screenshots took the screenshot inside the report, and this version adds the reference to the screenshot on failed tests, letting you take a screenshot in your framework at your own discretion.

No NPM installation yet, not sure if merging back or changing features:

Usage remains the same as Mocahwesome.

In your configuration file:
```
  framework: 'mocha',

  mochaOpts: {
      reporter: 'mochawesome-screenshots',
      reporterOptions: {
          reportDir: 'customReportDir',
          reportName: 'customReportName',
          reportTitle: 'customReportTitle',
          takePassedScreenshot: false,
          clearOldScreenshots: true
      },
      timeout: 600000
  },
```
