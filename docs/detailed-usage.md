---
layout: default
title: Detailed Usage Guide
nav_order: 2
---

# Detailed Usage Guide

This guide provides in-depth information about using CyJet's features and capabilities.

## Tool Window Overview

The Cypress button in your Run/Debug toolbar is your primary interface for interacting with Cypress tests. Here's what you'll find:

### Open Cypress GUI Option
- Open your project in IntelliJ IDEA
- Click the "Cypress" button in the Run/Debug toolbar
- Select "Open Cypress GUI" option
- The plugin will locate your cypress folder and the Cypress Test Runner GUI will open in a window

### Run Cypress Spec Option
- Open your project in IntelliJ IDEA
- Click the "Cypress" button in the Run/Debug toolbar
- Select "Run Cypress Spec" option
- Spec selection window will open and allow you to:
  - See the list of all test specs in your project
  - Search for your test spec
  - Select one or more test specs by clicking on the checkboxes
  - Select the preferred browser for test execution

## Running Tests

### Single Spec Execution
1. Select a test spec in the Spec Selector window's Test Explorer list
2. Choose your preferred browser from the options
3. Click the "Run selected tests" button
4. Test execution opens IDE's Run/Debug window, to show the test execution progress and results

### Batch Spec Execution
1. Choose your preferred browser from the options
2. Select multiple test specs in the Spec Selector window's Test Explorer list
3. Click the "Run selected tests" button
   - Or don't select any test spec and click "Run all tests" to run all tests in the project
4. Test execution opens IDE's Run/Debug window, to show the test execution progress and results

### Test Execution Status & Results
- The current version of CyJet runs tests **only in the `headless mode`**. Support for `headed mode` is coming soon!

### Notifications
- Get notified about test initiation/errors as IDE Notifications

## Troubleshooting

### Common Issues
1. **Plugin Frozen**
   - Minimize IDE and reopen
   - Switch to a different opened window/app and switch back to IDE

2. **Browser Launch Failed**
   - Verify browser installation
   - Verify browser configuration in the Cypress project in case of WebKit browser

3. **Cypress Binary Not Found**
   - Run command `npx cypress install` at your project root in the terminal before using CyJet

## Best Practices

### Project Organization
- Keep specs in a consistent directory structure
- Use descriptive test names

### Performance Optimization
- In case your Cypress project is inside a sub-folder of your main project, open the IDE at the Cypress project root

## Additional Resources

- [Plugin Demo](https://youtu.be/fyziOvFuHto)
- [Community Forums](https://cyjet.example.com/community)