# BackgroundTabLimit

## Information
https://developer.salesforce.com/docs/component-library/bundle/lightning:backgroundUtilityItem/documentation

Implement the lightning:backgroundUtilityItem interface to allow a component to be used as an app-level component that is created when the app loads, and runs code without rendering itself in the app UI.

Components that implement this interface are added to the app through the Select Utility Items milestone in Setup.

This example shows how to implement a background utility item that listens for lightning:tabCreated events when the app loads, and invokes lightning:workspaceAPI methods to prevent more than 10 tabs from opening. 

## Add utility to Lightning App

1. Go to `Setup`
2. Go to `Apps > App Manager`
3. Select the `Lightning` app you want to add it to
4. Go to `App Settings > Utility Items` and click `Add Utility Item`
5. Add `BackgroundTabLimit`